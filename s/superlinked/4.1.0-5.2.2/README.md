# Comparing `tmp/superlinked-4.1.0.tar.gz` & `tmp/superlinked-5.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superlinked-4.1.0.tar", max compression
+gzip compressed data, was "superlinked-5.2.2.tar", max compression
```

## Comparing `superlinked-4.1.0.tar` & `superlinked-5.2.2.tar`

### file list

```diff
@@ -1,228 +1,217 @@
--rw-r--r--   0        0        0    11354 2024-05-22 14:45:11.466898 superlinked-4.1.0/LICENSE
--rw-r--r--   0        0        0    28655 2024-05-22 14:45:11.466898 superlinked-4.1.0/NOTICE
--rw-r--r--   0        0        0     6840 2024-05-22 14:45:11.466898 superlinked-4.1.0/PYPI_README.md
--rw-r--r--   0        0        0     3698 2024-05-22 14:48:01.196184 superlinked-4.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.510898 superlinked-4.1.0/superlinked/evaluation/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.510898 superlinked-4.1.0/superlinked/evaluation/charts/__init__.py
--rw-r--r--   0        0        0     5601 2024-05-22 14:45:11.510898 superlinked-4.1.0/superlinked/evaluation/charts/recency_plotter.py
--rw-r--r--   0        0        0     8077 2024-05-22 14:45:11.510898 superlinked-4.1.0/superlinked/evaluation/vector_sampler.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.510898 superlinked-4.1.0/superlinked/framework/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.510898 superlinked-4.1.0/superlinked/framework/common/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/calculation/__init__.py
--rw-r--r--   0        0        0      742 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/calculation/distance_metric.py
--rw-r--r--   0        0        0     1621 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/calculation/vector_similarity.py
--rw-r--r--   0        0        0      805 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/const.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/__init__.py
--rw-r--r--   0        0        0     3624 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/aggregation_node.py
--rw-r--r--   0        0        0     2280 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/categorical_similarity_node.py
--rw-r--r--   0        0        0     1515 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/chunking_node.py
--rw-r--r--   0        0        0     2089 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/comparison_filter_node.py
--rw-r--r--   0        0        0     2586 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/concatenation_node.py
--rw-r--r--   0        0        0     1093 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/constant_node.py
--rw-r--r--   0        0        0     4985 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/context.py
--rw-r--r--   0        0        0     1846 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/custom_node.py
--rw-r--r--   0        0        0     5923 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/dag.py
--rw-r--r--   0        0        0     1338 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/dag_effect.py
--rw-r--r--   0        0        0     3664 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/event_aggregation_node.py
--rw-r--r--   0        0        0     1004 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/exception.py
--rw-r--r--   0        0        0     2023 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/index_node.py
--rw-r--r--   0        0        0     1415 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/named_function_node.py
--rw-r--r--   0        0        0     4465 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/node.py
--rw-r--r--   0        0        0     2414 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/number_embedding_node.py
--rw-r--r--   0        0        0     2368 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/number_similarity_node.py
--rw-r--r--   0        0        0     1620 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/period_time.py
--rw-r--r--   0        0        0      897 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/persistence_params.py
--rw-r--r--   0        0        0     2449 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/recency_node.py
--rw-r--r--   0        0        0     1128 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/resolved_schema_reference.py
--rw-r--r--   0        0        0     2019 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/schema_dag.py
--rw-r--r--   0        0        0     1384 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/schema_field_node.py
--rw-r--r--   0        0        0     1378 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/schema_object_reference.py
--rw-r--r--   0        0        0     2062 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/dag/text_embedding_node.py
--rw-r--r--   0        0        0     8081 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/data_types.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/embedding/__init__.py
--rw-r--r--   0        0        0     5281 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/embedding/categorical_similarity_embedding.py
--rw-r--r--   0        0        0     5890 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/embedding/chunking_util.py
--rw-r--r--   0        0        0     1576 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/embedding/custom_embedding.py
--rw-r--r--   0        0        0     1280 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/embedding/embedding.py
--rw-r--r--   0        0        0     3138 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/embedding/number_embedding.py
--rw-r--r--   0        0        0     2424 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/embedding/number_similarity_embedding.py
--rw-r--r--   0        0        0     8046 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/embedding/recency_embedding.py
--rw-r--r--   0        0        0     2134 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/embedding/sentence_transformer_embedding.py
--rw-r--r--   0        0        0     1250 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/exception.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/interface/__init__.py
--rw-r--r--   0        0        0     5851 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/interface/comparison_operand.py
--rw-r--r--   0        0        0      841 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/interface/comparison_operation_type.py
--rw-r--r--   0        0        0      808 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/interface/has_aggregation.py
--rw-r--r--   0        0        0      718 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/interface/has_length.py
--rw-r--r--   0        0        0      836 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/interface/has_multiplier.py
--rw-r--r--   0        0        0      940 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/interface/weighted.py
--rw-r--r--   0        0        0     1322 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/observable.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/parser/__init__.py
--rw-r--r--   0        0        0     5879 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/parser/data_parser.py
--rw-r--r--   0        0        0     4806 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/parser/dataframe_parser.py
--rw-r--r--   0        0        0      814 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/parser/exception.py
--rw-r--r--   0        0        0     4379 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/parser/json_parser.py
--rw-r--r--   0        0        0     1354 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/parser/parsed_schema.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/__init__.py
--rw-r--r--   0        0        0     1072 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/event_schema.py
--rw-r--r--   0        0        0     1964 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/event_schema_object.py
--rw-r--r--   0        0        0     1014 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/exception.py
--rw-r--r--   0        0        0      627 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/general_type.py
--rw-r--r--   0        0        0     1392 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/id_schema_object.py
--rw-r--r--   0        0        0     1178 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/schema.py
--rw-r--r--   0        0        0     3189 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/schema_decorator.py
--rw-r--r--   0        0        0     3209 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/schema_factory.py
--rw-r--r--   0        0        0     5687 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/schema_object.py
--rw-r--r--   0        0        0     3170 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/schema_reference.py
--rw-r--r--   0        0        0      686 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/schema_type.py
--rw-r--r--   0        0        0     3201 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/schema/schema_validator.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/source/__init__.py
--rw-r--r--   0        0        0      857 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/source/source.py
--rw-r--r--   0        0        0      647 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/source/types.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/space/__init__.py
--rw-r--r--   0        0        0     4398 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/space/aggregation.py
--rw-r--r--   0        0        0     2121 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/space/normalization.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/storage/__init__.py
--rw-r--r--   0        0        0      857 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/storage/entity.py
--rw-r--r--   0        0        0      878 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/storage/entity_data.py
--rw-r--r--   0        0        0      696 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/storage/entity_id.py
--rw-r--r--   0        0        0      627 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/storage/exception.py
--rw-r--r--   0        0        0     1516 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/storage/field.py
--rw-r--r--   0        0        0     2535 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/storage/field_data.py
--rw-r--r--   0        0        0      733 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/storage/field_data_type.py
--rw-r--r--   0        0        0     3213 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/storage/field_encoder.py
--rw-r--r--   0        0        0      746 2024-05-22 14:45:11.514898 superlinked-4.1.0/superlinked/framework/common/storage/persistence_type.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage/search_index_creation/__init__.py
--rw-r--r--   0        0        0     1216 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py
--rw-r--r--   0        0        0      671 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage/search_index_creation/search_algorithm.py
--rw-r--r--   0        0        0      692 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py
--rw-r--r--   0        0        0     2306 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage/vdb_connector.py
--rw-r--r--   0        0        0     1075 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage/vdb_knn_search_params.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage_manager/__init__.py
--rw-r--r--   0        0        0     6065 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage_manager/entity_builder.py
--rw-r--r--   0        0        0     2143 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage_manager/field_type_converter.py
--rw-r--r--   0        0        0     1059 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage_manager/knn_search_params.py
--rw-r--r--   0        0        0      769 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage_manager/node_result_params.py
--rw-r--r--   0        0        0    13379 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage_manager/storage_manager.py
--rw-r--r--   0        0        0     1462 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/storage_manager/storage_naming.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/util/__init__.py
--rw-r--r--   0        0        0      787 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/util/collection_util.py
--rw-r--r--   0        0        0     2074 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/util/dot_separated_path_util.py
--rw-r--r--   0        0        0      707 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/util/immutable_model.py
--rw-r--r--   0        0        0     1058 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/util/named_function_evaluator.py
--rw-r--r--   0        0        0      886 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/util/schema_util.py
--rw-r--r--   0        0        0     1642 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/util/string_util.py
--rw-r--r--   0        0        0      907 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/util/time_util.py
--rw-r--r--   0        0        0     1189 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/util/type_util.py
--rw-r--r--   0        0        0     4383 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/common/util/type_validator.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/compiler/__init__.py
--rw-r--r--   0        0        0     2556 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/compiler/online_schema_dag_compiler.py
--rw-r--r--   0        0        0      108 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/data_loader/__init__.py
--rw-r--r--   0        0        0      726 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/data_loader/data_loader.py
--rw-r--r--   0        0        0      221 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/__init__.py
--rw-r--r--   0        0        0      719 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/exception.py
--rw-r--r--   0        0        0     4467 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/executor.py
--rw-r--r--   0        0        0      124 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/in_memory/__init__.py
--rw-r--r--   0        0        0     7228 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py
--rw-r--r--   0        0        0      119 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/query/__init__.py
--rw-r--r--   0        0        0     6478 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/query/query_executor.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/rest/__init__.py
--rw-r--r--   0        0        0     1540 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/rest/rest_configuration.py
--rw-r--r--   0        0        0      818 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/rest/rest_descriptor.py
--rw-r--r--   0        0        0     4395 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/rest/rest_executor.py
--rw-r--r--   0        0        0     3236 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/executor/rest/rest_handler.py
--rw-r--r--   0        0        0      176 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/index/__init__.py
--rw-r--r--   0        0        0     1904 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/index/effect.py
--rw-r--r--   0        0        0    10985 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/index/index.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/index/util/__init__.py
--rw-r--r--   0        0        0     1516 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/index/util/aggregation_effect_group.py
--rw-r--r--   0        0        0     2448 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/index/util/aggregation_node_util.py
--rw-r--r--   0        0        0     6203 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py
--rw-r--r--   0        0        0     2557 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py
--rw-r--r--   0        0        0     3673 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/index/util/event_aggregation_node_util.py
--rw-r--r--   0        0        0      192 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/__init__.py
--rw-r--r--   0        0        0     1183 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/param.py
--rw-r--r--   0        0        0     3798 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/param_evaluator.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/predicate/__init__.py
--rw-r--r--   0        0        0      756 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/predicate/binary_op.py
--rw-r--r--   0        0        0     1521 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/predicate/binary_predicate.py
--rw-r--r--   0        0        0      924 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/predicate/evaluated_binary_predicate.py
--rw-r--r--   0        0        0     1128 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/predicate/query_predicate.py
--rw-r--r--   0        0        0    13173 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/query.py
--rw-r--r--   0        0        0     6223 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/query_filters.py
--rw-r--r--   0        0        0     6990 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/query_vector_factory.py
--rw-r--r--   0        0        0     3329 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/query_weighting.py
--rw-r--r--   0        0        0     2457 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/query/result.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/registry/__init__.py
--rw-r--r--   0        0        0      636 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/registry/exception.py
--rw-r--r--   0        0        0     1984 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/registry/superlinked_registry.py
--rw-r--r--   0        0        0      214 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/source/__init__.py
--rw-r--r--   0        0        0     2773 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/source/in_memory_source.py
--rw-r--r--   0        0        0     1987 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/source/rest_source.py
--rw-r--r--   0        0        0     1144 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/source/source.py
--rw-r--r--   0        0        0      183 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/space/__init__.py
--rw-r--r--   0        0        0     7479 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/space/categorical_similarity_space.py
--rw-r--r--   0        0        0     5509 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/space/custom_space.py
--rw-r--r--   0        0        0      856 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/space/exception.py
--rw-r--r--   0        0        0     8215 2024-05-22 14:45:11.518898 superlinked-4.1.0/superlinked/framework/dsl/space/number_space.py
--rw-r--r--   0        0        0     8456 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/dsl/space/recency_space.py
--rw-r--r--   0        0        0     2743 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/dsl/space/space.py
--rw-r--r--   0        0        0     1295 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/dsl/space/space_field_set.py
--rw-r--r--   0        0        0     4804 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/dsl/space/text_similarity_space.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/evaluator/__init__.py
--rw-r--r--   0        0        0     1043 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/evaluator/dag_evaluator.py
--rw-r--r--   0        0        0     5222 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/evaluator/online_dag_evaluator.py
--rw-r--r--   0        0        0     2237 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/evaluator/query_dag_evaluator.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/new_storage/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/new_storage/in_memory/__init__.py
--rw-r--r--   0        0        0      787 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/new_storage/in_memory/exception.py
--rw-r--r--   0        0        0     6127 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/new_storage/in_memory/in_memory_knn_search.py
--rw-r--r--   0        0        0     6408 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/new_storage/in_memory/in_memory_vdb.py
--rw-r--r--   0        0        0      921 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/new_storage/in_memory/index_config.py
--rw-r--r--   0        0        0     1305 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/new_storage/in_memory/json_codec.py
--rw-r--r--   0        0        0     1562 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/new_storage/in_memory/object_serializer.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/__init__.py
--rw-r--r--   0        0        0      801 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/batched_chunk_input_item.py
--rw-r--r--   0        0        0     7597 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/default_online_node.py
--rw-r--r--   0        0        0     1129 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/evaluation_result.py
--rw-r--r--   0        0        0      768 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/exception.py
--rw-r--r--   0        0        0     6395 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_aggregation_node.py
--rw-r--r--   0        0        0     3288 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_categorical_similarity_node.py
--rw-r--r--   0        0        0     3540 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_chunking_node.py
--rw-r--r--   0        0        0     2330 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_comparison_filter_node.py
--rw-r--r--   0        0        0     5221 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_concatenation_node.py
--rw-r--r--   0        0        0     2115 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_constant_node.py
--rw-r--r--   0        0        0     3435 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_custom_node.py
--rw-r--r--   0        0        0     8157 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_event_aggregation_node.py
--rw-r--r--   0        0        0     4135 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_index_node.py
--rw-r--r--   0        0        0     2434 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_named_function_node.py
--rw-r--r--   0        0        0     4996 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_node.py
--rw-r--r--   0        0        0     5773 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_node_registry.py
--rw-r--r--   0        0        0     3162 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_number_embedding_node.py
--rw-r--r--   0        0        0     3272 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_number_similarity_node.py
--rw-r--r--   0        0        0     2796 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_recency_node.py
--rw-r--r--   0        0        0     3732 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_schema_dag.py
--rw-r--r--   0        0        0     3509 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_schema_field_node.py
--rw-r--r--   0        0        0     3338 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/online_text_embedding_node.py
--rw-r--r--   0        0        0      794 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/parent_results.py
--rw-r--r--   0        0        0     1322 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/dag/parent_validator.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/source/__init__.py
--rw-r--r--   0        0        0     3486 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/source/in_memory_data_processor.py
--rw-r--r--   0        0        0     1539 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/source/in_memory_object_writer.py
--rw-r--r--   0        0        0     1752 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/source/in_memory_source.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/store_manager/__init__.py
--rw-r--r--   0        0        0     5707 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/online/store_manager/evaluation_result_store_manager.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/storage/__init__.py
--rw-r--r--   0        0        0     2587 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/storage/entity.py
--rw-r--r--   0        0        0     1936 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/storage/entity_store.py
--rw-r--r--   0        0        0     4966 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/storage/entity_store_manager.py
--rw-r--r--   0        0        0     1304 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/storage/field.py
--rw-r--r--   0        0        0     8076 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/storage/in_memory_entity_store.py
--rw-r--r--   0        0        0     1209 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/storage/in_memory_object_store.py
--rw-r--r--   0        0        0     1125 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/storage/object_store.py
--rw-r--r--   0        0        0     1570 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/storage/object_store_manager.py
--rw-r--r--   0        0        0     3317 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/framework/storage/persistable_dict.py
--rw-r--r--   0        0        0        0 2024-05-22 14:45:11.522899 superlinked-4.1.0/superlinked/py.typed
--rw-r--r--   0        0        0     8320 1970-01-01 00:00:00.000000 superlinked-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11354 2024-05-23 18:55:26.344260 superlinked-5.2.2/LICENSE
+-rw-r--r--   0        0        0    28655 2024-05-23 18:55:26.344260 superlinked-5.2.2/NOTICE
+-rw-r--r--   0        0        0     6840 2024-05-23 18:55:26.344260 superlinked-5.2.2/PYPI_README.md
+-rw-r--r--   0        0        0     3698 2024-05-23 18:58:32.028026 superlinked-5.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/evaluation/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/evaluation/charts/__init__.py
+-rw-r--r--   0        0        0     5601 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/evaluation/charts/recency_plotter.py
+-rw-r--r--   0        0        0     9028 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/evaluation/vector_sampler.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/calculation/__init__.py
+-rw-r--r--   0        0        0      742 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/calculation/distance_metric.py
+-rw-r--r--   0        0        0     1510 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/calculation/vector_similarity.py
+-rw-r--r--   0        0        0      805 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/const.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/__init__.py
+-rw-r--r--   0        0        0     3644 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/aggregation_node.py
+-rw-r--r--   0        0        0     2288 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/categorical_similarity_node.py
+-rw-r--r--   0        0        0     1520 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/chunking_node.py
+-rw-r--r--   0        0        0     2095 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/comparison_filter_node.py
+-rw-r--r--   0        0        0     2606 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/concatenation_node.py
+-rw-r--r--   0        0        0     1106 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/constant_node.py
+-rw-r--r--   0        0        0     4985 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/context.py
+-rw-r--r--   0        0        0     1854 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/custom_node.py
+-rw-r--r--   0        0        0     5923 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/dag.py
+-rw-r--r--   0        0        0     1338 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/dag_effect.py
+-rw-r--r--   0        0        0     3687 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/event_aggregation_node.py
+-rw-r--r--   0        0        0     1004 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/exception.py
+-rw-r--r--   0        0        0     2043 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/index_node.py
+-rw-r--r--   0        0        0     1428 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/named_function_node.py
+-rw-r--r--   0        0        0     4723 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/node.py
+-rw-r--r--   0        0        0     2422 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/number_embedding_node.py
+-rw-r--r--   0        0        0     2376 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/number_similarity_node.py
+-rw-r--r--   0        0        0     1620 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/period_time.py
+-rw-r--r--   0        0        0      897 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/persistence_params.py
+-rw-r--r--   0        0        0     2457 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/recency_node.py
+-rw-r--r--   0        0        0     1128 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/resolved_schema_reference.py
+-rw-r--r--   0        0        0     2019 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/schema_dag.py
+-rw-r--r--   0        0        0     1463 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/schema_field_node.py
+-rw-r--r--   0        0        0     1378 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/schema_object_reference.py
+-rw-r--r--   0        0        0     2035 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/dag/text_embedding_node.py
+-rw-r--r--   0        0        0     8107 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/data_types.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/embedding/__init__.py
+-rw-r--r--   0        0        0     5201 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/embedding/categorical_similarity_embedding.py
+-rw-r--r--   0        0        0     5890 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/embedding/chunking_util.py
+-rw-r--r--   0        0        0     1507 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/embedding/custom_embedding.py
+-rw-r--r--   0        0        0     1280 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/embedding/embedding.py
+-rw-r--r--   0        0        0     3138 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/embedding/number_embedding.py
+-rw-r--r--   0        0        0     2424 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/embedding/number_similarity_embedding.py
+-rw-r--r--   0        0        0     8046 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/embedding/recency_embedding.py
+-rw-r--r--   0        0        0     2134 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/embedding/sentence_transformer_embedding.py
+-rw-r--r--   0        0        0     1250 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/exception.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/interface/__init__.py
+-rw-r--r--   0        0        0     5851 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/interface/comparison_operand.py
+-rw-r--r--   0        0        0      841 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/interface/comparison_operation_type.py
+-rw-r--r--   0        0        0      808 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/interface/has_aggregation.py
+-rw-r--r--   0        0        0      718 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/interface/has_length.py
+-rw-r--r--   0        0        0      836 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/interface/has_multiplier.py
+-rw-r--r--   0        0        0      940 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/interface/weighted.py
+-rw-r--r--   0        0        0     1322 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/observable.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/parser/__init__.py
+-rw-r--r--   0        0        0     5829 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/parser/data_parser.py
+-rw-r--r--   0        0        0     5402 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/parser/dataframe_parser.py
+-rw-r--r--   0        0        0      814 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/parser/exception.py
+-rw-r--r--   0        0        0     4628 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/parser/json_parser.py
+-rw-r--r--   0        0        0     1354 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/parser/parsed_schema.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/schema/__init__.py
+-rw-r--r--   0        0        0     1072 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/schema/event_schema.py
+-rw-r--r--   0        0        0     1964 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/schema/event_schema_object.py
+-rw-r--r--   0        0        0     1014 2024-05-23 18:55:26.392260 superlinked-5.2.2/superlinked/framework/common/schema/exception.py
+-rw-r--r--   0        0        0      627 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/schema/general_type.py
+-rw-r--r--   0        0        0     1392 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/schema/id_schema_object.py
+-rw-r--r--   0        0        0     1178 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/schema/schema.py
+-rw-r--r--   0        0        0     3189 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/schema/schema_decorator.py
+-rw-r--r--   0        0        0     3228 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/schema/schema_factory.py
+-rw-r--r--   0        0        0     5701 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/schema/schema_object.py
+-rw-r--r--   0        0        0     3170 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/schema/schema_reference.py
+-rw-r--r--   0        0        0      686 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/schema/schema_type.py
+-rw-r--r--   0        0        0     3220 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/schema/schema_validator.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/source/__init__.py
+-rw-r--r--   0        0        0      857 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/source/source.py
+-rw-r--r--   0        0        0      647 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/source/types.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/space/__init__.py
+-rw-r--r--   0        0        0     4398 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/space/aggregation.py
+-rw-r--r--   0        0        0     2055 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/space/normalization.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage/__init__.py
+-rw-r--r--   0        0        0      820 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage/entity.py
+-rw-r--r--   0        0        0      855 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage/entity_data.py
+-rw-r--r--   0        0        0      696 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage/entity_id.py
+-rw-r--r--   0        0        0      627 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage/exception.py
+-rw-r--r--   0        0        0     1656 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage/field.py
+-rw-r--r--   0        0        0     2616 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage/field_data.py
+-rw-r--r--   0        0        0      757 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage/field_data_type.py
+-rw-r--r--   0        0        0     3514 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage/field_encoder.py
+-rw-r--r--   0        0        0     2772 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage/field_type_converter.py
+-rw-r--r--   0        0        0      746 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage/persistence_type.py
+-rw-r--r--   0        0        0      769 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage/result_entity_data.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage/search_index_creation/__init__.py
+-rw-r--r--   0        0        0     1242 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py
+-rw-r--r--   0        0        0      671 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage/search_index_creation/search_algorithm.py
+-rw-r--r--   0        0        0      692 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py
+-rw-r--r--   0        0        0     2397 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage/vdb_connector.py
+-rw-r--r--   0        0        0     1095 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage/vdb_knn_search_params.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage_manager/__init__.py
+-rw-r--r--   0        0        0     5459 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage_manager/admin_fields.py
+-rw-r--r--   0        0        0     5549 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage_manager/entity_builder.py
+-rw-r--r--   0        0        0      720 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage_manager/header.py
+-rw-r--r--   0        0        0     1079 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage_manager/knn_search_params.py
+-rw-r--r--   0        0        0      932 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage_manager/search_result_item.py
+-rw-r--r--   0        0        0    16654 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage_manager/storage_manager.py
+-rw-r--r--   0        0        0     1533 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/storage_manager/storage_naming.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/util/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/util/collection_util.py
+-rw-r--r--   0        0        0     2074 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/util/dot_separated_path_util.py
+-rw-r--r--   0        0        0     1777 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/util/generic_class_util.py
+-rw-r--r--   0        0        0      707 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/util/immutable_model.py
+-rw-r--r--   0        0        0     1058 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/util/named_function_evaluator.py
+-rw-r--r--   0        0        0     1642 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/util/string_util.py
+-rw-r--r--   0        0        0      907 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/util/time_util.py
+-rw-r--r--   0        0        0     4383 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/common/util/type_validator.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/compiler/__init__.py
+-rw-r--r--   0        0        0     2399 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/compiler/online_schema_dag_compiler.py
+-rw-r--r--   0        0        0      108 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/__init__.py
+-rw-r--r--   0        0        0      221 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/executor/__init__.py
+-rw-r--r--   0        0        0      719 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/executor/exception.py
+-rw-r--r--   0        0        0     3836 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/executor/executor.py
+-rw-r--r--   0        0        0      124 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/executor/in_memory/__init__.py
+-rw-r--r--   0        0        0     7115 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py
+-rw-r--r--   0        0        0      119 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/executor/query/__init__.py
+-rw-r--r--   0        0        0     6804 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/executor/query/query_executor.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/executor/rest/__init__.py
+-rw-r--r--   0        0        0     1540 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/executor/rest/rest_configuration.py
+-rw-r--r--   0        0        0      818 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/executor/rest/rest_descriptor.py
+-rw-r--r--   0        0        0     4834 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/executor/rest/rest_executor.py
+-rw-r--r--   0        0        0     3236 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/executor/rest/rest_handler.py
+-rw-r--r--   0        0        0      176 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/index/__init__.py
+-rw-r--r--   0        0        0     1904 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/index/effect.py
+-rw-r--r--   0        0        0    10985 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/index/index.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/index/util/__init__.py
+-rw-r--r--   0        0        0     1516 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/index/util/aggregation_effect_group.py
+-rw-r--r--   0        0        0     2448 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/index/util/aggregation_node_util.py
+-rw-r--r--   0        0        0     6203 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py
+-rw-r--r--   0        0        0     2557 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py
+-rw-r--r--   0        0        0     3673 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/index/util/event_aggregation_node_util.py
+-rw-r--r--   0        0        0      192 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/query/__init__.py
+-rw-r--r--   0        0        0     1183 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/query/param.py
+-rw-r--r--   0        0        0     3798 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/query/param_evaluator.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/query/predicate/__init__.py
+-rw-r--r--   0        0        0      756 2024-05-23 18:55:26.396260 superlinked-5.2.2/superlinked/framework/dsl/query/predicate/binary_op.py
+-rw-r--r--   0        0        0     1521 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/query/predicate/binary_predicate.py
+-rw-r--r--   0        0        0      924 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/query/predicate/evaluated_binary_predicate.py
+-rw-r--r--   0        0        0     1128 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/query/predicate/query_predicate.py
+-rw-r--r--   0        0        0    13227 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/query/query.py
+-rw-r--r--   0        0        0     6223 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/query/query_filters.py
+-rw-r--r--   0        0        0     6842 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/query/query_vector_factory.py
+-rw-r--r--   0        0        0     3329 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/query/query_weighting.py
+-rw-r--r--   0        0        0     2613 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/query/result.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/registry/__init__.py
+-rw-r--r--   0        0        0      636 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/registry/exception.py
+-rw-r--r--   0        0        0     1330 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/registry/superlinked_registry.py
+-rw-r--r--   0        0        0      214 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/source/__init__.py
+-rw-r--r--   0        0        0     2225 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/source/data_loader_source.py
+-rw-r--r--   0        0        0     2773 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/source/in_memory_source.py
+-rw-r--r--   0        0        0     1987 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/source/rest_source.py
+-rw-r--r--   0        0        0     1144 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/source/source.py
+-rw-r--r--   0        0        0      183 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/space/__init__.py
+-rw-r--r--   0        0        0     7479 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/space/categorical_similarity_space.py
+-rw-r--r--   0        0        0     5509 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/space/custom_space.py
+-rw-r--r--   0        0        0      856 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/space/exception.py
+-rw-r--r--   0        0        0     8215 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/space/number_space.py
+-rw-r--r--   0        0        0     8456 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/space/recency_space.py
+-rw-r--r--   0        0        0     2743 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/space/space.py
+-rw-r--r--   0        0        0     1295 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/space/space_field_set.py
+-rw-r--r--   0        0        0     4804 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/dsl/space/text_similarity_space.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/evaluator/__init__.py
+-rw-r--r--   0        0        0     1043 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/evaluator/dag_evaluator.py
+-rw-r--r--   0        0        0     4807 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/evaluator/online_dag_evaluator.py
+-rw-r--r--   0        0        0     2237 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/evaluator/query_dag_evaluator.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/__init__.py
+-rw-r--r--   0        0        0      801 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/batched_chunk_input_item.py
+-rw-r--r--   0        0        0     7597 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/default_online_node.py
+-rw-r--r--   0        0        0     1213 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/evaluation_result.py
+-rw-r--r--   0        0        0      768 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/exception.py
+-rw-r--r--   0        0        0     6312 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/online_aggregation_node.py
+-rw-r--r--   0        0        0     3205 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/online_categorical_similarity_node.py
+-rw-r--r--   0        0        0     3457 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/online_chunking_node.py
+-rw-r--r--   0        0        0     2247 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/online_comparison_filter_node.py
+-rw-r--r--   0        0        0     5138 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/online_concatenation_node.py
+-rw-r--r--   0        0        0     2032 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/online_constant_node.py
+-rw-r--r--   0        0        0     3283 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/online_custom_node.py
+-rw-r--r--   0        0        0     7908 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/online_event_aggregation_node.py
+-rw-r--r--   0        0        0     4052 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/online_index_node.py
+-rw-r--r--   0        0        0     2351 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/online_named_function_node.py
+-rw-r--r--   0        0        0     5089 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/online_node.py
+-rw-r--r--   0        0        0     5690 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/online_node_registry.py
+-rw-r--r--   0        0        0     3079 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/online_number_embedding_node.py
+-rw-r--r--   0        0        0     3189 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/online_number_similarity_node.py
+-rw-r--r--   0        0        0     2713 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/online_recency_node.py
+-rw-r--r--   0        0        0     3732 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/online_schema_dag.py
+-rw-r--r--   0        0        0     3426 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/online_schema_field_node.py
+-rw-r--r--   0        0        0     3255 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/online_text_embedding_node.py
+-rw-r--r--   0        0        0      794 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/parent_results.py
+-rw-r--r--   0        0        0     1322 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/dag/parent_validator.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/source/__init__.py
+-rw-r--r--   0        0        0     3486 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/source/in_memory_data_processor.py
+-rw-r--r--   0        0        0     1437 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/source/in_memory_object_writer.py
+-rw-r--r--   0        0        0     1752 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/online/source/in_memory_source.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/storage/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/storage/in_memory/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/storage/in_memory/exception.py
+-rw-r--r--   0        0        0     6725 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/storage/in_memory/in_memory_search.py
+-rw-r--r--   0        0        0     7121 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/storage/in_memory/in_memory_vdb.py
+-rw-r--r--   0        0        0      921 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/storage/in_memory/index_config.py
+-rw-r--r--   0        0        0     1305 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/storage/in_memory/json_codec.py
+-rw-r--r--   0        0        0     1562 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/framework/storage/in_memory/object_serializer.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:55:26.400260 superlinked-5.2.2/superlinked/py.typed
+-rw-r--r--   0        0        0     8320 1970-01-01 00:00:00.000000 superlinked-5.2.2/PKG-INFO
```

### Comparing `superlinked-4.1.0/LICENSE` & `superlinked-5.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/NOTICE` & `superlinked-5.2.2/NOTICE`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/PYPI_README.md` & `superlinked-5.2.2/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/pyproject.toml` & `superlinked-5.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "superlinked"
-version = "4.1.0"  # The version will be dynamically updated
+version = "5.2.2"  # The version will be dynamically updated
 description = "The Superlinked vector computing library"
 authors = ["Superlinked Release <release@superlinked.com>"]
 readme = "PYPI_README.md"
 license = "Apache-2.0"
 include = ["NOTICE"]
 
 [tool.poetry.dependencies]
```

### Comparing `superlinked-4.1.0/superlinked/evaluation/charts/recency_plotter.py` & `superlinked-5.2.2/superlinked/evaluation/charts/recency_plotter.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/evaluation/vector_sampler.py` & `superlinked-5.2.2/superlinked/evaluation/vector_sampler.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,21 +11,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Any, cast
 
 import numpy as np
-from numpy import typing as npt
+from beartype.typing import Sequence
 
+from superlinked.framework.common.data_types import NPArray
 from superlinked.framework.common.schema.id_schema_object import IdSchemaObject
 from superlinked.framework.common.schema.schema import T
+from superlinked.framework.common.schema.schema_object import SchemaObject
+from superlinked.framework.common.storage_manager.header import Header
+from superlinked.framework.common.storage_manager.storage_manager import ResultTypeT
 from superlinked.framework.dsl.executor.in_memory.in_memory_executor import InMemoryApp
 from superlinked.framework.dsl.index.index import Index
-from superlinked.framework.storage.entity import Entity, EntityId
+from superlinked.framework.storage.in_memory.in_memory_vdb import InMemoryVDB
 
 
 class VectorNotFoundError(Exception):
     pass
 
 
 class VectorCollection:
@@ -34,22 +38,22 @@
     the object of which `self.vectors[i]` is the embedded vector.
 
     Attributes:
         id_list (list[str]): List of object ids.
         vectors (npt.NDArray[np.float64]): Numpy array of
     """
 
-    def __init__(self, id_list: list[str], vectors: npt.NDArray[np.float64]) -> None:
+    def __init__(self, id_list: Sequence[str], vectors: NPArray) -> None:
         if (len(id_list) > 1) & (len(id_list) != vectors.shape[0]):
             raise ValueError(
                 f"id_list length and vectors parameter shape's first dimension should match. "
                 f"Got {id_list=} and {vectors.shape[0]=}"
             )
-        self.id_list: list[str] = id_list
-        self.vectors: npt.NDArray[np.float64] = vectors
+        self.id_list: Sequence[str] = id_list
+        self.vectors: NPArray = vectors
 
     def __len__(self) -> int:
         return len(self.id_list)
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, VectorCollection):
             return (self.id_list == other.id_list) & np.allclose(
@@ -127,24 +131,23 @@
             )
         if len(ids) != len(readable_ids):
             raise ValueError(
                 f"id_ and readable_id_ should have the same length. "
                 f"Got {len(ids)} and {len(readable_ids)}"
             )
 
-        entity_vectors: list[npt.NDArray[np.float64]] = []
+        entity_vectors: list[NPArray] = []
         entity_ids: list[str] = []
         for identification, readable_id in zip(ids, readable_ids):
-            user_entity_id = EntityId(
-                identification, index._node.node_id, schema._base_class_name
+            vector = self.__app.storage_manager.read_node_result(
+                schema, identification, index._node.node_id, index._node.node_data_type
             )
-            vector = self.__app.entity_store_manager.get_vector(user_entity_id)
             if vector is None:
                 raise VectorNotFoundError(
-                    f"No vector found for entity id {user_entity_id} in the given index and schema."
+                    f"No vector found for {schema._schema_name} with id {identification} in the given index."
                 )
 
             entity_vectors.append(vector.value)
             entity_ids.append(readable_id)
 
         return VectorCollection(entity_ids, np.array(entity_vectors))
 
@@ -164,44 +167,63 @@
             VectorCollection: All vectors for each corresponding entity to the given index and schema and a list of
                 ids. Position `i` in the id list correspond to row `i` in the vector array.
 
         Raises:
             VectorNotFoundError: If no vector is found for any entities.
         """
         schema = cast(IdSchemaObject, schema)
-        entities = self.__app.entity_store_manager.get_entities(
-            index._node.node_id, schema._schema_name
+        headers = self._read_node_results(
+            schema, index._node.node_id, index._node.node_data_type
         )
         if include_chunks:
-            entity_ids: list[str] = [entity.id_.object_id for entity in entities]
+            entity_ids: list[str] = [header.object_id for header in headers]
             readable_ids: list[str] = [
-                self.human_readable_id_for_chunks(entity) for entity in entities
+                self.human_readable_id_for_chunks(header) for header in headers
             ]
             return self.get_vectors_by_ids(entity_ids, index, schema, readable_ids)
 
         entity_ids = list(
             {
-                self.get_id_for_standalone_entity_origin_id_for_chunk(entity)
-                for entity in entities
+                self.__get_id_for_standalone_entity_origin_id_for_chunk(header)
+                for header in headers
             }
         )
         return self.get_vectors_by_ids(entity_ids, index, schema)
 
+    def _read_node_results(
+        self, schema: SchemaObject, node_id: str, result_type: type[ResultTypeT]
+    ) -> Sequence[Header]:
+        entity_builder = self.__app.storage_manager._entity_builder
+        in_memory_vdb = cast(InMemoryVDB, self.__app.storage_manager._vdb_connector)
+
+        schema_filter = (
+            entity_builder._admin_fields.schema_id.field == schema._schema_name
+        )
+        result_field = entity_builder.compose_field(node_id, result_type)
+        returned_fields = entity_builder._admin_fields.header_fields
+        entity_data = in_memory_vdb.read_entities_matching_filters(
+            [schema_filter], [result_field], returned_fields
+        )
+        return [
+            entity_builder._admin_fields.extract_header(ed.field_data)
+            for ed in entity_data
+        ]
+
     @staticmethod
-    def get_id_for_standalone_entity_origin_id_for_chunk(entity: Entity) -> str:
-        if entity.is_chunk():
-            origin_id = cast(EntityId, entity.origin_id)
-            return origin_id.object_id
-        return entity.id_.object_id
+    def __get_id_for_standalone_entity_origin_id_for_chunk(
+        header: Header,
+    ) -> str:
+        if header.origin_id is not None:
+            return header.origin_id
+        return header.object_id
 
     @staticmethod
-    def human_readable_id_for_chunks(entity: Entity) -> str:
-        if entity.is_chunk():
-            origin_id = cast(EntityId, entity.origin_id)
-            return f"{origin_id.object_id}-{entity.id_.object_id}"
-        return entity.id_.object_id
+    def human_readable_id_for_chunks(header: Header) -> str:
+        if header.origin_id is not None:
+            return f"{header.origin_id}-{header.object_id}"
+        return header.object_id
 
     def __str__(self) -> str:
         return f"VectorSampler on app: {print(self.__app)}"
 
     def __repr__(self) -> str:
         return self.__str__()
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/calculation/distance_metric.py` & `superlinked-5.2.2/superlinked/framework/common/calculation/distance_metric.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/calculation/vector_similarity.py` & `superlinked-5.2.2/superlinked/framework/common/calculation/vector_similarity.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,34 +9,28 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import numpy as np
-import numpy.typing as npt
 
 from superlinked.framework.common.calculation.distance_metric import DistanceMetric
-from superlinked.framework.common.data_types import Vector
+from superlinked.framework.common.data_types import NPArray, Vector
 
 
 class VectorSimilarityCalculator:
-
     def __init__(self, method: DistanceMetric) -> None:
         self.__method = method
 
     def calculate_similarity(self, vector_a: Vector, vector_b: Vector) -> float:
         return self.calculate_similarity_np(vector_a.value, vector_b.value)
 
-    def calculate_similarity_np(
-        self, vector_a: npt.NDArray[np.float64], vector_b: npt.NDArray[np.float64]
-    ) -> float:
+    def calculate_similarity_np(self, vector_a: NPArray, vector_b: NPArray) -> float:
         match self.__method:
             case DistanceMetric.INNER_PRODUCT:
                 return self.__calculate_inner_product(vector_a, vector_b)
             case _:
                 raise ValueError(f"Unsupported calculation method: {self.__method}")
 
-    def __calculate_inner_product(
-        self, vector_a: npt.NDArray[np.float64], vector_b: npt.NDArray[np.float64]
-    ) -> float:
+    def __calculate_inner_product(self, vector_a: NPArray, vector_b: NPArray) -> float:
         return np.inner(vector_a, vector_b)
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/const.py` & `superlinked-5.2.2/superlinked/framework/common/const.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/aggregation_node.py` & `superlinked-5.2.2/superlinked/framework/common/dag/aggregation_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 class AggregationNode(Node[Vector], HasLength):
     def __init__(
         self,
         weighted_parents: list[Weighted[Node[Vector]]],
         dag_effects: set[DagEffect],
     ) -> None:
         super().__init__(
+            Vector,
             [weighted_parent.item for weighted_parent in weighted_parents],
             persistence_params=PersistenceParams(persist_parent_evaluation_result=True),
             dag_effects=dag_effects,
         )
         self.__validate_parents()
         self.weighted_parents = weighted_parents
         # All parents are of the same length as it was validated earlier.
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/categorical_similarity_node.py` & `superlinked-5.2.2/superlinked/framework/common/dag/categorical_similarity_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 class CategoricalSimilarityNode(Node[Vector], HasLength, HasAggregation):
     def __init__(
         self,
         parent: Node[str],
         categorical_similarity_param: CategoricalSimilarityParams,
     ) -> None:
-        super().__init__([parent])
+        super().__init__(Vector, [parent])
         self.__aggregation = VectorAggregation(L2Norm())
         self.embedding = CategoricalSimilarityEmbedding(
             categorical_similarity_param=categorical_similarity_param,
             normalization=self.__aggregation.normalization,
         )
 
     @property
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/chunking_node.py` & `superlinked-5.2.2/superlinked/framework/common/dag/chunking_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self,
         parent: Node[str],
         chunk_size: int | None = None,
         chunk_overlap: int | None = None,
         split_chars_keep: list[str] | None = None,
         split_chars_remove: list[str] | None = None,
     ) -> None:
-        super().__init__([parent])
+        super().__init__(str, [parent])
         self.chunk_size = chunk_size
         self.chunk_overlap = chunk_overlap
         self.split_chars_keep = split_chars_keep
         self.split_chars_remove = split_chars_remove
 
     @override
     def _get_node_id_parameters(self) -> dict[str, Any]:
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/comparison_filter_node.py` & `superlinked-5.2.2/superlinked/framework/common/dag/comparison_filter_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         comparison_operation: ComparisonOperation[SchemaField],
         dag_effects: set[DagEffect] | None = None,
     ) -> None:
         if parent.schema_field != comparison_operation._operand:
             raise InitializationException(
                 f"{self.class_name}'s parent and operand must be the same."
             )
-        super().__init__([parent])
+        super().__init__(bool, [parent])
         if dag_effects is not None:
             self.dag_effects = dag_effects
         self.comparison_operation = comparison_operation
 
     @property
     @override
     def persist_evaluation_result(self) -> bool:
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/concatenation_node.py` & `superlinked-5.2.2/superlinked/framework/common/dag/concatenation_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         self,
         parents: list[Node[Vector]],
         default_weight: float = DEFAULT_WEIGHT,
     ) -> None:
         # Since events can change only a part of the whole result, we
         # must persist the rest of the parts.
         super().__init__(
+            Vector,
             parents,
             persistence_params=PersistenceParams(persist_parent_evaluation_result=True),
         )
         self.__validate_parents()
         self.default_weight = default_weight
         self.__length = sum(cast(HasLength, parent).length for parent in self.parents)
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/constant_node.py` & `superlinked-5.2.2/superlinked/framework/common/dag/constant_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,13 +18,13 @@
 
 from superlinked.framework.common.dag.node import NDT, Node
 from superlinked.framework.common.schema.schema_object import SchemaObject
 
 
 class ConstantNode(Node[NDT]):
     def __init__(self, value: NDT, schema: SchemaObject) -> None:
-        super().__init__([], schemas={schema})
+        super().__init__(type(value), [], schemas={schema})
         self.value = value
 
     @override
     def _get_node_id_parameters(self) -> dict[str, Any]:
         return {"schemas": self.schemas, "value": str(self.value)}
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/context.py` & `superlinked-5.2.2/superlinked/framework/common/dag/context.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/custom_node.py` & `superlinked-5.2.2/superlinked/framework/common/dag/custom_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 class CustomVectorEmbeddingNode(Node[Vector], HasLength, HasAggregation):
     def __init__(
         self,
         parent: Node[Vector],
         length: int,
         aggregation: Aggregation,
     ) -> None:
-        super().__init__([parent])
+        super().__init__(Vector, [parent])
         self.__aggregation = aggregation
         self.embedding = CustomEmbedding(
             length=length, normalization=self.__aggregation.normalization
         )
 
     @property
     def length(self) -> int:
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/dag.py` & `superlinked-5.2.2/superlinked/framework/common/dag/dag.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/dag_effect.py` & `superlinked-5.2.2/superlinked/framework/common/dag/dag_effect.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/event_aggregation_node.py` & `superlinked-5.2.2/superlinked/framework/common/dag/event_aggregation_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,26 +29,27 @@
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.interface.weighted import Weighted
 from superlinked.framework.common.schema.event_schema_object import EventSchemaObject
 from superlinked.framework.common.schema.schema_object import SchemaObject
 
 
-class EventAggregationNode(Node[str], HasLength):
+class EventAggregationNode(Node[Vector], HasLength):
     @dataclass
     class InitParams:
         input_to_aggregate: Node[Vector]
         event_schema: EventSchemaObject
         affected_schema: SchemaObjectReference
         affecting_schema: SchemaObjectReference
         filter_inputs: list[Weighted[ComparisonFilterNode]]
         dag_effects: list[DagEffect]
 
     def __init__(self, init_params: InitParams) -> None:
         super().__init__(
+            Vector,
             [init_params.input_to_aggregate]
             + [filter.item for filter in init_params.filter_inputs],
             dag_effects=set(init_params.dag_effects),
             persistence_params=PersistenceParams(
                 persist_evaluation_result=True, persist_parent_evaluation_result=True
             ),
         )
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/exception.py` & `superlinked-5.2.2/superlinked/framework/common/dag/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/index_node.py` & `superlinked-5.2.2/superlinked/framework/common/dag/index_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 class IndexNode(Node[Vector], HasLength):
     def __init__(
         self,
         parents: set[Node[Vector]],
     ) -> None:
         super().__init__(
+            Vector,
             self.__validate_and_order_parents(parents),
             persistence_params=PersistenceParams(
                 persist_evaluation_result=True, persistence_type=PersistenceType.VECTOR
             ),
         )
         self.__length = cast(HasLength, self.parents[0]).length
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/named_function_node.py` & `superlinked-5.2.2/superlinked/framework/common/dag/named_function_node.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 class NamedFunctionNode(Node[NDT]):
     def __init__(
         self,
         named_function: NamedFunction,
         schema: SchemaObject,
         return_type: type[NDT],
     ) -> None:
-        super().__init__([], schemas={schema})
+        super().__init__(return_type, [], schemas={schema})
         self.named_function = named_function
         self.return_type = return_type
 
     @override
     def _get_node_id_parameters(self) -> dict[str, Any]:
         return {
             "schemas": self.schemas,
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/node.py` & `superlinked-5.2.2/superlinked/framework/common/dag/node.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,20 +16,21 @@
 
 import hashlib
 from abc import ABC, abstractmethod
 from typing import Any, Generic, TypeVar
 
 from superlinked.framework.common.dag.dag_effect import DagEffect
 from superlinked.framework.common.dag.persistence_params import PersistenceParams
+from superlinked.framework.common.data_types import PythonTypes
 from superlinked.framework.common.schema.schema_object import SchemaObject
 from superlinked.framework.common.storage.persistence_type import PersistenceType
 from superlinked.framework.common.util.string_util import StringUtil
 
 # NodeDataType
-NDT = TypeVar("NDT")
+NDT = TypeVar("NDT", bound=PythonTypes)
 # NodeType
 NT = TypeVar("NT", bound="Node")
 
 
 class Node(Generic[NDT], ABC):
     _instances: dict[str, Node] = {}
 
@@ -41,19 +42,21 @@
             instance = cls._instances[node_id]
         else:
             cls._instances[node_id] = instance
         return instance
 
     def __init__(
         self,
+        node_data_type: type[NDT],
         parents: list[Node],
         schemas: set[SchemaObject] | None = None,
         dag_effects: set[DagEffect] | None = None,
         persistence_params: PersistenceParams | None = None,
     ) -> None:
+        self._node_data_type = node_data_type
         self._node_id: str | None = None
         self.children: list[Node] = []
         self.parents = parents
         self.schemas: set[SchemaObject] = (schemas or set()).union(
             {schema for parent in parents for schema in parent.schemas}
             if parents
             else set()
@@ -70,14 +73,18 @@
     def _append_child(self, child: Node) -> None:
         self.children.append(child)
         self._persistence_params.persist_evaluation_result |= (
             child._persistence_params.persist_parent_evaluation_result
         )
 
     @property
+    def node_data_type(self) -> type[NDT]:
+        return self._node_data_type
+
+    @property
     def node_id(self) -> str:
         if not self._node_id:
             self._node_id = self._generate_node_id()
         return self._node_id
 
     @property
     def is_root(self) -> bool:
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/number_embedding_node.py` & `superlinked-5.2.2/superlinked/framework/common/dag/number_embedding_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 class NumberEmbeddingNode(Node[Vector], HasLength, HasAggregation):
     def __init__(
         self,
         parent: Node[float | int],
         embedding_params: NumberEmbeddingParams,
     ) -> None:
-        super().__init__([parent])
+        super().__init__(Vector, [parent])
         self.__aggregation = VectorAvg(NoNorm())
         self.embedding = NumberEmbedding(
             embedding_params.min_value,
             embedding_params.max_value,
             embedding_params.mode,
             embedding_params.negative_filter,
             self.__aggregation.normalization,
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/number_similarity_node.py` & `superlinked-5.2.2/superlinked/framework/common/dag/number_similarity_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         self,
         parent: Node[float | int],
         min_value: float,
         max_value: float,
         negative_filter: float,
         aggregation_mode: InputAggregationMode,
     ) -> None:
-        super().__init__([parent])
+        super().__init__(Vector, [parent])
         normalization = NoNorm()
         self.embedding = NumberSimilarityEmbedding(
             min_value,
             max_value,
             negative_filter,
             normalization,
         )
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/period_time.py` & `superlinked-5.2.2/superlinked/framework/common/dag/period_time.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/persistence_params.py` & `superlinked-5.2.2/superlinked/framework/common/dag/persistence_params.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/recency_node.py` & `superlinked-5.2.2/superlinked/framework/common/dag/recency_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         self,
         parent: Node[int],
         time_period_hour_offset: timedelta,
         period_time_list: list[PeriodTime],
         aggregation_mode: InputAggregationMode,
         negative_filter: float,
     ) -> None:
-        super().__init__([parent])
+        super().__init__(Vector, [parent])
         normalization = calculate_recency_normalization(period_time_list)
         self.embedding = RecencyEmbedding(
             period_time_list,
             normalization,
             time_period_hour_offset,
             negative_filter,
         )
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/resolved_schema_reference.py` & `superlinked-5.2.2/superlinked/framework/common/dag/resolved_schema_reference.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/schema_dag.py` & `superlinked-5.2.2/superlinked/framework/common/dag/schema_dag.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/schema_field_node.py` & `superlinked-5.2.2/superlinked/framework/common/dag/schema_field_node.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,20 @@
 from superlinked.framework.common.schema.schema_object import SFT, SchemaField
 
 
 class SchemaFieldNode(Generic[SFT], Node[SFT]):
     def __init__(
         self, schema_field: SchemaField[SFT], dag_effects: set[DagEffect] | None = None
     ) -> None:
-        super().__init__([], schemas={schema_field.schema_obj}, dag_effects=dag_effects)
+        super().__init__(
+            schema_field.type_,
+            [],
+            schemas={schema_field.schema_obj},
+            dag_effects=dag_effects,
+        )
         self.schema_field = schema_field
 
     @override
     def _get_node_id_parameters(self) -> dict[str, Any]:
         return {
             "schema_field": self.schema_field,
             "schemas": self.schemas,
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/schema_object_reference.py` & `superlinked-5.2.2/superlinked/framework/common/dag/schema_object_reference.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/dag/text_embedding_node.py` & `superlinked-5.2.2/superlinked/framework/common/dag/text_embedding_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,19 +32,18 @@
 
 class TextEmbeddingNode(Node[Vector], HasLength, HasAggregation):
     def __init__(
         self,
         parent: Node[str],
         model_name: str,
     ) -> None:
-        super().__init__([parent])
+        super().__init__(Vector, [parent])
         self.model_name = model_name
         self.__aggregation = VectorAggregation(L2Norm())
         self.post_init()
-        super().__init__([parent])
 
     def post_init(self) -> None:
         self.embedding = SentenceTransformerEmbedding(
             self.model_name, self.__aggregation.normalization
         )
 
     @property
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/data_types.py` & `superlinked-5.2.2/superlinked/framework/common/data_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,38 +14,38 @@
 
 from __future__ import annotations
 
 from collections.abc import Mapping
 from typing import Any, Union
 
 import numpy as np
-import numpy.typing as npt
 
 from superlinked.framework.common.exception import (
     MismatchingDimensionException,
     NegativeFilterException,
 )
 
 Json = Mapping[str, Any]
+NPArray = np.ndarray[Any, np.dtype[np.float64]]
 
 
 class Vector:
     EMPTY_VECTOR: Vector | None = None
 
     def __init__(
         self,
-        value: Union[list[float], npt.NDArray[np.float64]],
+        value: Union[list[float], NPArray],
         negative_filter_indices: set[int] | None = None,
         vector_before_normalization: Vector | None = None,
     ) -> None:
         if isinstance(value, np.ndarray):
             value_to_set = value
         else:
             value_to_set = np.array(value, dtype=float)
-        self.value: npt.NDArray[np.float64] = value_to_set
+        self.value: NPArray = value_to_set
         self.__dimension: int = len(self.value)
         self.__negative_filter_indices = negative_filter_indices or set()
         self.__validate_negative_filter_indices()
         self.__vector_before_normalization = vector_before_normalization
 
     @property
     def dimension(self) -> int:
@@ -192,15 +192,15 @@
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, Vector):
             return np.array_equal(self.value, other.value)
         return False
 
     def copy_with_new(
         self,
-        value: list[float] | npt.NDArray[np.float64] | None = None,
+        value: list[float] | NPArray | None = None,
         negative_filter_indices: set[int] | None = None,
         vector_before_normalization: Vector | None = None,
     ) -> Vector:
         value_to_use = self.value if value is None else value
         vector_before_normalization_to_use = (
             (
                 self.vector_before_normalization.copy_with_new()
@@ -221,7 +221,10 @@
             vector_before_normalization_to_use,
         )
 
     def __copy(self) -> Vector:
         if self.is_empty:
             return self
         return self.copy_with_new()
+
+
+PythonTypes = float | int | str | Vector | NPArray
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/embedding/categorical_similarity_embedding.py` & `superlinked-5.2.2/superlinked/framework/common/embedding/categorical_similarity_embedding.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import numpy as np
-import numpy.typing as npt
 from typing_extensions import override
 
 from superlinked.framework.common.dag.context import ExecutionContext
-from superlinked.framework.common.data_types import Vector
+from superlinked.framework.common.data_types import NPArray, Vector
 from superlinked.framework.common.embedding.embedding import Embedding
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.space.normalization import Normalization
 
 CATEGORICAL_ENCODING_VALUE: int = 1
 
 
@@ -62,23 +61,21 @@
             else None
         )
 
     @override
     def embed(self, input_: str, context: ExecutionContext) -> Vector:
         # TODO: https://linear.app/superlinked/issue/ENG-1736/make-schemafields-composite
         parsed_input: list[str] = self.__parse_categories(input_=input_)
-        one_hot_encoding: npt.NDArray[np.float64] = self.__n_hot_encode(
+        one_hot_encoding: NPArray = self.__n_hot_encode(
             parsed_input, context.is_query_context()
         )
         return Vector(one_hot_encoding)
 
-    def __n_hot_encode(
-        self, category_list: list[str], is_query: bool
-    ) -> npt.NDArray[np.float64]:
-        n_hot_encoding: npt.NDArray[np.float64] = np.full(
+    def __n_hot_encode(self, category_list: list[str], is_query: bool) -> NPArray:
+        n_hot_encoding: NPArray = np.full(
             self.__length,
             0 if is_query else self.categorical_similarity_param.negative_filter,
             dtype=np.float32,
         )
         category_indices: list[int] = self.__get_category_indices(category_list)
         if category_indices:
             n_hot_encoding[category_indices] = self.__get_normalized_vector_input()
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/embedding/chunking_util.py` & `superlinked-5.2.2/superlinked/framework/common/embedding/chunking_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/embedding/custom_embedding.py` & `superlinked-5.2.2/superlinked/framework/common/embedding/custom_embedding.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import numpy as np
-import numpy.typing as npt
 from typing_extensions import override
 
 from superlinked.framework.common.dag.context import ExecutionContext
-from superlinked.framework.common.data_types import Vector
+from superlinked.framework.common.data_types import NPArray, Vector
 from superlinked.framework.common.embedding.embedding import Embedding
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.space.normalization import Normalization
 
 
-class CustomEmbedding(Embedding[npt.NDArray[np.float64]], HasLength):
+class CustomEmbedding(Embedding[NPArray], HasLength):
     def __init__(self, length: int, normalization: Normalization) -> None:
         self.__length: int = length
         self._normalization: Normalization = normalization
 
     @override
     def embed(
         self,
-        input_: npt.NDArray[np.float64],
+        input_: NPArray,
         context: ExecutionContext,  # pylint: disable=unused-argument
     ) -> Vector:
         return Vector(input_).normalize(self._normalization.norm(input_))
 
     @property
     def length(self) -> int:
         return self.__length
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/embedding/embedding.py` & `superlinked-5.2.2/superlinked/framework/common/embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/embedding/number_embedding.py` & `superlinked-5.2.2/superlinked/framework/common/embedding/number_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/embedding/number_similarity_embedding.py` & `superlinked-5.2.2/superlinked/framework/common/embedding/number_similarity_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/embedding/recency_embedding.py` & `superlinked-5.2.2/superlinked/framework/common/embedding/recency_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/embedding/sentence_transformer_embedding.py` & `superlinked-5.2.2/superlinked/framework/common/embedding/sentence_transformer_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/exception.py` & `superlinked-5.2.2/superlinked/framework/common/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/interface/comparison_operand.py` & `superlinked-5.2.2/superlinked/framework/common/interface/comparison_operand.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/interface/comparison_operation_type.py` & `superlinked-5.2.2/superlinked/framework/common/interface/comparison_operation_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/interface/has_aggregation.py` & `superlinked-5.2.2/superlinked/framework/common/interface/has_aggregation.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/interface/has_length.py` & `superlinked-5.2.2/superlinked/framework/common/interface/has_length.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/interface/has_multiplier.py` & `superlinked-5.2.2/superlinked/framework/common/interface/has_multiplier.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/interface/weighted.py` & `superlinked-5.2.2/superlinked/framework/common/interface/weighted.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/observable.py` & `superlinked-5.2.2/superlinked/framework/common/observable.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/parser/data_parser.py` & `superlinked-5.2.2/superlinked/framework/common/parser/data_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,18 +126,16 @@
         """
         if not isinstance(parsed_schemas, list):
             parsed_schemas = [parsed_schemas]
         self.__check_parsed_schemas(parsed_schemas)
         return self._marshal(parsed_schemas)
 
     def __validate_mapping_against_schema(
-        self, schema: IdSchemaObjectT, mapping: Mapping[SchemaField, str] | None
+        self, schema: IdSchemaObjectT, mapping: Mapping[SchemaField, str]
     ) -> None:
-        if not mapping:
-            return
         schema_fields = list(schema._get_schema_fields()) + [schema.id]
         if invalid_keys := [key for key in mapping.keys() if key not in schema_fields]:
             invalid_key_names = [
                 f"{key.schema_obj._base_class_name}.{key.name}" for key in invalid_keys
             ]
             raise InvalidMappingException(
                 f"{invalid_key_names} don't belong to the {schema._base_class_name} schema."
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/parser/dataframe_parser.py` & `superlinked-5.2.2/superlinked/framework/common/parser/dataframe_parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from collections.abc import Mapping
-from typing import Any, Generic
+from typing import Generic
 
 import pandas as pd
 
 from superlinked.framework.common.parser.data_parser import DataParser
 from superlinked.framework.common.parser.exception import (
     DuplicateIdException,
     MissingIdException,
@@ -28,14 +28,15 @@
     ParsedSchema,
     ParsedSchemaField,
 )
 from superlinked.framework.common.schema.id_schema_object import (
     IdSchemaObjectT,
     SchemaField,
 )
+from superlinked.framework.common.schema.schema_reference import SchemaReference
 
 
 class DataFrameParser(
     Generic[IdSchemaObjectT], DataParser[IdSchemaObjectT, pd.DataFrame]
 ):
     """
     DataFrameParser gets a `pd.DataFrame` and using column-string mapping
@@ -44,92 +45,105 @@
 
     def __init__(
         self, schema: IdSchemaObjectT, mapping: Mapping[SchemaField, str] | None = None
     ) -> None:
         super().__init__(schema, mapping)
         self._id_name = self.mapping.get(self._schema.id, self._schema.id.name)
 
-    def _get_column_name_to_schema_field_mapping(self) -> dict[str, SchemaField]:
-        reverse_mapping: dict[str, SchemaField] = {
-            self.mapping.get(field, field.name) if self.mapping else field.name: field
-            for field in list(self._schema._get_schema_fields()) + [self._schema.id]
-        }
-        return reverse_mapping
-
     def unmarshal(self, data: pd.DataFrame) -> list[ParsedSchema]:
         """
         Parses the given DataFrame into a list of ParsedSchema objects according to the defined schema and mapping.
-
         Args:
             data (pd.DataFrame): Pandas DataFrame input.
-
         Returns:
             list[ParsedSchema]: A list of ParsedSchema objects that will be processed by the spaces.
         """
+        data_copy = data.copy()
         schema_cols: dict[str, SchemaField] = (
             self._get_column_name_to_schema_field_mapping()
         )
 
-        self._ensure_id(data)
+        self._ensure_id(data_copy)
+        data_copy[self._id_name] = data_copy[self._id_name].astype(str)
+        schema_ref_cols = [
+            key
+            for key, value in schema_cols.items()
+            if isinstance(value, SchemaReference)
+        ]
+        data_copy[schema_ref_cols] = data_copy[schema_ref_cols].astype(str)
 
-        records: list[dict[str, Any]] = data.loc[:, list(schema_cols.keys())].to_dict(
-            orient="records"
-        )
-        return [
+        records = data_copy[list(schema_cols.keys())].to_dict(orient="records")
+
+        parsed_schemas = [
             ParsedSchema(
                 self._schema,
                 record[self._id_name],
                 [
                     ParsedSchemaField.from_schema_field(
                         schema_field=schema_cols[key], value=value
                     )
                     for key, value in record.items()
                     if key != self._id_name and not pd.isnull(value)
                 ],
             )
             for record in records
         ]
 
+        return parsed_schemas
+
     def _marshal(
         self,
         parsed_schemas: list[ParsedSchema],
     ) -> list[pd.DataFrame]:
         """
         Converts a list of ParsedSchema objects into a list of pandas DataFrame.
         You can use this functionality to check, if your mapping was defined properly.
-
         Args:
             parsed_schemas (list[ParsedSchema]): A list of ParsedSchema objects that you get
                 after unmarshaling your `DataFrame`.
-
         Returns:
             list[pd.DataFrame]: A list of DataFrame representation of the parsed schemas.
         """
-
         records = [
             {
                 **{self._id_name: parsed_schema.id_},
                 **{
                     field.schema_field.name: field.value
                     for field in parsed_schema.fields
                 },
             }
             for parsed_schema in parsed_schemas
         ]
-        return [pd.DataFrame(records)]
+        return [pd.DataFrame.from_records(records)]  # type: ignore[attr-defined]
+
+    def _get_column_name_to_schema_field_mapping(self) -> dict[str, SchemaField]:
+        return {
+            self.mapping.get(field, field.name): field
+            for field in list(self._schema._get_schema_fields()) + [self._schema.id]
+        }
 
     def _ensure_id(self, data: pd.DataFrame) -> None:
         if self._id_name not in data.columns:
             raise KeyError(
                 f"No {self._id_name} column in supplied dataframe. Create a unique id column with the specified name."
             )
-        ids: pd.Series = data[self._id_name]
-        if any(not self._is_id_value_valid(id_val) for id_val in ids.tolist()):
+
+        if self._has_missing_ids(data):
             raise MissingIdException(
                 "The mandatory id field has missing values in the input object."
             )
-        vc_ids = ids.value_counts()
-        if vc_ids.max() > 1:
-            duplicate_ids = vc_ids[vc_ids > 1].index.tolist()
+
+        if duplicate_ids := self._find_duplicate_ids(data):
             raise DuplicateIdException(
                 f"Multiple rows have the same id: {', '.join([str(f) for f in duplicate_ids])}"
             )
+
+    def _has_missing_ids(self, data: pd.DataFrame) -> bool:
+        return any(
+            not self._is_id_value_valid(id_val)
+            for id_val in data[self._id_name].tolist()
+        )
+
+    def _find_duplicate_ids(self, data: pd.DataFrame) -> list[str]:
+        mask = data[self._id_name]
+        duplicate_mask = mask.duplicated()
+        return mask[duplicate_mask].unique().tolist()
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/parser/exception.py` & `superlinked-5.2.2/superlinked/framework/common/parser/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/parser/json_parser.py` & `superlinked-5.2.2/superlinked/framework/common/parser/json_parser.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from typing import Generic, cast
+from typing import Generic
 
 from superlinked.framework.common.data_types import Json
 from superlinked.framework.common.parser.data_parser import DataParser
 from superlinked.framework.common.parser.exception import MissingIdException
 from superlinked.framework.common.parser.parsed_schema import (
     ParsedSchema,
     ParsedSchemaField,
 )
 from superlinked.framework.common.schema.id_schema_object import IdSchemaObjectT
 from superlinked.framework.common.schema.schema_object import SFT, SchemaField
+from superlinked.framework.common.schema.schema_reference import SchemaReference
 from superlinked.framework.common.util.dot_separated_path_util import (
     DotSeparatedPathUtil,
     ValuedDotSeparatedPath,
 )
 
 
 class JsonParser(Generic[IdSchemaObjectT], DataParser[IdSchemaObjectT, Json]):
@@ -95,21 +96,24 @@
 
     def __ensure_id(self, data: Json) -> str:
         id_ = self._parse_schema_field_value(self._schema.id, data)
         if not self._is_id_value_valid(id_):
             raise MissingIdException(
                 "The mandatory id field is missing from the input object."
             )
-        return cast(str, id_)
+        return str(id_)
 
     def _parse_schema_field_value(
         self, field: SchemaField[SFT], data: Json
     ) -> SFT | None:
         path: str = self.__get_path(field)
-        return DotSeparatedPathUtil.get(data, path)
+        parsed_schema_field_value = DotSeparatedPathUtil.get(data, path)
+        if isinstance(field, SchemaReference):
+            parsed_schema_field_value = str(parsed_schema_field_value)
+        return parsed_schema_field_value
 
     def __get_path(self, field: SchemaField[SFT]) -> str:
         return self.mapping.get(field, field.name)
 
     def __get_all_fields_from_parsed_schema(
         self, parsed_schema: ParsedSchema
     ) -> list[ParsedSchemaField]:
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/parser/parsed_schema.py` & `superlinked-5.2.2/superlinked/framework/common/parser/parsed_schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/schema/event_schema.py` & `superlinked-5.2.2/superlinked/framework/common/schema/event_schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/schema/event_schema_object.py` & `superlinked-5.2.2/superlinked/framework/common/schema/event_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/schema/exception.py` & `superlinked-5.2.2/superlinked/framework/common/schema/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/schema/general_type.py` & `superlinked-5.2.2/superlinked/framework/common/schema/general_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/schema/id_schema_object.py` & `superlinked-5.2.2/superlinked/framework/common/schema/id_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/schema/schema.py` & `superlinked-5.2.2/superlinked/framework/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/schema/schema_decorator.py` & `superlinked-5.2.2/superlinked/framework/common/schema/schema_decorator.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/schema/schema_factory.py` & `superlinked-5.2.2/superlinked/framework/common/schema/schema_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from superlinked.framework.common.schema.schema_object import (
     ConcreteSchemaField,
     SchemaFieldDescriptor,
 )
 from superlinked.framework.common.schema.schema_reference import SchemaReference
 from superlinked.framework.common.schema.schema_type import SchemaType
 from superlinked.framework.common.schema.schema_validator import SchemaValidator
-from superlinked.framework.common.util.schema_util import SchemaUtil
+from superlinked.framework.common.util.generic_class_util import GenericClassUtil
 
 
 class SchemaFactory:
     def __init__(self) -> None:
         self.__schema_validators = {
             SchemaType.SCHEMA: SchemaValidator(SchemaType.SCHEMA),
             SchemaType.EVENT_SCHEMA: SchemaValidator(SchemaType.EVENT_SCHEMA),
@@ -45,15 +45,15 @@
         schema_validator = self.__schema_validators[schema_type]
         schema_validator.check_class_attributes(cls)
         schema_validator.check_unannotated_members(cls)
         schema_name: str = cls.__name__
         schema_field_descriptors = list[SchemaFieldDescriptor]()
         for name, type_ in cls.__annotations__.items():
             type_args = get_args(type_)
-            type_ = SchemaUtil.if_not_class_get_origin(type_)
+            type_ = GenericClassUtil.if_not_class_get_origin(type_)
             if not type_:
                 continue
             if issubclass(
                 type_,
                 get_args(self.__schema_field_types[schema_type]),
             ):
                 schema_field_descriptors.append(
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/schema/schema_object.py` & `superlinked-5.2.2/superlinked/framework/common/schema/schema_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,29 +13,28 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Any, Generic, TypeVar
 
-import numpy as np
-import numpy.typing as npt
 from beartype.typing import Sequence
 
+from superlinked.framework.common.data_types import NPArray, PythonTypes
 from superlinked.framework.common.interface.comparison_operand import ComparisonOperand
 
 # Exclude from documentation.
 # A better approach would be to separate this file into atomic objects,
 # which is blocked due to circular dependency issues.
 __pdoc__ = {}
 __pdoc__["SchemaFieldDescriptor"] = False
 
 
 # SchemaFieldType
-SFT = TypeVar("SFT")
+SFT = TypeVar("SFT", bound=PythonTypes)
 SchemaObjectT = TypeVar("SchemaObjectT", bound="SchemaObject")
 
 
 class SchemaObject:
     """
     `@schema` decorated class that has multiple `SchemaField`s.
 
@@ -165,21 +164,21 @@
     Field of a schema that represents an integer.
     """
 
     def __init__(self, name: str, schema_obj: SchemaObjectT) -> None:
         super().__init__(name, schema_obj, int)
 
 
-class Array(SchemaField[npt.NDArray[np.float64]]):
+class Array(SchemaField[NPArray]):
     """
     Field of a schema that represents a vector.
     """
 
     def __init__(self, name: str, schema_obj: SchemaObjectT) -> None:
-        super().__init__(name, schema_obj, npt.NDArray[np.float64])
+        super().__init__(name, schema_obj, NPArray)
 
 
 ConcreteSchemaField = String | Timestamp | Float | Integer | Array
 ConcreteSchemaFieldT = TypeVar("ConcreteSchemaFieldT", bound="ConcreteSchemaField")
 
 
 @dataclass
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/schema/schema_reference.py` & `superlinked-5.2.2/superlinked/framework/common/schema/schema_reference.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/schema/schema_type.py` & `superlinked-5.2.2/superlinked/framework/common/schema/schema_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/schema/schema_validator.py` & `superlinked-5.2.2/superlinked/framework/common/schema/schema_validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,29 +21,29 @@
     InvalidMemberException,
 )
 from superlinked.framework.common.schema.general_type import T
 from superlinked.framework.common.schema.id_schema_object import IdField
 from superlinked.framework.common.schema.schema_object import ConcreteSchemaField
 from superlinked.framework.common.schema.schema_reference import SchemaReference
 from superlinked.framework.common.schema.schema_type import SchemaType
-from superlinked.framework.common.util.schema_util import SchemaUtil
+from superlinked.framework.common.util.generic_class_util import GenericClassUtil
 
 valid_schema_field_types = {
     SchemaType.SCHEMA: ConcreteSchemaField | IdField,
     SchemaType.EVENT_SCHEMA: ConcreteSchemaField | IdField | SchemaReference,
 }
 
 
 class SchemaValidator:
     def __init__(self, schema_type: SchemaType) -> None:
         self.__schema_type = schema_type
 
     def check_class_attributes(self, cls: type[T]) -> None:
         for _, type_ in cls.__annotations__.items():
-            type_ = SchemaUtil.if_not_class_get_origin(type_)
+            type_ = GenericClassUtil.if_not_class_get_origin(type_)
             if not (
                 issubclass(
                     type_,
                     get_args(valid_schema_field_types[self.__schema_type]),
                 )
             ):
                 raise InvalidAttributeException(
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/source/source.py` & `superlinked-5.2.2/superlinked/framework/common/source/source.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/source/types.py` & `superlinked-5.2.2/superlinked/framework/common/source/types.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/space/aggregation.py` & `superlinked-5.2.2/superlinked/framework/common/space/aggregation.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/space/normalization.py` & `superlinked-5.2.2/superlinked/framework/common/space/normalization.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,37 +12,36 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from abc import ABC, abstractmethod
 from typing import Any
 
 import numpy as np
-import numpy.typing as npt
 from typing_extensions import override
 
-from superlinked.framework.common.data_types import Vector
+from superlinked.framework.common.data_types import NPArray, Vector
 
 
 class Normalization(ABC):
 
     @abstractmethod
-    def norm(self, value: npt.NDArray[np.float64]) -> float: ...
+    def norm(self, value: NPArray) -> float: ...
 
     def denormalize(self, vector: Vector) -> Vector:
         if vector.vector_before_normalization is None:
             return vector
         return vector.vector_before_normalization.apply_negative_filter(vector)
 
     def __str__(self) -> str:
         return f"{self.__class__.__name__}({self.__dict__ if self.__dict__ else ''})"
 
 
 class L2Norm(Normalization):
     @override
-    def norm(self, value: npt.NDArray[np.float64]) -> float:
+    def norm(self, value: NPArray) -> float:
         return np.linalg.norm(value)  # type: ignore[attr-defined]
 
     @override
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, type(self))
 
 
@@ -52,15 +51,15 @@
         self.__validate_length()
 
     def __validate_length(self) -> None:
         if self.length == 0:
             raise ValueError("Normalization length cannot be zero.")
 
     @override
-    def norm(self, value: npt.NDArray[np.float64]) -> float:
+    def norm(self, value: NPArray) -> float:
         return self.length
 
     @override
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, type(self)) and self.length == other.length
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/storage/entity.py` & `superlinked-5.2.2/superlinked/framework/common/storage/entity.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from dataclasses import dataclass
 
-from beartype.typing import Sequence
-
 from superlinked.framework.common.storage.entity_id import EntityId
 from superlinked.framework.common.storage.field import Field
 
 
 @dataclass
 class Entity:
     id_: EntityId
-    fields: Sequence[Field]
+    fields: dict[str, Field]
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/storage/entity_data.py` & `superlinked-5.2.2/superlinked/framework/common/storage_manager/search_result_item.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from dataclasses import dataclass
 
 from beartype.typing import Sequence
 
-from superlinked.framework.common.storage.entity_id import EntityId
-from superlinked.framework.common.storage.field_data import FieldData
+from superlinked.framework.common.parser.parsed_schema import ParsedSchemaField
+from superlinked.framework.common.storage_manager.header import Header
 
 
-@dataclass
-class EntityData:
-    id_: EntityId
-    field_data: Sequence[FieldData]
+@dataclass(frozen=True)
+class SearchResultItem:
+    header: Header
+    fields: Sequence[ParsedSchemaField]
+    score: float
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/storage/entity_id.py` & `superlinked-5.2.2/superlinked/framework/common/storage/entity_id.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/storage/exception.py` & `superlinked-5.2.2/superlinked/framework/common/storage/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/storage/field.py` & `superlinked-5.2.2/superlinked/framework/common/storage/field.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,24 +10,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from dataclasses import dataclass
-
 from superlinked.framework.common.interface.comparison_operand import ComparisonOperand
 from superlinked.framework.common.storage.field_data_type import FieldDataType
 
 
-@dataclass(frozen=True)
 class Field(ComparisonOperand):
-    data_type: FieldDataType
-    name: str
+    def __init__(self, data_type: FieldDataType, name: str) -> None:
+        super().__init__(Field)
+        self.data_type = data_type
+        self.name = name
+
+    def __hash__(self) -> int:
+        return hash((self.name, self.data_type))
 
     @staticmethod
     def _built_in_equal(
         left_operand: ComparisonOperand[Field], right_operand: object
     ) -> bool:
         if isinstance(left_operand, Field) and isinstance(right_operand, Field):
             return (
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/storage/field_data.py` & `superlinked-5.2.2/superlinked/framework/common/storage/field_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,40 +13,34 @@
 # limitations under the License.
 
 
 from __future__ import annotations
 
 from typing import Generic, TypeVar
 
-from superlinked.framework.common.data_types import Vector
+from superlinked.framework.common.data_types import NPArray, Vector
 from superlinked.framework.common.storage.field import Field
 from superlinked.framework.common.storage.field_data_type import FieldDataType
+from superlinked.framework.common.storage.field_type_converter import FieldTypeConverter
 
+# FieldType
 FT = TypeVar("FT")
 
-VALID_TYPE_BY_FIELD_DATA_TYPE: dict[FieldDataType, type] = {
-    FieldDataType.BLOB: str,
-    FieldDataType.DOUBLE: float,
-    FieldDataType.INT: int,
-    FieldDataType.STRING: str,
-    FieldDataType.VECTOR: Vector,
-}
-
 
 class FieldData(Field, Generic[FT]):
     def __init__(self, type_: FieldDataType, name: str, value: FT) -> None:
         super().__init__(type_, name)
         self.__validate_value(type_, value)
         self.value = value
 
-    def __validate_value(self, type_: FieldDataType, value: FT) -> None:
-        valid_type = VALID_TYPE_BY_FIELD_DATA_TYPE[type_]
+    def __validate_value(self, data_type: FieldDataType, value: FT) -> None:
+        valid_type = FieldTypeConverter.get_valid_python_types(data_type)
         if not isinstance(value, valid_type):
             raise ValueError(
-                f"Invalid value {value} for the given field data type {type_}"
+                f"Invalid value {value} for the given field data type {data_type}"
             )
 
     @classmethod
     def from_field(cls, field: Field, value: FT) -> FieldData:
         return cls(field.data_type, field.name, value)
 
 
@@ -61,14 +55,19 @@
 
 
 class IntFieldData(FieldData[int]):
     def __init__(self, name: str, value: int) -> None:
         super().__init__(FieldDataType.INT, name, value)
 
 
+class NPArrayFieldData(FieldData[NPArray]):
+    def __init__(self, name: str, value: NPArray) -> None:
+        super().__init__(FieldDataType.NPARRAY, name, value)
+
+
 class StringFieldData(FieldData[str]):
     def __init__(self, name: str, value: str) -> None:
         super().__init__(FieldDataType.STRING, name, value)
 
 
 class VectorFieldData(FieldData[Vector]):
     def __init__(self, name: str, value: Vector) -> None:
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/storage/field_data_type.py` & `superlinked-5.2.2/superlinked/framework/common/storage/field_data_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,9 +15,10 @@
 from enum import Enum
 
 
 class FieldDataType(Enum):
     BLOB = "BLOB"
     DOUBLE = "DOUBLE"
     INT = "INT"
+    NPARRAY = "NPARRAY"
     STRING = "STRING"
     VECTOR = "VECTOR"
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/storage/field_encoder.py` & `superlinked-5.2.2/superlinked/framework/common/storage/field_encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from abc import ABC, abstractmethod
 from typing import Any, Callable, Generic, TypeVar
 
-from superlinked.framework.common.data_types import Vector
+from superlinked.framework.common.data_types import NPArray, Vector
 from superlinked.framework.common.storage.exception import EncoderException
 from superlinked.framework.common.storage.field import Field
 from superlinked.framework.common.storage.field_data import FieldData
 from superlinked.framework.common.storage.field_data_type import FieldDataType
 
 # Encoded type
 ET = TypeVar("ET")
@@ -27,21 +27,23 @@
 
 class FieldEncoder(ABC, Generic[ET]):
     def __init__(self) -> None:
         self._encode_map: dict[FieldDataType, Callable[..., ET]] = {
             FieldDataType.BLOB: self._encode_blob,
             FieldDataType.DOUBLE: self._encode_double,
             FieldDataType.INT: self._encode_int,
+            FieldDataType.NPARRAY: self._encode_nparray,
             FieldDataType.STRING: self._encode_string,
             FieldDataType.VECTOR: self._encode_vector,
         }
         self._decode_map: dict[FieldDataType, Callable[[ET], Any]] = {
             FieldDataType.BLOB: self._decode_blob,
             FieldDataType.DOUBLE: self._decode_double,
             FieldDataType.INT: self._decode_int,
+            FieldDataType.NPARRAY: self._decode_nparray,
             FieldDataType.STRING: self._decode_string,
             FieldDataType.VECTOR: self._decode_vector,
         }
 
     @abstractmethod
     def _encode_blob(self, blob: str) -> ET:
         pass
@@ -63,14 +65,22 @@
         pass
 
     @abstractmethod
     def _decode_int(self, int_: ET) -> int:
         pass
 
     @abstractmethod
+    def _encode_nparray(self, nparray: NPArray) -> ET:
+        pass
+
+    @abstractmethod
+    def _decode_nparray(self, nparray: ET) -> NPArray:
+        pass
+
+    @abstractmethod
     def _encode_string(self, string: str) -> ET:
         pass
 
     @abstractmethod
     def _decode_string(self, string: ET) -> str:
         pass
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/storage/persistence_type.py` & `superlinked-5.2.2/superlinked/framework/common/storage/persistence_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py` & `superlinked-5.2.2/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,18 +19,18 @@
     SearchAlgorithm,
 )
 from superlinked.framework.common.storage.search_index_creation.vector_component_precision import (
     VectorComponentPrecision,
 )
 
 
-@dataclass
+@dataclass(frozen=True)
 class IndexFieldDescriptor:
     field_name: str
 
 
-@dataclass
+@dataclass(frozen=True)
 class VectorIndexFieldDescriptor(IndexFieldDescriptor):
     field_size: int
     distance_metric: DistanceMetric
     search_algorithm: SearchAlgorithm
     coordinate_type: VectorComponentPrecision
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/storage/search_index_creation/search_algorithm.py` & `superlinked-5.2.2/superlinked/framework/common/storage/search_index_creation/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py` & `superlinked-5.2.2/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/storage/vdb_connector.py` & `superlinked-5.2.2/superlinked/framework/common/storage/vdb_connector.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,23 +16,24 @@
 from typing import Any
 
 from beartype.typing import Sequence
 
 from superlinked.framework.common.storage.entity import Entity
 from superlinked.framework.common.storage.entity_data import EntityData
 from superlinked.framework.common.storage.field import Field
+from superlinked.framework.common.storage.result_entity_data import ResultEntityData
 from superlinked.framework.common.storage.search_index_creation.index_field_descriptor import (
     IndexFieldDescriptor,
     VectorIndexFieldDescriptor,
 )
 from superlinked.framework.common.storage.search_index_creation.search_algorithm import (
     SearchAlgorithm,
 )
 from superlinked.framework.common.storage.vdb_knn_search_params import (
-    VDBKnnSearchParams,
+    VDBKNNSearchParams,
 )
 
 
 class VDBConnector(ABC):
     @abstractmethod
     def close_connection(self) -> None:
         pass
@@ -66,11 +67,11 @@
 
     @abstractmethod
     def knn_search(
         self,
         index_name: str,
         schema_name: str,
         returned_fields: Sequence[Field],
-        vdb_knn_search_params: VDBKnnSearchParams,
+        vdb_knn_search_params: VDBKNNSearchParams,
         **params: Any
-    ) -> Sequence[EntityData]:
+    ) -> Sequence[ResultEntityData]:
         pass
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/storage/vdb_knn_search_params.py` & `superlinked-5.2.2/superlinked/framework/common/storage/vdb_knn_search_params.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,13 +19,13 @@
 from superlinked.framework.common.interface.comparison_operand import (
     ComparisonOperation,
 )
 from superlinked.framework.common.storage.field import Field
 from superlinked.framework.common.storage.field_data import VectorFieldData
 
 
-@dataclass
-class VDBKnnSearchParams:
+@dataclass(frozen=True)
+class VDBKNNSearchParams:
     vector_field: VectorFieldData
-    limit: int
+    limit: int | None
     filters: Sequence[ComparisonOperation[Field]] | None = None
     radius: float | None = None
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/storage_manager/entity_builder.py` & `superlinked-5.2.2/superlinked/framework/common/storage_manager/entity_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,88 +13,82 @@
 # limitations under the License.
 
 
 from typing import Any
 
 from beartype.typing import Sequence
 
+from superlinked.framework.common.data_types import PythonTypes
 from superlinked.framework.common.parser.parsed_schema import (
     ParsedSchema,
     ParsedSchemaField,
 )
 from superlinked.framework.common.schema.id_schema_object import IdSchemaObject
 from superlinked.framework.common.schema.schema_object import SchemaField
 from superlinked.framework.common.storage.entity import Entity
 from superlinked.framework.common.storage.entity_data import EntityData
 from superlinked.framework.common.storage.entity_id import EntityId
 from superlinked.framework.common.storage.field import Field
-from superlinked.framework.common.storage.field_data import FieldData, StringFieldData
-from superlinked.framework.common.storage_manager.field_type_converter import (
-    FieldTypeConverter,
-)
+from superlinked.framework.common.storage.field_data import FieldData
+from superlinked.framework.common.storage.field_type_converter import FieldTypeConverter
+from superlinked.framework.common.storage_manager.admin_fields import AdminFields
 from superlinked.framework.common.storage_manager.storage_naming import StorageNaming
 
 
 class EntityBuilder:
     def __init__(
         self,
         storage_naming: StorageNaming,
-        field_type_converter: FieldTypeConverter | None = None,
     ) -> None:
         self._storage_naming = storage_naming
-        self._field_type_converter = field_type_converter or FieldTypeConverter()
+        self._admin_fields = AdminFields()
 
     def compose_entity_id(self, schema_id: str, object_id: str) -> EntityId:
         return EntityId(schema_id, object_id)
 
     def compose_entity(self, entity_id: EntityId, fields: Sequence[Field]) -> Entity:
-        return Entity(entity_id, fields)
+        return Entity(entity_id, {field.name: field for field in fields})
 
     def convert_schema_field_to_field(self, schema_field: SchemaField) -> Field:
         return Field(
-            self._field_type_converter.convert_schema_field_type(type(schema_field)),
+            FieldTypeConverter.convert_schema_field_type(type(schema_field)),
             self._storage_naming.generate_field_name_from_schema_field(schema_field),
         )
 
     def convert_parsed_schema_field_to_field_data(
         self, parsed_schema_field: ParsedSchemaField
     ) -> FieldData:
         field = self.convert_schema_field_to_field(parsed_schema_field.schema_field)
         return FieldData.from_field(field, parsed_schema_field.value)
 
-    def compose_entity_from_schema_fields(
+    def compose_entity_data(
         self,
         schema_id: str,
         object_id: str,
-        schema_fields: Sequence[SchemaField],
-    ) -> Entity:
+        field_data: Sequence[FieldData],
+    ) -> EntityData:
         entity_id = self.compose_entity_id(schema_id, object_id)
-        return Entity(
-            entity_id,
-            [
-                self.convert_schema_field_to_field(schema_field)
-                for schema_field in schema_fields
-            ],
+        admin_field_data = list(self._admin_fields.create_header_field_data(entity_id))
+        return EntityData(
+            entity_id, {fd.name: fd for fd in (list(field_data) + admin_field_data)}
         )
 
-    def compose_entity_data(
+    def compose_entity_data_from_parsed_schema_fields(
         self,
         schema_id: str,
         object_id: str,
         parsed_schema_fields: Sequence[ParsedSchemaField],
     ) -> EntityData:
-        entity_id = self.compose_entity_id(schema_id, object_id)
-        base_fields = list(self.create_admin_field_data(entity_id))
-        return EntityData(
-            entity_id,
+        return self.compose_entity_data(
+            schema_id,
+            object_id,
             [
                 self.convert_parsed_schema_field_to_field_data(parsed_schema_field)
                 for parsed_schema_field in parsed_schema_fields
-            ]
-            + base_fields,
+            ],
         )
 
     def parse_schema_field_data(
         self,
         schema_field_data: FieldData,
         schema_field_by_field_name: dict[str, SchemaField],
     ) -> ParsedSchemaField:
@@ -109,66 +103,50 @@
         schema_field_by_field_name: dict[str, SchemaField],
     ) -> ParsedSchema:
         return ParsedSchema(
             schema,
             entity_data.id_.object_id,
             [
                 self.parse_schema_field_data(field_data, schema_field_by_field_name)
-                for field_data in entity_data.field_data
+                for field_data in entity_data.field_data.values()
             ],
         )
 
-    def create_admin_field_data(
-        self,
-        entity_id: EntityId,
-        origin_id: str | None = None,
-    ) -> Sequence[FieldData]:
-        field_data = [
-            StringFieldData(StorageNaming.SCHEMA_INDEX_NAME, entity_id.schema_id),
-            StringFieldData(StorageNaming.OBJECT_ID_INDEX_NAME, entity_id.object_id),
-        ]
-        if origin_id:
-            field_data.append(
-                StringFieldData(StorageNaming.ORIGIN_ID_INDEX_NAME, origin_id)
-            )
-        return field_data
-
     def compose_field_from_node_data_descriptor(
-        self, node_data_key: str, node_data_type: type
+        self, node_id: str, node_data_key: str, node_data_type: type[PythonTypes]
     ) -> Field:
-        return Field(
-            self._field_type_converter.convert_python_type(node_data_type),
-            self._storage_naming.generate_node_data_field_name(node_data_key),
+        return self.compose_field(
+            self._storage_naming.generate_node_data_field_name(node_id, node_data_key),
+            node_data_type,
         )
 
     def compose_field(
         self,
-        node_id: str,
-        result_type: type,
+        field_name: str,
+        field_value_type: type,
     ) -> Field:
         return Field(
-            self._field_type_converter.convert_python_type(result_type),
-            node_id,
+            FieldTypeConverter.convert_python_type(field_value_type),
+            field_name,
         )
 
     def compose_field_data(
-        self,
-        node_id: str,
-        result: Any,
+        self, field_name: str, field_value: PythonTypes
     ) -> FieldData:
         return FieldData(
-            self._field_type_converter.convert_python_type(type(result)),
-            node_id,
-            result,
+            FieldTypeConverter.convert_python_type(type(field_value)),
+            field_name,
+            field_value,
         )
 
     def compose_field_data_from_node_data(
-        self, node_data: dict[str, Any]
+        self, node_id: str, node_data: dict[str, Any]
     ) -> Sequence[FieldData]:
         return [
             FieldData(
-                self._field_type_converter.convert_python_type(type(value)),
-                self._storage_naming.generate_node_data_field_name(key),
+                FieldTypeConverter.convert_python_type(type(value)),
+                self._storage_naming.generate_node_data_field_name(node_id, key),
                 value,
             )
             for key, value in node_data.items()
+            if value is not None
         ]
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/storage_manager/field_type_converter.py` & `superlinked-5.2.2/superlinked/framework/common/storage/field_type_converter.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,55 +10,72 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Any, cast
 
-from superlinked.framework.common.data_types import Vector
+from superlinked.framework.common.data_types import NPArray, PythonTypes, Vector
 from superlinked.framework.common.schema.schema_object import (
     Array,
     ConcreteSchemaField,
     Float,
     Integer,
     SchemaField,
     String,
     Timestamp,
 )
 from superlinked.framework.common.storage.field_data_type import FieldDataType
+from superlinked.framework.common.util.generic_class_util import GenericClassUtil
 
 FIELD_DATA_TYPE_BY_SCHEMA_FIELD_TYPE: dict[type[ConcreteSchemaField], FieldDataType] = {
-    Array: FieldDataType.VECTOR,
+    Array: FieldDataType.NPARRAY,
     Float: FieldDataType.DOUBLE,
     Integer: FieldDataType.INT,
     String: FieldDataType.STRING,
     Timestamp: FieldDataType.INT,
 }
 
-PytonTypes = float | int | str | Vector
-
-FIELD_DATA_TYPE_BY_PYTHON_TYPE: dict[type[PytonTypes], FieldDataType] = {
-    float: FieldDataType.INT,
-    int: FieldDataType.DOUBLE,
+FIELD_DATA_TYPE_BY_PYTHON_TYPE: dict[type[PythonTypes], FieldDataType] = {
+    float: FieldDataType.DOUBLE,
+    int: FieldDataType.INT,
     str: FieldDataType.STRING,
-    Vector: FieldDataType.INT,
+    NPArray: FieldDataType.NPARRAY,
+    Vector: FieldDataType.VECTOR,
+}
+
+VALID_TYPE_BY_FIELD_DATA_TYPE: dict[FieldDataType, type[PythonTypes]] = {
+    FieldDataType.BLOB: str,
+    FieldDataType.DOUBLE: float,
+    FieldDataType.INT: int,
+    FieldDataType.NPARRAY: NPArray,
+    FieldDataType.STRING: str,
+    FieldDataType.VECTOR: Vector,
 }
 
 
 class FieldTypeConverter:
+    @staticmethod
     def convert_schema_field_type(
-        self, schema_field_cls: type[SchemaField[Any]]
+        schema_field_cls: type[SchemaField[Any]],
     ) -> FieldDataType:
         if field_data_type := FIELD_DATA_TYPE_BY_SCHEMA_FIELD_TYPE.get(
             cast(type[ConcreteSchemaField], schema_field_cls)
         ):
             return field_data_type
         raise NotImplementedError(
             f"Unknown schema field type: {schema_field_cls.__name__}"
         )
 
-    def convert_python_type(self, type_: type) -> FieldDataType:
+    @staticmethod
+    def convert_python_type(type_: type[PythonTypes]) -> FieldDataType:
         if field_data_type := FIELD_DATA_TYPE_BY_PYTHON_TYPE.get(
-            cast(type[PytonTypes], type_)
+            cast(type[PythonTypes], type_)
         ):
             return field_data_type
         raise NotImplementedError(f"Unknown python type: {type_}")
+
+    @staticmethod
+    def get_valid_python_types(data_type: FieldDataType) -> type[PythonTypes]:
+        return GenericClassUtil.if_not_class_get_origin(
+            VALID_TYPE_BY_FIELD_DATA_TYPE[data_type]
+        )
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/storage_manager/knn_search_params.py` & `superlinked-5.2.2/superlinked/framework/dsl/query/predicate/query_predicate.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,23 +9,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from dataclasses import dataclass
+from enum import Enum
+from typing import Generic, TypeVar
 
-from beartype.typing import Sequence
-
-from superlinked.framework.common.data_types import Vector
-from superlinked.framework.common.interface.comparison_operand import (
-    ComparisonOperation,
-)
 from superlinked.framework.common.schema.schema_object import SchemaField
+from superlinked.framework.dsl.query.param import NumericParamType, Param
+
+# Exclude from documentation.
+__pdoc__ = {}
+__pdoc__["QueryPredicate"] = False
+
+# Operation type
+OPT = TypeVar("OPT", bound=Enum)
 
 
-@dataclass
-class KnnSearchParams:
-    vector: Vector
-    limit: int
-    filters: Sequence[ComparisonOperation[SchemaField]] | None = None
-    radius: float | None = None
+@dataclass(frozen=True)
+class QueryPredicate(Generic[OPT]):
+    op: OPT
+    params: list[SchemaField | Param | str | int | float | None]
+    weight_param: NumericParamType
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/storage_manager/node_result_params.py` & `superlinked-5.2.2/superlinked/framework/common/storage_manager/header.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from dataclasses import dataclass
-from typing import Any
 
 
-@dataclass
-class NodeResultParams:
-    result: Any
-    origin_id: str | None = None
-    node_data: dict[str, Any] | None = None
+@dataclass(frozen=True)
+class Header:
+    schema_id: str
+    object_id: str
+    origin_id: str | None
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/storage_manager/storage_manager.py` & `superlinked-5.2.2/superlinked/framework/common/storage_manager/storage_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,51 +16,55 @@
 from typing import Any, Iterator, TypeVar, cast
 
 from beartype.typing import Sequence
 
 from superlinked.framework.common.calculation.distance_metric import DistanceMetric
 from superlinked.framework.common.dag.dag import Dag
 from superlinked.framework.common.dag.index_node import IndexNode
+from superlinked.framework.common.data_types import Json, PythonTypes
 from superlinked.framework.common.exception import InvalidSchemaException
 from superlinked.framework.common.interface.comparison_operand import (
     ComparisonOperation,
 )
 from superlinked.framework.common.parser.parsed_schema import (
     ParsedSchema,
     ParsedSchemaField,
 )
 from superlinked.framework.common.schema.id_schema_object import IdSchemaObject
 from superlinked.framework.common.schema.schema_object import SchemaField, SchemaObject
 from superlinked.framework.common.storage.entity_data import EntityData
 from superlinked.framework.common.storage.field import Field
 from superlinked.framework.common.storage.field_data import VectorFieldData
+from superlinked.framework.common.storage.result_entity_data import ResultEntityData
 from superlinked.framework.common.storage.search_index_creation.index_field_descriptor import (
     IndexFieldDescriptor,
     VectorIndexFieldDescriptor,
 )
 from superlinked.framework.common.storage.search_index_creation.search_algorithm import (
     SearchAlgorithm,
 )
 from superlinked.framework.common.storage.search_index_creation.vector_component_precision import (
     VectorComponentPrecision,
 )
 from superlinked.framework.common.storage.vdb_connector import VDBConnector
 from superlinked.framework.common.storage.vdb_knn_search_params import (
-    VDBKnnSearchParams,
+    VDBKNNSearchParams,
 )
 from superlinked.framework.common.storage_manager.entity_builder import EntityBuilder
 from superlinked.framework.common.storage_manager.knn_search_params import (
-    KnnSearchParams,
+    KNNSearchParams,
 )
-from superlinked.framework.common.storage_manager.node_result_params import (
-    NodeResultParams,
+from superlinked.framework.common.storage_manager.search_result_item import (
+    SearchResultItem,
 )
 from superlinked.framework.common.storage_manager.storage_naming import StorageNaming
 
 ResultTypeT = TypeVar("ResultTypeT")
+# NodeDataValueType
+NDVT = TypeVar("NDVT", bound=PythonTypes)
 
 
 class StorageManager:
     def __init__(
         self,
         vdb_connector: VDBConnector,
     ) -> None:
@@ -97,81 +101,109 @@
         self._vdb_connector.drop_search_index(index_name)
 
     def knn_search(
         self,
         index_node: IndexNode,
         schema: IdSchemaObject,
         returned_schema_fields: Sequence[SchemaField],
-        knn_search_params: KnnSearchParams,
+        knn_search_params: KNNSearchParams,
         **params: Any,
-    ) -> Sequence[ParsedSchema]:
-        self._check_valid_knn_search_input(schema, returned_schema_fields)
+    ) -> Sequence[SearchResultItem]:
+        self._validate_knn_search_input(schema, returned_schema_fields)
         index_name = self._storage_naming.get_index_name_from_index_node(index_node)
         vector_field = cast(
             VectorFieldData,
             self._entity_builder.compose_field_data(
                 index_node.node_id, knn_search_params.vector
             ),
         )
         returned_fields = {
             self._entity_builder.convert_schema_field_to_field(
                 returned_schema_field
             ): returned_schema_field
             for returned_schema_field in returned_schema_fields
         }
-        search_result: Sequence[EntityData] = self._vdb_connector.knn_search(
+        search_result: Sequence[ResultEntityData] = self._vdb_connector.knn_search(
             index_name,
             schema._schema_name,
-            list(returned_fields.keys()),
-            VDBKnnSearchParams(
+            list(returned_fields.keys())
+            + list(self._entity_builder._admin_fields.header_fields),
+            VDBKNNSearchParams(
                 vector_field,
                 knn_search_params.limit,
-                self._get_filter_field_data(knn_search_params.filters or []),
+                self._compose_filter_field_data(
+                    schema, knn_search_params.filters or []
+                ),
                 knn_search_params.radius,
             ),
             **params,
         )
         schema_field_by_field_name = self._create_schema_field_by_field_name(
             returned_fields
         )
         return [
-            self._entity_builder.parse_entity_data(
-                schema, entity_data, schema_field_by_field_name
+            SearchResultItem(
+                self._entity_builder._admin_fields.extract_header(
+                    result_entity_data.field_data
+                ),
+                [
+                    self._entity_builder.parse_schema_field_data(
+                        field_data, schema_field_by_field_name
+                    )
+                    for field_data in result_entity_data.field_data.values()
+                    if not self._entity_builder._admin_fields.is_admin_field(field_data)
+                ],
+                result_entity_data.score,
             )
-            for entity_data in search_result
+            for result_entity_data in search_result
         ]
 
-    def _check_valid_knn_search_input(
+    def _validate_knn_search_input(
         self,
         schema: SchemaObject,
         returned_schema_fields: Sequence[SchemaField],
     ) -> None:
         if invalid_schema_fields := [
             schema_field
             for schema_field in returned_schema_fields
             if schema_field.schema_obj != schema
         ]:
             raise InvalidSchemaException(
                 "`knn_search` can only return schema_fields from "
                 + f"the searched schema {schema}, got {invalid_schema_fields}"
             )
 
-    def _get_filter_field_data(
-        self, filters: Sequence[ComparisonOperation[SchemaField]]
+    def _compose_filter_field_data(
+        self, schema: SchemaObject, filters: Sequence[ComparisonOperation[SchemaField]]
     ) -> Sequence[ComparisonOperation[Field]]:
         return [
             ComparisonOperation(
                 filter_._op,
                 self._entity_builder.convert_schema_field_to_field(
                     cast(SchemaField, filter_._operand)
                 ),
                 filter_._other,
             )
             for filter_ in filters
-        ]
+        ] + [self._entity_builder._admin_fields.schema_id.field == schema._schema_name]
+
+    def write_object_blob(
+        self, schema: SchemaObject, object_id: str, object_blob: Json
+    ) -> None:
+        if object_blob_data_field := (
+            self._entity_builder._admin_fields.create_object_blob_field_data(
+                object_blob
+            )
+        ):
+            entity_data = self._entity_builder.compose_entity_data(
+                schema._schema_name,
+                object_id,
+                [object_blob_data_field],
+            )
+            self._vdb_connector.write_entities([entity_data])
 
     def write_parsed_schema_fields(
         self, object_id: str, parsed_schema_fields: Sequence[ParsedSchemaField]
     ) -> None:
         def get_schema_name_of_parsed_schema_field(
             parsed_schema_field: ParsedSchemaField,
         ) -> str:
@@ -184,51 +216,84 @@
                 sorted(
                     parsed_schema_fields,
                     key=get_schema_name_of_parsed_schema_field,
                 ),
                 get_schema_name_of_parsed_schema_field,
             )
 
-        fields = [
-            self._entity_builder.compose_entity_data(
+        entity_data = [
+            self._entity_builder.compose_entity_data_from_parsed_schema_fields(
                 schema_name, object_id, list(parsed_schema_fields_group)
             )
             for schema_name, parsed_schema_fields_group in group_parsed_schema_fields_by_schema_name(
                 parsed_schema_fields
             )
         ]
-        self._vdb_connector.write_entities(fields)
+        self._vdb_connector.write_entities(entity_data)
 
     def write_node_result(
         self,
         schema: SchemaObject,
         object_id: str,
         node_id: str,
-        node_result_params: NodeResultParams,
+        result: PythonTypes,
+        origin_id: str | None = None,
     ) -> None:
         entity_id = self._entity_builder.compose_entity_id(
             schema._schema_name, object_id
         )
         field_data = list(
-            self._entity_builder.create_admin_field_data(
-                entity_id, node_result_params.origin_id
+            self._entity_builder._admin_fields.create_header_field_data(
+                entity_id, origin_id
             )
         )
-        result_field_data = self._entity_builder.compose_field_data(
-            node_id, node_result_params.result
+        if result is not None:
+            result_field_data = self._entity_builder.compose_field_data(node_id, result)
+            field_data.append(result_field_data)
+        self._vdb_connector.write_entities(
+            [EntityData(entity_id, {fd.name: fd for fd in field_data})]
+        )
+
+    def write_node_data(
+        self,
+        schema: SchemaObject,
+        object_id: str,
+        node_id: str,
+        node_data: dict[str, PythonTypes],
+    ) -> None:
+        entity_id = self._entity_builder.compose_entity_id(
+            schema._schema_name, object_id
+        )
+        field_data = list(
+            self._entity_builder._admin_fields.create_header_field_data(entity_id)
         )
-        field_data.append(result_field_data)
         field_data.extend(
             list(
                 self._entity_builder.compose_field_data_from_node_data(
-                    node_result_params.node_data or {}
+                    node_id, node_data
                 )
             )
         )
-        self._vdb_connector.write_entities([EntityData(entity_id, field_data)])
+        self._vdb_connector.write_entities(
+            [EntityData(entity_id, {fd.name: fd for fd in field_data})]
+        )
+
+    def read_object_blob(
+        self, schema: SchemaObject, object_id: str
+    ) -> dict[str, Any] | None:
+        entity = self._entity_builder.compose_entity(
+            self._entity_builder.compose_entity_id(schema._schema_name, object_id),
+            [self._entity_builder._admin_fields.object_blob.field],
+        )
+        entity_data = self._vdb_connector.read_entities([entity])
+        if not entity_data:
+            return None
+        return self._entity_builder._admin_fields.extract_object_blob_field_data(
+            entity_data[0].field_data
+        )
 
     def read_schema_field_values(
         self, object_id: str, schema_fields: Sequence[SchemaField]
     ) -> ParsedSchema:
         schema = self._get_schema_of_schema_fields(schema_fields)
         entity_id = self._entity_builder.compose_entity_id(
             schema._schema_name, object_id
@@ -265,43 +330,58 @@
 
     def read_node_result(
         self,
         schema: SchemaObject,
         object_id: str,
         node_id: str,
         result_type: type[ResultTypeT],
-        node_data_descriptor: dict[str, type] | None = None,
-    ) -> tuple[ResultTypeT | None, dict[str, Any]]:
+    ) -> ResultTypeT | None:
         entity_id = self._entity_builder.compose_entity_id(
             schema._schema_name, object_id
         )
         result_field = self._entity_builder.compose_field(node_id, result_type)
-        node_data_key_by_field = self._map_node_data_keys_to_fields(
-            node_data_descriptor or {}
-        )
-        fields = list(node_data_key_by_field.keys()) + [result_field]
+        fields = [result_field]
         entity = self._entity_builder.compose_entity(entity_id, fields)
-        node_data_key_by_field_name = {
-            field.name: key for field, key in node_data_key_by_field.items()
-        }
         entity_data = self._vdb_connector.read_entities([entity])[0]
-        node_data = {
-            node_data_key_by_field_name[field_data.name]: field_data.value
-            for field_data in entity_data.field_data
-            if field_data.name != result_field.name
-        }
         result_value = next(
             (
                 cast(ResultTypeT, field_data.value)
-                for field_data in entity_data.field_data
+                for field_data in entity_data.field_data.values()
                 if field_data.name == result_field.name
             ),
             None,
         )
-        return result_value, node_data
+        return result_value
+
+    def read_node_data(
+        self,
+        schema: SchemaObject,
+        object_id: str,
+        node_id: str,
+        node_data_descriptor: dict[str, type[NDVT]],
+    ) -> dict[str, NDVT]:
+        entity_id = self._entity_builder.compose_entity_id(
+            schema._schema_name, object_id
+        )
+        field_by_node_data_key = self._map_fields_by_node_data_keys(
+            node_id, node_data_descriptor or {}
+        )
+        if not field_by_node_data_key:
+            return {}
+        fields = list(field_by_node_data_key.values())
+        node_data_key_by_field_name = {
+            field.name: key for key, field in field_by_node_data_key.items()
+        }
+        entity = self._entity_builder.compose_entity(entity_id, fields)
+        entity_data = self._vdb_connector.read_entities([entity])[0]
+        node_data = {
+            node_data_key_by_field_name[field_data.name]: cast(NDVT, field_data.value)
+            for field_data in entity_data.field_data.values()
+        }
+        return node_data
 
     def _get_index_field_descriptors_from_dag(
         self,
         dag: Dag,
         distance_metric: DistanceMetric,
         search_algorithm: SearchAlgorithm,
         vector_coordinate_type: VectorComponentPrecision,
@@ -321,30 +401,35 @@
             [
                 IndexFieldDescriptor(
                     self._storage_naming.generate_field_name_from_schema_field(
                         indexed_field
                     )
                 )
                 for indexed_field in indexed_fields
+            ]
+            + [
+                IndexFieldDescriptor(
+                    self._entity_builder._admin_fields.schema_id.field.name
+                )
             ],
         )
 
     def _create_schema_field_by_field_name(
         self, fields: dict[Field, SchemaField]
     ) -> dict[str, SchemaField]:
         return {field.name: schema_field for field, schema_field in fields.items()}
 
-    def _map_node_data_keys_to_fields(
-        self, node_data_descriptor: dict[str, type]
-    ) -> dict[Field, str]:
+    def _map_fields_by_node_data_keys(
+        self, node_id: str, node_data_descriptor: dict[str, type[NDVT]]
+    ) -> dict[str, Field]:
         return {
-            self._entity_builder.compose_field_from_node_data_descriptor(
-                key, type_
-            ): key
-            for key, type_ in (node_data_descriptor).items()
+            key: self._entity_builder.compose_field_from_node_data_descriptor(
+                node_id, key, cast(type[PythonTypes], type_)
+            )
+            for key, type_ in node_data_descriptor.items()
         }
 
     @staticmethod
     def _get_indexed_schema_fields_of_dag(dag: Dag) -> Sequence[SchemaField]:
         # TODO FAI-1814: this should be filtered by the soon-to-be introduced Indexed property of the SchemaField.
         return [
             schema_field
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/storage_manager/storage_naming.py` & `superlinked-5.2.2/superlinked/framework/common/storage_manager/storage_naming.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,20 @@
 from superlinked.framework.common.schema.schema_object import SchemaField
 
 
 class StorageNaming:
     INDEX_PREFIX = "idx_"
     NODE_DATA_PREFIX = "__node_data__"
     OBJECT_ID_INDEX_NAME = "__object_id__"
+    OBJECT_BLOB_INDEX_NAME = "__object_blob__"
     ORIGIN_ID_INDEX_NAME = "__origin_id__"
     SCHEMA_INDEX_NAME = "__schema__"
     SCHEMA_FIELD_PREFIX = "__schema_field__"
 
     def get_index_name_from_index_node(self, index_node: IndexNode) -> str:
         return f"{StorageNaming.INDEX_PREFIX}{index_node.node_id}"
 
     def generate_field_name_from_schema_field(self, schema_field: SchemaField) -> str:
         return f"{StorageNaming.SCHEMA_FIELD_PREFIX}{schema_field.schema_obj._schema_name}_{schema_field.name}"
 
-    def generate_node_data_field_name(self, node_data_key: str) -> str:
-        return f"{StorageNaming.NODE_DATA_PREFIX}{node_data_key}"
+    def generate_node_data_field_name(self, node_id: str, node_data_key: str) -> str:
+        return f"{StorageNaming.NODE_DATA_PREFIX}{node_id}_{node_data_key}"
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/util/collection_util.py` & `superlinked-5.2.2/superlinked/framework/common/util/collection_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/util/dot_separated_path_util.py` & `superlinked-5.2.2/superlinked/framework/common/util/dot_separated_path_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/util/immutable_model.py` & `superlinked-5.2.2/superlinked/framework/common/util/immutable_model.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/util/named_function_evaluator.py` & `superlinked-5.2.2/superlinked/framework/common/util/named_function_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/util/schema_util.py` & `superlinked-5.2.2/superlinked/framework/common/util/generic_class_util.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,18 +9,43 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import inspect
-from typing import get_origin
+from typing import Any, cast, get_args, get_origin
 
+from beartype.typing import Sequence
+
+from superlinked.framework.common.data_types import NPArray
 from superlinked.framework.common.schema.general_type import T
 
 
-class SchemaUtil:
+class GenericClassUtil:
     @staticmethod
-    def if_not_class_get_origin(type_: type[T]) -> type | None:
+    def if_not_class_get_origin(type_: type[T]) -> type:
         if inspect.isclass(type_):
+            # For backward compatibility!
+            if type_ == NPArray:
+                return type_.__origin__
             return type_
-        return get_origin(type_)
+        return cast(type, get_origin(type_))
+
+    @staticmethod
+    def get_generic_types(object_: Any) -> Sequence[Any]:
+        generic_base_class = next(
+            filter(
+                lambda base_class: bool(get_args(base_class)),
+                getattr(object_.__class__, "__orig_bases__", []),
+            ),
+            None,
+        )
+        if not generic_base_class:
+            raise ValueError(
+                f"{object_.__class__.__name__} does not have a Generic base class."
+            )
+        return get_args(generic_base_class)
+
+    @staticmethod
+    def get_single_generic_type(object_: Any) -> Any:
+        return GenericClassUtil.get_generic_types(object_)[0]
```

### Comparing `superlinked-4.1.0/superlinked/framework/common/util/string_util.py` & `superlinked-5.2.2/superlinked/framework/common/util/string_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/util/time_util.py` & `superlinked-5.2.2/superlinked/framework/common/util/time_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/common/util/type_validator.py` & `superlinked-5.2.2/superlinked/framework/common/util/type_validator.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/compiler/online_schema_dag_compiler.py` & `superlinked-5.2.2/superlinked/framework/compiler/online_schema_dag_compiler.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,54 +10,51 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.dag.schema_dag import SchemaDag
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.online.dag.online_node import OnlineNode
 from superlinked.framework.online.dag.online_node_registry import OnlineNodeRegistry
 from superlinked.framework.online.dag.online_schema_dag import OnlineSchemaDag
-from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
-    EvaluationResultStoreManager,
-)
 
 
 class OnlineSchemaDagCompiler:
     def __init__(
         self, nodes: set[Node], store_compilation_results: bool = True
     ) -> None:
         self.__nodes = nodes
         self.__store_compilation_results = store_compilation_results
         self.__compiled_nodes: dict[str, OnlineNode] = {}
         self.__online_node_registry = OnlineNodeRegistry()
 
     def compile_node(
         self,
         node: Node,
-        evaluation_result_store_manager: EvaluationResultStoreManager,
+        storage_manager: StorageManager,
     ) -> OnlineNode:
         if compiled_node := self.__compiled_nodes.get(node.node_id):
             return compiled_node
         compiled_parents = [
-            self.compile_node(parent, evaluation_result_store_manager)
+            self.compile_node(parent, storage_manager)
             for parent in node.parents
             if parent in self.__nodes
         ]
         compiled_node = self.__online_node_registry.init_online_node(
-            node, compiled_parents, evaluation_result_store_manager
+            node, compiled_parents, storage_manager
         )
         self.__compiled_nodes[node.node_id] = compiled_node
         return compiled_node
 
     def compile_schema_dag(
         self,
         dag: SchemaDag,
-        evaluation_result_store_manager: EvaluationResultStoreManager,
+        storage_manager: StorageManager,
     ) -> OnlineSchemaDag:
         compiled_nodes: list[OnlineNode] = [
-            self.compile_node(node, evaluation_result_store_manager)
-            for node in dag.nodes
+            self.compile_node(node, storage_manager) for node in dag.nodes
         ]
         if not self.__store_compilation_results:
             self.__compiled_nodes = {}
         return OnlineSchemaDag(dag.schema, compiled_nodes)
```

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/data_loader/data_loader.py` & `superlinked-5.2.2/superlinked/framework/dsl/registry/exception.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from abc import ABC, abstractmethod
-from typing import Any
 
-
-class DataLoader(ABC):
-    @abstractmethod
-    def load(self) -> Any:
-        pass
+class DuplicateElementException(Exception):
+    pass
```

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/executor/exception.py` & `superlinked-5.2.2/superlinked/framework/dsl/executor/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/executor/executor.py` & `superlinked-5.2.2/superlinked/framework/dsl/executor/rest/rest_executor.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,131 +10,129 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
-from typing import Annotated, Any, Generic, TypeVar
+from typing import Mapping
 
-from beartype.typing import Sequence
-from typing_extensions import Self
-
-from superlinked.framework.common.dag.context import ExecutionContext
-from superlinked.framework.common.util.time_util import now
-from superlinked.framework.common.util.type_util import get_single_generic_type
-from superlinked.framework.common.util.type_validator import TypeValidator
+from superlinked.framework.common.dag.context import ContextValue
+from superlinked.framework.dsl.executor.executor import App, Executor
+from superlinked.framework.dsl.executor.in_memory.in_memory_executor import (
+    InMemoryApp,
+    InMemoryExecutor,
+)
+from superlinked.framework.dsl.executor.rest.rest_configuration import (
+    RestEndpointConfiguration,
+    RestQuery,
+)
+from superlinked.framework.dsl.executor.rest.rest_handler import RestHandler
 from superlinked.framework.dsl.index.index import Index
-from superlinked.framework.dsl.source.source import SourceT
-from superlinked.framework.storage.entity_store import EntityStore
-from superlinked.framework.storage.entity_store_manager import EntityStoreManager
-from superlinked.framework.storage.object_store import ObjectStore
-from superlinked.framework.storage.object_store_manager import ObjectStoreManager
-
-ExecutorT = TypeVar("ExecutorT", bound="Executor")
-EntityStoreT = TypeVar("EntityStoreT", bound=EntityStore)
-ObjectStoreT = TypeVar("ObjectStoreT", bound=ObjectStore)
+from superlinked.framework.dsl.source.data_loader_source import DataLoaderSource
+from superlinked.framework.dsl.source.rest_source import RestSource
 
 
-class App(ABC, Generic[ExecutorT, EntityStoreT, ObjectStoreT]):
+class RestExecutor(Executor[RestSource | DataLoaderSource]):
     """
-    Abstract base class for an App, a running executor that can for example do queries or ingest data.
+    The RestExecutor is a subclass of the Executor base class. It encapsulates all the parameters required for
+    the REST application. It also instantiates an InMemoryExecutor for data storage purposes.
+
+    Attributes:
+        sources (list[RestSource]): List of Rest sources that has information about the schema.
+        indices (list[Index]): List indices.
+        queries (list[RestQuery]): List of executable queries.
+        endpoint_configuration (RestEndpointConfiguration): Optional configuration for REST endpoints.
     """
 
     def __init__(
         self,
-        executor: ExecutorT,
-        entity_store: EntityStoreT,
-        object_store: ObjectStoreT,
-    ) -> None:
-        """
-        Initialize the App.
-
-        Args:
-            executor (TExecutor): The executor instance.
-            entity_store (EntityStore): The entity store instance.
-            object_store (ObjectStore): The object store instance.
-        """
-        self._executor = executor
-        self._entity_store = entity_store
-        self._entity_store_manager = EntityStoreManager(self._entity_store)
-        self._object_store = object_store
-        self._object_store_manager = ObjectStoreManager(self._object_store)
-        self.now = now()
-
-    @property
-    def executor(self) -> ExecutorT:
-        """
-        Get the executor.
-
-        Returns:
-            ExecutorT: The executor instance.
-        """
-        return self._executor
-
-    @property
-    def object_store_manager(self) -> ObjectStoreManager:
-        """
-        Get the object store manager.
+        sources: list[RestSource | DataLoaderSource],
+        indices: list[Index],
+        queries: list[RestQuery],
+        endpoint_configuration: RestEndpointConfiguration | None = None,
+        context_data: Mapping[str, Mapping[str, ContextValue]] | None = None,
+    ):
+        """
+        Initialize the RestExecutor.
+        Attributes:
+            sources (list[RestSource]): List of Rest sources that has information about the schema.
+            indices (list[Index]): List indices.
+            queries (list[RestQuery]): List of executable queries.
+            endpoint_configuration (RestEndpointConfiguration): Optional configuration for REST endpoints.
+        """
+        online_sources = [source._online_source for source in sources]
+        self._online_executor = InMemoryExecutor(online_sources, indices, context_data)
+        super().__init__(sources, indices, self._online_executor.context)
+
+        self._queries = queries
+        self._endpoint_configuration = (
+            endpoint_configuration or RestEndpointConfiguration()
+        )
 
-        Returns:
-            ObjectStoreManager: The object store manager instance.
+    def run(self) -> RestApp:
         """
-        return self._object_store_manager
-
-    @property
-    def entity_store_manager(self) -> EntityStoreManager:
-        """
-        Get the entity store manager.
+        Run the RestExecutor. It returns an app that will create rest endpoints.
 
         Returns:
-            EntityStoreManager: The entity store manager instance.
+            RestApp: An instance of RestApp.
         """
-        return self._entity_store_manager
+        return RestApp(self)
 
 
-class Executor(ABC, Generic[SourceT]):
+class RestApp(App):
     """
-    Abstract base class for an executor.
+    Rest implementation of the App class.
+
+    Attributes:
+        executor (RestExecutor): An instance of RestExecutor.
     """
 
-    @TypeValidator.wrap
-    def __init__(
-        self,
-        sources: Sequence[SourceT],
-        indices: Annotated[Sequence[Index], TypeValidator.list_validator(Index)],
-        context: ExecutionContext,
-    ) -> None:
+    def __init__(self, executor: RestExecutor):
         """
-        Initialize the Executor.
+        Initialize the RestApp from an RestExecutor.
 
         Args:
-            sources (list[SourceT]): The list of sources.
-            indices (list[Index]): The list of indices.
-            context (Mapping[str, Mapping[str, Any]]): The context mapping.
+            executor (RestExecutor): An instance of RestExecutor.
         """
-        TypeValidator.validate_list_item_type(
-            sources, get_single_generic_type(self), "sources"
+        self.__online_app = executor._online_executor.run()
+        super().__init__(
+            executor,
+            self.__online_app._vdb_connector,
+        )
+
+        self.__data_loader_sources = [
+            source
+            for source in executor._sources
+            if isinstance(source, DataLoaderSource)
+        ]
+
+        self.__rest_handler = RestHandler(
+            self.__online_app,
+            [source for source in executor._sources if isinstance(source, RestSource)],
+            executor._queries,
+            executor._endpoint_configuration,
         )
-        self._sources = sources
-        self._indices = indices
-        self._context = context
 
     @property
-    def context(self) -> ExecutionContext:
+    def data_loader_sources(self) -> list[DataLoaderSource]:
+        return self.__data_loader_sources
+
+    @property
+    def online_app(self) -> InMemoryApp:
         """
-        Get the context.
+        Property that returns the InMemoryApp instance associated with the RestApp.
 
         Returns:
-            Mapping[str, Mapping[str, Any]]: The context mapping.
+            InMemoryApp: An instance of InMemoryApp.
         """
-        return self._context
+        return self.__online_app
 
-    @abstractmethod
-    def run(self) -> App[Self, Any, Any]:
+    @property
+    def handler(self) -> RestHandler:
         """
-        Abstract method to run the executor.
+        Property that returns the RestHandler instance associated with the RestApp.
 
         Returns:
-            App[Self]: An instance of App.
+            RestHandler: An instance of RestHandler.
         """
+        return self.__rest_handler
```

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py` & `superlinked-5.2.2/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,17 +35,16 @@
 from superlinked.framework.evaluator.online_dag_evaluator import OnlineDagEvaluator
 from superlinked.framework.online.source.in_memory_data_processor import (
     InMemoryDataProcessor,
 )
 from superlinked.framework.online.source.in_memory_object_writer import (
     InMemoryObjectWriter,
 )
-from superlinked.framework.storage.in_memory_entity_store import InMemoryEntityStore
-from superlinked.framework.storage.in_memory_object_store import InMemoryObjectStore
-from superlinked.framework.storage.persistable_dict import ObjectReader, ObjectWriter
+from superlinked.framework.storage.in_memory.in_memory_vdb import InMemoryVDB
+from superlinked.framework.storage.in_memory.object_serializer import ObjectSerializer
 
 
 class InMemoryExecutor(Executor[InMemorySource]):
     """
     In-memory implementation of the Executor class. Supply it with the sources through which
     your data is received, and the indices indicating the desired vector spaces, and the executor will
     create the spaces optimized for search.
@@ -84,42 +83,47 @@
         Returns:
             InMemoryApp: An instance of InMemoryApp.
         """
         return InMemoryApp(self)
 
 
 @TypeValidator.wrap
-class InMemoryApp(App[InMemoryExecutor, InMemoryEntityStore, InMemoryObjectStore]):
+class InMemoryApp(App[InMemoryExecutor, InMemoryVDB]):
     """
     In-memory implementation of the App class.
 
     Attributes:
         executor (InMemoryExecutor): An instance of InMemoryExecutor.
     """
 
     def __init__(self, executor: InMemoryExecutor) -> None:
         """
         Initialize the InMemoryApp from an InMemoryExecutor.
 
         Args:
             executor (InMemoryExecutor): An instance of InMemoryExecutor.
         """
-        super().__init__(executor, InMemoryEntityStore(), InMemoryObjectStore())
-        self._object_writer = InMemoryObjectWriter(self._object_store_manager)
+        super().__init__(
+            executor,
+            InMemoryVDB(),
+        )
+        for index in self.executor._indices:
+            self.storage_manager.create_search_index(index._dag)
+        self._object_writer = InMemoryObjectWriter(self._storage_manager)
         self._index_online_dag_evaluator_map = {
             index: OnlineDagEvaluator(
                 index._dag,
                 set(index._space_schemas).union(index._effect_schemas),
-                self._entity_store_manager,
+                self._storage_manager,
             )
             for index in self.executor._indices
         }
         self._index_query_vector_factory_map = {
             index: QueryVectorFactory(
-                index._dag, set(index._space_schemas), self._entity_store_manager
+                index._dag, set(index._space_schemas), self._storage_manager
             )
             for index in self.executor._indices
         }
         self._data_processors = [
             InMemoryDataProcessor(
                 self._index_online_dag_evaluator_map[index], executor._context, index
             )
@@ -129,25 +133,23 @@
             source._source.register(self._object_writer)
         for data_processor, index in zip(
             self._data_processors, self._executor._indices
         ):
             for source in self.__filter_index_sources(index, self._executor._sources):
                 source._source.register(data_processor)
 
-    def restore(self, reader: ObjectReader) -> None:
+    def restore(self, serializer: ObjectSerializer) -> None:
         node_ids = [index._node_id for index in self.executor._indices]
         app_identifier = "_".join(node_ids)
-        self._object_store.restore(reader, app_identifier)
-        self._entity_store.restore(reader, app_identifier)
+        self._vdb_connector.restore(serializer, app_identifier)
 
-    def persist(self, writer: ObjectWriter) -> None:
+    def persist(self, serializer: ObjectSerializer) -> None:
         node_ids = [index._node_id for index in self.executor._indices]
         app_identifier = "_".join(node_ids)
-        self._object_store.persist(writer, app_identifier)
-        self._entity_store.persist(writer, app_identifier)
+        self._vdb_connector.persist(serializer, app_identifier)
 
     def query(self, query_obj: QueryObj, **params: Any) -> Result:
         """
         Execute a query. Example:
         ```
         query = (
             Query(relevance_index, weights=[{"relevance_space": Param("relevance_weight")}])
```

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/executor/query/query_executor.py` & `superlinked-5.2.2/superlinked/framework/dsl/executor/query/query_executor.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,34 +10,40 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Any
 
+from beartype.typing import Sequence
+
 from superlinked.framework.common.dag.context import (
     CONTEXT_COMMON,
     CONTEXT_COMMON_NOW,
     ExecutionContext,
     ExecutionEnvironment,
     NowStrategy,
 )
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.exception import QueryException
+from superlinked.framework.common.schema.id_schema_object import IdSchemaObject
+from superlinked.framework.common.storage_manager.knn_search_params import (
+    KNNSearchParams,
+)
+from superlinked.framework.common.storage_manager.search_result_item import (
+    SearchResultItem,
+)
 from superlinked.framework.common.util import time_util
 from superlinked.framework.dsl.executor.executor import App
 from superlinked.framework.dsl.query.param_evaluator import ParamEvaluator
 from superlinked.framework.dsl.query.query import QueryObj
 from superlinked.framework.dsl.query.query_filters import QueryFilters
 from superlinked.framework.dsl.query.query_vector_factory import QueryVectorFactory
 from superlinked.framework.dsl.query.result import Result, ResultEntry
 from superlinked.framework.dsl.space.space import Space
-from superlinked.framework.storage.entity import Entity
-from superlinked.framework.storage.entity_store_manager import EntityId
-from superlinked.framework.storage.object_store_manager import DataId
 
 
 class QueryExecutor:
     """
     QueryExecutor provides an interface to execute predefined queries with query time parameters.
     """
 
@@ -73,19 +79,20 @@
             QueryException: If the query index is not amongst the executor's indices.
         """
         self.__check_executor_has_index()
         param_evaluator = ParamEvaluator(params)
         limit = param_evaluator.evaluate_limit_param(self.query_obj.limit_)
         radius = param_evaluator.evaluate_radius_param(self.query_obj.radius_)
         # TODO FAI-1838 use self.query_obj.hard_filters in self._knn_search
-        entities: list[Entity] = self._knn(
+        entities: Sequence[SearchResultItem] = self._knn(
             self._get_query_vector(param_evaluator), limit, radius
         )
         return Result(
-            self.query_obj.schema, self._map_entities_to_result_entries(entities)
+            self.query_obj.schema,
+            self._map_entities_to_result_entries(self.query_obj.schema, entities),
         )
 
     def _get_query_vector(self, param_evaluator: ParamEvaluator) -> Vector:
         query_filters = self._create_query_filters(param_evaluator)
         space_weight_map = self.__get_space_weight_map(param_evaluator)
         return self.query_vector_factory.produce_vector(
             self.query_obj.index._node_id,
@@ -107,41 +114,42 @@
         eval_context.update_data(
             {CONTEXT_COMMON: {CONTEXT_COMMON_NOW: self.__query_now()}}
         )
         return eval_context
 
     def _knn(
         self, vector: Vector, limit: int | None, radius: float | None
-    ) -> list[Entity]:
-        return self.app.entity_store_manager.knn(
-            self.query_obj.index._node_id,
-            vector,
-            self.query_obj.schema._schema_name,
-            limit,
-            radius,
+    ) -> Sequence[SearchResultItem]:
+        return self.app.storage_manager.knn_search(
+            self.query_obj.index._node,
+            self.query_obj.schema,
+            [],
+            KNNSearchParams(vector=vector, limit=limit, radius=radius),
         )
 
     def _map_entities_to_result_entries(
-        self, entities: list[Entity]
-    ) -> list[ResultEntry]:
+        self, schema: IdSchemaObject, result_items: Sequence[SearchResultItem]
+    ) -> Sequence[ResultEntry]:
         return [
             ResultEntry(
                 entity,
-                self._get_stored_object_or_raise(entity.origin_id or entity.id_),
+                self._get_stored_object_or_raise(
+                    schema, entity.header.origin_id or entity.header.object_id
+                ),
             )
-            for entity in entities
+            for entity in result_items
         ]
 
-    def _get_stored_object_or_raise(self, entity_id: EntityId) -> dict[str, Any]:
-        stored_object = self.app.object_store_manager.load(
-            DataId(entity_id.schema_id, entity_id.object_id)
-        )
+    def _get_stored_object_or_raise(
+        self, schema: IdSchemaObject, object_id: str
+    ) -> dict[str, Any]:
+        stored_object = self.app.storage_manager.read_object_blob(schema, object_id)
         if not stored_object:
             raise QueryException(
-                f"No stored object found for the given entity_id: {entity_id}"
+                f"No stored {schema._schema_name} object found for the given object_id: {object_id}"
             )
         return stored_object
 
     def __check_executor_has_index(self) -> None:
         if self.query_obj.index not in self.app.executor._indices:
             raise QueryException(
                 f"Query index {self.query_obj.index} is not amongst "
```

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/executor/rest/rest_configuration.py` & `superlinked-5.2.2/superlinked/framework/dsl/executor/rest/rest_configuration.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/executor/rest/rest_descriptor.py` & `superlinked-5.2.2/superlinked/framework/dsl/executor/rest/rest_descriptor.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/executor/rest/rest_executor.py` & `superlinked-5.2.2/superlinked/framework/dsl/executor/executor.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,118 +10,115 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from typing import Mapping
+from abc import ABC, abstractmethod
+from typing import Annotated, Any, Generic, TypeVar
 
-from superlinked.framework.common.dag.context import ContextValue
-from superlinked.framework.dsl.executor.executor import App, Executor
-from superlinked.framework.dsl.executor.in_memory.in_memory_executor import (
-    InMemoryApp,
-    InMemoryExecutor,
-)
-from superlinked.framework.dsl.executor.rest.rest_configuration import (
-    RestEndpointConfiguration,
-    RestQuery,
-)
-from superlinked.framework.dsl.executor.rest.rest_handler import RestHandler
+from beartype.typing import Sequence
+from typing_extensions import Self
+
+from superlinked.framework.common.dag.context import ExecutionContext
+from superlinked.framework.common.storage.vdb_connector import VDBConnector
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
+from superlinked.framework.common.util.generic_class_util import GenericClassUtil
+from superlinked.framework.common.util.time_util import now
+from superlinked.framework.common.util.type_validator import TypeValidator
 from superlinked.framework.dsl.index.index import Index
-from superlinked.framework.dsl.source.rest_source import RestSource
+from superlinked.framework.dsl.source.source import SourceT
 
+ExecutorT = TypeVar("ExecutorT", bound="Executor")
+VDBConnectorT = TypeVar("VDBConnectorT", bound=VDBConnector)
 
-class RestExecutor(Executor[RestSource]):
-    """
-    The RestExecutor is a subclass of the Executor base class. It encapsulates all the parameters required for
-    the REST application. It also instantiates an InMemoryExecutor for data storage purposes.
 
-    Attributes:
-        sources (list[RestSource]): List of Rest sources that has information about the schema.
-        indices (list[Index]): List indices.
-        queries (list[RestQuery]): List of executable queries.
-        endpoint_configuration (RestEndpointConfiguration): Optional configuration for REST endpoints.
+class App(ABC, Generic[ExecutorT, VDBConnectorT]):
+    """
+    Abstract base class for an App, a running executor that can for example do queries or ingest data.
     """
 
     def __init__(
         self,
-        sources: list[RestSource],
-        indices: list[Index],
-        queries: list[RestQuery],
-        endpoint_configuration: RestEndpointConfiguration | None = None,
-        context_data: Mapping[str, Mapping[str, ContextValue]] | None = None,
-    ):
-        """
-        Initialize the RestExecutor.
-
-        Attributes:
-            sources (list[RestSource]): List of Rest sources that has information about the schema.
-            indices (list[Index]): List indices.
-            queries (list[RestQuery]): List of executable queries.
-            endpoint_configuration (RestEndpointConfiguration): Optional configuration for REST endpoints.
-        """
-        online_sources = [source._online_source for source in sources]
-        self._online_executor = InMemoryExecutor(online_sources, indices, context_data)
-        super().__init__(sources, indices, self._online_executor.context)
-
-        self._queries = queries
-        self._endpoint_configuration = (
-            endpoint_configuration or RestEndpointConfiguration()
-        )
+        executor: ExecutorT,
+        vdb_connector: VDBConnectorT,
+    ) -> None:
+        """
+        Initialize the App.
+
+        Args:
+            executor (TExecutor): The executor instance.
+            entity_store (EntityStore): The entity store instance.
+            object_store (ObjectStore): The object store instance.
+        """
+        self._executor = executor
+        self._vdb_connector = vdb_connector
+        self._storage_manager = StorageManager(self._vdb_connector)
+        self.now = now()
+
+    @property
+    def executor(self) -> ExecutorT:
+        """
+        Get the executor.
 
-    def run(self) -> RestApp:
+        Returns:
+            ExecutorT: The executor instance.
         """
-        Run the RestExecutor. It returns an app that will create rest endpoints.
+        return self._executor
+
+    @property
+    def storage_manager(self) -> StorageManager:
+        """
+        Get the storage manager.
 
         Returns:
-            RestApp: An instance of RestApp.
+            StorageManager: The storage manager instance.
         """
-        return RestApp(self)
+        return self._storage_manager
 
 
-class RestApp(App):
+class Executor(ABC, Generic[SourceT]):
     """
-    Rest implementation of the App class.
-
-    Attributes:
-        executor (RestExecutor): An instance of RestExecutor.
+    Abstract base class for an executor.
     """
 
-    def __init__(self, executor: RestExecutor):
+    @TypeValidator.wrap
+    def __init__(
+        self,
+        sources: Sequence[SourceT],
+        indices: Annotated[Sequence[Index], TypeValidator.list_validator(Index)],
+        context: ExecutionContext,
+    ) -> None:
         """
-        Initialize the RestApp from an RestExecutor.
+        Initialize the Executor.
 
         Args:
-            executor (RestExecutor): An instance of RestExecutor.
+            sources (list[SourceT]): The list of sources.
+            indices (list[Index]): The list of indices.
+            context (Mapping[str, Mapping[str, Any]]): The context mapping.
         """
-        self.__online_app = executor._online_executor.run()
-        super().__init__(
-            executor, self.__online_app._entity_store, self.__online_app._object_store
-        )
-
-        self.__rest_handler = RestHandler(
-            self.__online_app,
-            executor._sources,
-            executor._queries,
-            executor._endpoint_configuration,
+        TypeValidator.validate_list_item_type(
+            sources, GenericClassUtil.get_single_generic_type(self), "sources"
         )
+        self._sources = sources
+        self._indices = indices
+        self._context = context
 
     @property
-    def online_app(self) -> InMemoryApp:
+    def context(self) -> ExecutionContext:
         """
-        Property that returns the InMemoryApp instance associated with the RestApp.
+        Get the context.
 
         Returns:
-            InMemoryApp: An instance of InMemoryApp.
+            Mapping[str, Mapping[str, Any]]: The context mapping.
         """
-        return self.__online_app
+        return self._context
 
-    @property
-    def handler(self) -> RestHandler:
+    @abstractmethod
+    def run(self) -> App[Self, Any]:
         """
-        Property that returns the RestHandler instance associated with the RestApp.
+        Abstract method to run the executor.
 
         Returns:
-            RestHandler: An instance of RestHandler.
+            App[Self, Any]: An instance of App.
         """
-        return self.__rest_handler
```

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/executor/rest/rest_handler.py` & `superlinked-5.2.2/superlinked/framework/dsl/executor/rest/rest_handler.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/index/effect.py` & `superlinked-5.2.2/superlinked/framework/dsl/index/effect.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/index/index.py` & `superlinked-5.2.2/superlinked/framework/dsl/index/index.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/index/util/aggregation_effect_group.py` & `superlinked-5.2.2/superlinked/framework/dsl/index/util/aggregation_effect_group.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/index/util/aggregation_node_util.py` & `superlinked-5.2.2/superlinked/framework/dsl/index/util/aggregation_node_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py` & `superlinked-5.2.2/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py` & `superlinked-5.2.2/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/index/util/event_aggregation_node_util.py` & `superlinked-5.2.2/superlinked/framework/dsl/index/util/event_aggregation_node_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/query/param.py` & `superlinked-5.2.2/superlinked/framework/dsl/query/param.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/query/param_evaluator.py` & `superlinked-5.2.2/superlinked/framework/dsl/query/param_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/query/predicate/binary_op.py` & `superlinked-5.2.2/superlinked/framework/dsl/query/predicate/binary_op.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/query/predicate/binary_predicate.py` & `superlinked-5.2.2/superlinked/framework/dsl/query/predicate/binary_predicate.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/query/predicate/evaluated_binary_predicate.py` & `superlinked-5.2.2/superlinked/framework/dsl/query/predicate/evaluated_binary_predicate.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/query/predicate/query_predicate.py` & `superlinked-5.2.2/superlinked/framework/common/storage/entity_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,27 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from dataclasses import dataclass
-from enum import Enum
-from typing import Generic, TypeVar
-
-from superlinked.framework.common.schema.schema_object import SchemaField
-from superlinked.framework.dsl.query.param import NumericParamType, Param
 
-# Exclude from documentation.
-__pdoc__ = {}
-__pdoc__["QueryPredicate"] = False
+from dataclasses import dataclass
 
-# Operation type
-OPT = TypeVar("OPT", bound=Enum)
+from superlinked.framework.common.storage.entity_id import EntityId
+from superlinked.framework.common.storage.field_data import FieldData
 
 
 @dataclass(frozen=True)
-class QueryPredicate(Generic[OPT]):
-    op: OPT
-    params: list[SchemaField | Param | str | int | float | None]
-    weight_param: NumericParamType
+class EntityData:
+    id_: EntityId
+    field_data: dict[str, FieldData]
```

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/query/query.py` & `superlinked-5.2.2/superlinked/framework/dsl/query/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 )
 from superlinked.framework.common.interface.comparison_operation_type import (
     ComparisonOperationType,
 )
 from superlinked.framework.common.schema.id_schema_object import IdSchemaObject
 from superlinked.framework.common.schema.schema import T
 from superlinked.framework.common.schema.schema_object import SchemaField
-from superlinked.framework.common.util.type_util import get_single_generic_type
+from superlinked.framework.common.util.generic_class_util import GenericClassUtil
 from superlinked.framework.common.util.type_validator import TypeValidator
 from superlinked.framework.dsl.index.index import Index
 from superlinked.framework.dsl.query.param import (
     IntParamType,
     NumericParamType,
     Param,
     ParamType,
@@ -252,15 +252,18 @@
         Returns:
             Self: The query object itself.
         """
         if comparison_operation._op not in VALID_HARD_FILTER_TYPES:
             raise QueryException(
                 f"Unsupported filter operation: {comparison_operation._op}."
             )
-        allowed_types = [Param, get_single_generic_type(comparison_operation._operand)]
+        allowed_types = [
+            Param,
+            GenericClassUtil.get_single_generic_type(comparison_operation._operand),
+        ]
         if type(comparison_operation._other) not in allowed_types:
             raise QueryException(
                 f"Unsupported filter operand type: {comparison_operation._other.__class__.__name__}."
             )
         hard_filters = self.hard_filters.copy()
         hard_filters.append(comparison_operation)
         return self.__alter({"hard_filters": hard_filters})
```

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/query/query_filters.py` & `superlinked-5.2.2/superlinked/framework/dsl/query/query_filters.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/query/query_vector_factory.py` & `superlinked-5.2.2/superlinked/framework/dsl/query/query_vector_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,35 +26,34 @@
 from superlinked.framework.common.exception import QueryException
 from superlinked.framework.common.parser.parsed_schema import (
     ParsedSchema,
     ParsedSchemaField,
 )
 from superlinked.framework.common.schema.id_schema_object import IdSchemaObject
 from superlinked.framework.common.schema.schema_object import SchemaObject
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.dsl.query.query_filters import QueryFilters
 from superlinked.framework.dsl.query.query_weighting import QueryWeighting
 from superlinked.framework.dsl.space.space import Space
 from superlinked.framework.evaluator.query_dag_evaluator import QueryDagEvaluator
-from superlinked.framework.storage.entity import EntityId
-from superlinked.framework.storage.entity_store_manager import EntityStoreManager
 
 # Exclude from documentation.
 __pdoc__ = {}
 __pdoc__["QueryVectorFactory"] = False
 
 
 class QueryVectorFactory:
     def __init__(
         self,
         dag: Dag,
         schemas: set[SchemaObject],
-        entity_store_manager: EntityStoreManager,
+        storage_manager: StorageManager,
     ) -> None:
-        self._evaluator = QueryDagEvaluator(dag, schemas, entity_store_manager)
-        self._entity_store_manager = entity_store_manager
+        self._evaluator = QueryDagEvaluator(dag, schemas, storage_manager)
+        self._storage_manager = storage_manager
         self._query_weighting = QueryWeighting(dag)
 
     def produce_vector(
         self,
         index_node_id: str,
         query_filters: QueryFilters,
         global_space_weight_map: dict[Space, float],
@@ -89,20 +88,19 @@
     def _get_looks_like_vector(
         self,
         index_node_id: str,
         query_filters: QueryFilters,
     ) -> Vector | None:
         if looks_like_filter := query_filters.looks_like_filter:
             # search by the vector of the referenced entity
-            if _vector := self._entity_store_manager.get_vector(
-                EntityId(
-                    object_id=str(looks_like_filter.value),
-                    node_id=index_node_id,
-                    schema_id=looks_like_filter.predicate.left_param.schema_obj._schema_name,
-                )
+            if _vector := self._storage_manager.read_node_result(
+                looks_like_filter.predicate.left_param.schema_obj,
+                str(looks_like_filter.value),
+                index_node_id,
+                Vector,
             ):
                 _vector = _vector * looks_like_filter.weight
                 return cast(Vector, _vector)
 
             raise QueryException(
                 f"Entity not found object_id: {looks_like_filter.value} node_id: {index_node_id}"
             )
```

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/query/query_weighting.py` & `superlinked-5.2.2/superlinked/framework/dsl/query/query_weighting.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/query/result.py` & `superlinked-5.2.2/superlinked/framework/dsl/query/result.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,49 +11,52 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from dataclasses import dataclass
 from typing import Any
 
+from beartype.typing import Sequence
 from pandas import DataFrame
 
 from superlinked.framework.common.schema.id_schema_object import IdSchemaObject
-from superlinked.framework.storage.entity import Entity
+from superlinked.framework.common.storage_manager.search_result_item import (
+    SearchResultItem,
+)
 
 
 @dataclass(frozen=True)
 class ResultEntry:
     """
     Represents a single entry in a Result, encapsulating the entity and its associated data.
 
     Attributes:
-        entity (Entity): The entity of the result entry.
-            This is an instance of the Entity class, which represents a unique entity in the system.
-            It contains information such as the entity's ID and type.
+        entity (SearchResultItem): The entity of the result entry.
+            This is an instance of the SearchResultItem class, which represents a unique entity in the system.
+            It contains header information such as the entity's ID and schema and the queried fields.
         stored_object (dict[str, Any]): The stored object of the result entry.
             This is essentially the raw data that was input into the system.
     """
 
-    entity: Entity
+    entity: SearchResultItem
     stored_object: dict[str, Any]
 
 
 @dataclass(frozen=True)
 class Result:
     """
     A class representing the result of a query.
 
     Attributes:
         schema (IdSchemaObject): The schema of the result.
-        entries (list[ResultEntry]): A list of result entries.
+        entries (Sequence[ResultEntry]): A list of result entries.
     """
 
     schema: IdSchemaObject
-    entries: list[ResultEntry]
+    entries: Sequence[ResultEntry]
 
     def to_pandas(self) -> DataFrame:
         """
         Converts the query result entries into a pandas DataFrame.
 
         Each row in the DataFrame corresponds to a single entity in the result, with
         columns representing the fields of the stored objects.
@@ -62,10 +65,10 @@
             DataFrame: A pandas DataFrame where each row represents a result entity, and
                 each column corresponds to the fields of the stored objects.
         """
         return DataFrame([entry.stored_object for entry in self.entries])
 
     def __str__(self) -> str:
         return "\n".join(
-            f"#{i+1} id:{entry.entity.id_.object_id}, object:{entry.stored_object}"
+            f"#{i+1} id:{entry.entity.header.object_id}, object:{entry.stored_object}"
             for i, entry in enumerate(self.entries)
         )
```

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/registry/exception.py` & `superlinked-5.2.2/superlinked/framework/online/dag/batched_chunk_input_item.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,10 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from dataclasses import dataclass
 
-class DuplicateElementException(Exception):
-    pass
+from superlinked.framework.online.dag.parent_results import ParentResults
+
+
+@dataclass(frozen=True)
+class BatchedChunkInputItem:
+    parsed_schema_index: int
+    input_: ParentResults
```

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/source/in_memory_source.py` & `superlinked-5.2.2/superlinked/framework/dsl/source/in_memory_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/source/rest_source.py` & `superlinked-5.2.2/superlinked/framework/dsl/source/rest_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/source/source.py` & `superlinked-5.2.2/superlinked/framework/dsl/source/source.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/space/categorical_similarity_space.py` & `superlinked-5.2.2/superlinked/framework/dsl/space/categorical_similarity_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/space/custom_space.py` & `superlinked-5.2.2/superlinked/framework/dsl/space/custom_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/space/exception.py` & `superlinked-5.2.2/superlinked/framework/dsl/space/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/space/number_space.py` & `superlinked-5.2.2/superlinked/framework/dsl/space/number_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/space/recency_space.py` & `superlinked-5.2.2/superlinked/framework/dsl/space/recency_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/space/space.py` & `superlinked-5.2.2/superlinked/framework/dsl/space/space.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/space/space_field_set.py` & `superlinked-5.2.2/superlinked/framework/dsl/space/space_field_set.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/dsl/space/text_similarity_space.py` & `superlinked-5.2.2/superlinked/framework/dsl/space/text_similarity_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/evaluator/dag_evaluator.py` & `superlinked-5.2.2/superlinked/framework/evaluator/dag_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/evaluator/online_dag_evaluator.py` & `superlinked-5.2.2/superlinked/framework/evaluator/online_dag_evaluator.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,48 +19,40 @@
 from superlinked.framework.common.exception import (
     InvalidDagEffectException,
     InvalidSchemaException,
 )
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
 from superlinked.framework.common.schema.id_schema_object import IdSchemaObject
 from superlinked.framework.common.schema.schema_object import SchemaObject
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.compiler.online_schema_dag_compiler import (
     OnlineSchemaDagCompiler,
 )
 from superlinked.framework.evaluator.dag_evaluator import DagEvaluator
 from superlinked.framework.online.dag.evaluation_result import EvaluationResult
 from superlinked.framework.online.dag.online_schema_dag import OnlineSchemaDag
-from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
-    EvaluationResultStoreManager,
-)
-from superlinked.framework.storage.entity_store_manager import EntityStoreManager
 
 
 class OnlineDagEvaluator(DagEvaluator[EvaluationResult[Vector]]):
     def __init__(
         self,
         dag: Dag,
         schemas: set[SchemaObject],
-        entity_store_manager: EntityStoreManager,
+        storage_manager: StorageManager,
     ) -> None:
         super().__init__()
         self._dag = dag
         self._schemas = schemas
-        self._evaluation_result_store_manager = EvaluationResultStoreManager(
-            entity_store_manager
-        )
         self._schema_online_schema_dag_mapper = (
             self.__init_schema_online_schema_dag_mapper(
-                self._schemas, self._dag, self._evaluation_result_store_manager
+                self._schemas, self._dag, storage_manager
             )
         )
         self._dag_effect_online_schema_dag_mapper = (
-            self.__init_dag_effect_online_schema_dag_mapper(
-                self._dag, self._evaluation_result_store_manager
-            )
+            self.__init_dag_effect_online_schema_dag_mapper(self._dag, storage_manager)
         )
 
     def __get_single_schema(self, parsed_schemas: list[ParsedSchema]) -> IdSchemaObject:
         unique_schemas: set[IdSchemaObject] = {
             parsed_schema.schema for parsed_schema in parsed_schemas
         }
         if len(unique_schemas) != 1:
@@ -99,33 +91,33 @@
             f"DagEffect ({dag_effect}) isn't present in the index."
         )
 
     def __init_schema_online_schema_dag_mapper(
         self,
         schemas: set[SchemaObject],
         dag: Dag,
-        evaluation_result_store_manager: EvaluationResultStoreManager,
+        storage_manager: StorageManager,
     ) -> dict[SchemaObject, OnlineSchemaDag]:
         return {
             schema: OnlineSchemaDagCompiler(set(dag.nodes)).compile_schema_dag(
                 dag.project_to_schema(schema),
-                evaluation_result_store_manager,
+                storage_manager,
             )
             for schema in schemas
         }
 
     def __init_dag_effect_online_schema_dag_mapper(
-        self, dag: Dag, evaluation_result_store_manager: EvaluationResultStoreManager
+        self, dag: Dag, storage_manager: StorageManager
     ) -> dict[DagEffect, OnlineSchemaDag]:
         dag_effect_schema_dag_map = {
             dag_effect: dag.project_to_dag_effect(dag_effect)
             for dag_effect in dag.dag_effects
         }
         return {
             dag_effect: OnlineSchemaDagCompiler(
                 set(schema_dag.nodes)
             ).compile_schema_dag(
                 schema_dag,
-                evaluation_result_store_manager,
+                storage_manager,
             )
             for dag_effect, schema_dag in dag_effect_schema_dag_map.items()
         }
```

### Comparing `superlinked-4.1.0/superlinked/framework/evaluator/query_dag_evaluator.py` & `superlinked-5.2.2/superlinked/framework/evaluator/query_dag_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/new_storage/in_memory/exception.py` & `superlinked-5.2.2/superlinked/framework/storage/in_memory/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/new_storage/in_memory/in_memory_knn_search.py` & `superlinked-5.2.2/superlinked/framework/storage/in_memory/in_memory_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,56 +24,69 @@
 from superlinked.framework.common.exception import ValidationException
 from superlinked.framework.common.interface.comparison_operand import (
     ComparisonOperation,
 )
 from superlinked.framework.common.storage.field import Field
 from superlinked.framework.common.storage.field_data import VectorFieldData
 from superlinked.framework.common.storage.vdb_knn_search_params import (
-    VDBKnnSearchParams,
+    VDBKNNSearchParams,
 )
-from superlinked.framework.new_storage.in_memory.exception import (
+from superlinked.framework.storage.in_memory.exception import (
     VectorFieldDimensionException,
     VectorFieldTypeException,
 )
-from superlinked.framework.new_storage.in_memory.index_config import IndexConfig
+from superlinked.framework.storage.in_memory.index_config import IndexConfig
 
 
-class InMemoryKnnSearch:
+class InMemorySearch:
     def search(
         self,
+        vdb: defaultdict[str, dict[str, Any]],
+        filters: Sequence[ComparisonOperation[Field]],
+        has_fields: Sequence[Field],
+    ) -> Sequence[str]:
+        return [
+            row_id
+            for row_id, values in vdb.items()
+            if InMemorySearch._is_subset(values, filters, has_fields)
+        ]
+
+    def knn_search(
+        self,
         index_config: IndexConfig,
         vdb: defaultdict[str, dict[str, Any]],
-        search_params: VDBKnnSearchParams,
-    ) -> list[str]:
-        self._check_vector_field_name(index_config, search_params.vector_field)
+        search_params: VDBKNNSearchParams,
+    ) -> list[tuple[str, float]]:
+        self._check_vector_field(index_config, search_params.vector_field)
         self._check_filters(index_config, search_params.filters)
         filtered_vectors = self._filter_indexed_vectors(
-            vdb, search_params.vector_field, search_params.filters
+            vdb,
+            search_params.vector_field,
+            search_params.filters,
         )
         similarities = self._calculate_similarities(
             index_config.vector_similarity_calculator,
-            search_params.vector_field,
+            search_params.vector_field.value,
             filtered_vectors,
         )
         sorted_similarities = self._sort_similarities(
             similarities,
             search_params.radius,
         )
-        return [
-            row_id
-            for row_id, _ in (
-                sorted_similarities[: search_params.limit]
-                if search_params.limit
-                else sorted_similarities
-            )
-        ]
+        return (
+            sorted_similarities[: search_params.limit]
+            if search_params.limit
+            else sorted_similarities
+        )
 
-    def _check_vector_field_name(
+    def _check_vector_field(
         self, index_config: IndexConfig, vector_field: VectorFieldData
     ) -> None:
+        if vector_field.value is None:
+            raise ValidationException("Cannot search with none-type vector!")
         if index_config.vector_field_name != vector_field.name:
             raise ValidationException(
                 f"Indexed {index_config.vector_field_name} and"
                 + f" searched {vector_field.name} vectors are different!"
             )
 
     def _check_filters(
@@ -94,20 +107,20 @@
         vdb: dict[str, dict[str, Any]],
         vector_field: VectorFieldData,
         filters: Sequence[ComparisonOperation[Field]] | None,
     ) -> dict[str, Vector]:
         filtered_unchecked_vectors = {
             row_id: values[vector_field.name]
             for row_id, values in vdb.items()
-            if InMemoryKnnSearch._is_subset(values, filters or [])
+            if InMemorySearch._is_subset(values, filters or [])
             and values.get(vector_field.name) is not None
         }
         filtered_vectors = self._validate_filtered_vectors(
             filtered_unchecked_vectors,
-            vector_field.value,
+            cast(Vector, vector_field.value),
         )
         return filtered_vectors
 
     def _validate_filtered_vectors(
         self, filtered_unchecked_vectors: dict[str, Any], vector: Vector
     ) -> dict[str, Vector]:
         if wrong_types := {
@@ -127,22 +140,22 @@
                 f"Indexed vector field contains vectors with wrong dimensions: {wrong_dimensions}"
             )
         return cast(dict[str, Vector], filtered_unchecked_vectors)
 
     def _calculate_similarities(
         self,
         vector_similarity_calculator: VectorSimilarityCalculator,
-        vector_field: VectorFieldData,
+        vector: Vector,
         filtered_vectors: dict[str, Vector],
     ) -> dict[str, float]:
         return {
             row_id: vector_similarity_calculator.calculate_similarity(
-                vector, vector_field.value
+                filtered_vector, vector
             )
-            for row_id, vector in filtered_vectors.items()
+            for row_id, filtered_vector in filtered_vectors.items()
         }
 
     def _sort_similarities(
         self,
         similarities: dict[str, float],
         radius: float | None,
     ) -> list[tuple[str, float]]:
@@ -156,17 +169,20 @@
             reverse=True,
         )
 
     @staticmethod
     def _is_subset(
         raw_entity: dict[str, Any],
         filters: Sequence[ComparisonOperation[Field]],
+        has_fields: Sequence[Field] | None = None,
     ) -> bool:
         """
         Return true, if all filters are True to the entity.
         """
-        if not filters:
+        if not (filters or has_fields):
             return True
         return all(
             filter_.evaluate(raw_entity.get(cast(Field, filter_._operand).name))
             for filter_ in filters
+        ) and all(
+            raw_entity.get(filter_.name) is not None for filter_ in has_fields or []
         )
```

### Comparing `superlinked-4.1.0/superlinked/framework/new_storage/in_memory/in_memory_vdb.py` & `superlinked-5.2.2/superlinked/framework/storage/in_memory/in_memory_vdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,49 +19,46 @@
 from beartype.typing import Sequence
 from typing_extensions import override
 
 from superlinked.framework.common.calculation.vector_similarity import (
     VectorSimilarityCalculator,
 )
 from superlinked.framework.common.exception import ValidationException
+from superlinked.framework.common.interface.comparison_operand import (
+    ComparisonOperation,
+)
 from superlinked.framework.common.storage.entity import Entity
 from superlinked.framework.common.storage.entity_data import EntityData
 from superlinked.framework.common.storage.entity_id import EntityId
 from superlinked.framework.common.storage.field import Field
 from superlinked.framework.common.storage.field_data import FieldData
+from superlinked.framework.common.storage.result_entity_data import ResultEntityData
 from superlinked.framework.common.storage.search_index_creation.index_field_descriptor import (
     IndexFieldDescriptor,
     VectorIndexFieldDescriptor,
 )
 from superlinked.framework.common.storage.search_index_creation.search_algorithm import (
     SearchAlgorithm,
 )
 from superlinked.framework.common.storage.vdb_connector import VDBConnector
 from superlinked.framework.common.storage.vdb_knn_search_params import (
-    VDBKnnSearchParams,
-)
-from superlinked.framework.new_storage.in_memory.in_memory_knn_search import (
-    InMemoryKnnSearch,
-)
-from superlinked.framework.new_storage.in_memory.index_config import IndexConfig
-from superlinked.framework.new_storage.in_memory.json_codec import (
-    JsonDecoder,
-    JsonEncoder,
-)
-from superlinked.framework.new_storage.in_memory.object_serializer import (
-    ObjectSerializer,
+    VDBKNNSearchParams,
 )
+from superlinked.framework.storage.in_memory.in_memory_search import InMemorySearch
+from superlinked.framework.storage.in_memory.index_config import IndexConfig
+from superlinked.framework.storage.in_memory.json_codec import JsonDecoder, JsonEncoder
+from superlinked.framework.storage.in_memory.object_serializer import ObjectSerializer
 
 
 class InMemoryVDB(VDBConnector):
     def __init__(self) -> None:
         super().__init__()
         self._vdb = defaultdict[str, dict[str, Any]](dict)
         self._index_configs: dict[str, IndexConfig] = {}
-        self._knn_search = InMemoryKnnSearch()
+        self._search = InMemorySearch()
 
     @override
     def close_connection(self) -> None:
         self._vdb = defaultdict[str, dict[str, Any]](dict)
         self._index_configs = dict[str, IndexConfig]()
 
     @override
@@ -90,50 +87,71 @@
         return [SearchAlgorithm.FLAT]
 
     @override
     def write_entities(self, entity_data: Sequence[EntityData]) -> None:
         for ed in entity_data:
             row_id = InMemoryVDB._get_row_id_from_entity_id(ed.id_)
             self._vdb[row_id].update(
-                {field_data.name: field_data.value for field_data in ed.field_data}
+                {name: fd.value for name, fd in ed.field_data.items()}
             )
 
     @override
     def read_entities(self, entities: Sequence[Entity]) -> Sequence[EntityData]:
         return [
             EntityData(
                 entity.id_,
-                [
-                    FieldData.from_field(
-                        field,
-                        self._vdb[
-                            InMemoryVDB._get_row_id_from_entity_id(entity.id_)
-                        ].get(field.name),
-                    )
-                    for field in entity.fields
-                ],
+                self._find_field_data(
+                    InMemoryVDB._get_row_id_from_entity_id(entity.id_),
+                    list(entity.fields.values()),
+                ),
             )
             for entity in entities
         ]
 
+    def _find_field_data(
+        self, row_id: str, fields: Sequence[Field]
+    ) -> dict[str, FieldData]:
+        raw_entity = self._vdb[row_id]
+        return {
+            field.name: FieldData.from_field(field, raw_entity.get(field.name))
+            for field in fields
+            if raw_entity.get(field.name) is not None
+        }
+
+    def read_entities_matching_filters(
+        self,
+        filters: Sequence[ComparisonOperation[Field]],
+        has_fields: Sequence[Field],
+        return_fields: Sequence[Field],
+    ) -> Sequence[EntityData]:
+        row_ids = self._search.search(self._vdb, filters, has_fields)
+        return [
+            EntityData(
+                InMemoryVDB._get_entity_id_from_row_id(row_id),
+                self._find_field_data(row_id, return_fields),
+            )
+            for row_id in row_ids
+        ]
+
     @override
     def knn_search(
         self,
         index_name: str,
         schema_name: str,
         returned_fields: Sequence[Field],
-        vdb_knn_search_params: VDBKnnSearchParams,
+        vdb_knn_search_params: VDBKNNSearchParams,
         **params: Any,
-    ) -> Sequence[EntityData]:
+    ) -> Sequence[ResultEntityData]:
         index_config = self._get_index_config(index_name)
-        sorted_row_ids: list[str] = self._knn_search.search(
+        sorted_scores: list[tuple[str, float]] = self._search.knn_search(
             index_config, self._vdb, vdb_knn_search_params
         )
         return [
-            self._get_entity_data(row_id, returned_fields) for row_id in sorted_row_ids
+            self._get_result_entity_data(row_id, score, returned_fields)
+            for row_id, score in sorted_scores
         ]
 
     def persist(self, serialzer: ObjectSerializer, app_identifier: str) -> None:
         serialzer.write(
             self.__class__.__name__,
             json.dumps(self._vdb, cls=JsonEncoder),
             app_identifier,
@@ -151,26 +169,21 @@
         index_config = self._index_configs.get(index_name)
         if not index_config:
             raise ValidationException(
                 f"Index with the given name {index_name} doesn't exist!"
             )
         return index_config
 
-    def _get_entity_data(
-        self, row_id: str, returned_fields: Sequence[Field]
-    ) -> EntityData:
-        raw_entity = self._vdb.get(row_id, {})
-        return EntityData(
+    def _get_result_entity_data(
+        self, row_id: str, score: float, returned_fields: Sequence[Field]
+    ) -> ResultEntityData:
+        return ResultEntityData(
             InMemoryVDB._get_entity_id_from_row_id(row_id),
-            [
-                FieldData.from_field(
-                    returned_field, raw_entity.get(returned_field.name)
-                )
-                for returned_field in returned_fields
-            ],
+            self._find_field_data(row_id, returned_fields),
+            score,
         )
 
     @staticmethod
     def _get_row_id_from_entity_id(entity_id: EntityId) -> str:
         return f"{entity_id.schema_id}:{entity_id.object_id}"
 
     @staticmethod
```

### Comparing `superlinked-4.1.0/superlinked/framework/new_storage/in_memory/index_config.py` & `superlinked-5.2.2/superlinked/framework/storage/in_memory/index_config.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/new_storage/in_memory/json_codec.py` & `superlinked-5.2.2/superlinked/framework/storage/in_memory/json_codec.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/new_storage/in_memory/object_serializer.py` & `superlinked-5.2.2/superlinked/framework/storage/in_memory/object_serializer.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/batched_chunk_input_item.py` & `superlinked-5.2.2/superlinked/framework/common/storage/result_entity_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+
 from dataclasses import dataclass
 
-from superlinked.framework.online.dag.parent_results import ParentResults
+from superlinked.framework.common.storage.entity_data import EntityData
 
 
 @dataclass(frozen=True)
-class BatchedChunkInputItem:
-    parsed_schema_index: int
-    input_: ParentResults
+class ResultEntityData(EntityData):
+    score: float
```

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/default_online_node.py` & `superlinked-5.2.2/superlinked/framework/online/dag/default_online_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/evaluation_result.py` & `superlinked-5.2.2/superlinked/framework/online/dag/evaluation_result.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import uuid
 from dataclasses import dataclass, field
 from typing import Generic, TypeVar
 
+from superlinked.framework.common.data_types import PythonTypes
+
 # EvaluationResultType
-ERT = TypeVar("ERT")
+ERT = TypeVar("ERT", bound=PythonTypes)
 
 
 @dataclass(frozen=True)
 class SingleEvaluationResult(Generic[ERT]):
     node_id: str
     value: ERT
     _object_id: str | None = None
```

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/exception.py` & `superlinked-5.2.2/superlinked/framework/online/dag/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/online_aggregation_node.py` & `superlinked-5.2.2/superlinked/framework/online/dag/online_aggregation_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,34 +27,32 @@
 from superlinked.framework.common.exception import (
     MismatchingDimensionException,
     ValidationException,
 )
 from superlinked.framework.common.interface.has_aggregation import HasAggregation
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.space.aggregation import Aggregation
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.online.dag.default_online_node import DefaultOnlineNode
 from superlinked.framework.online.dag.evaluation_result import SingleEvaluationResult
 from superlinked.framework.online.dag.online_node import OnlineNode
 from superlinked.framework.online.dag.parent_validator import ParentValidationType
-from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
-    EvaluationResultStoreManager,
-)
 
 
 class OnlineAggregationNode(DefaultOnlineNode[AggregationNode, Vector], HasLength):
     def __init__(
         self,
         node: AggregationNode,
         parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
+        storage_manager: StorageManager,
     ) -> None:
         super().__init__(
             node,
             parents,
-            evaluation_result_store_manager,
+            storage_manager,
             ParentValidationType.AT_LEAST_ONE_PARENT,
         )
         OnlineAggregationNode.__validate_parents(parents)
 
     @property
     def length(self) -> int:
         return self.node.length
```

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/online_categorical_similarity_node.py` & `superlinked-5.2.2/superlinked/framework/online/dag/online_categorical_similarity_node.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,35 +22,33 @@
     CategoricalSimilarityNode,
 )
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.online.dag.evaluation_result import EvaluationResult
 from superlinked.framework.online.dag.online_node import OnlineNode
 from superlinked.framework.online.dag.parent_validator import ParentValidationType
-from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
-    EvaluationResultStoreManager,
-)
 
 
 class OnlineCategoricalSimilarityNode(
     OnlineNode[CategoricalSimilarityNode, Vector], HasLength
 ):
     def __init__(
         self,
         node: CategoricalSimilarityNode,
         parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
+        storage_manager: StorageManager,
     ) -> None:
         super().__init__(
             node,
             parents,
-            evaluation_result_store_manager,
+            storage_manager,
             ParentValidationType.LESS_THAN_TWO_PARENTS,
         )
 
     @property
     def length(self) -> int:
         return self.node.length
```

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/online_chunking_node.py` & `superlinked-5.2.2/superlinked/framework/online/dag/online_chunking_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,34 +19,32 @@
 from typing_extensions import override
 
 from superlinked.framework.common.dag.chunking_node import ChunkingNode
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.embedding.chunking_util import Chunker
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.online.dag.evaluation_result import EvaluationResult
 from superlinked.framework.online.dag.exception import ChunkException
 from superlinked.framework.online.dag.online_node import OnlineNode
 from superlinked.framework.online.dag.parent_validator import ParentValidationType
-from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
-    EvaluationResultStoreManager,
-)
 
 
 class OnlineChunkingNode(OnlineNode[ChunkingNode, str]):
     def __init__(
         self,
         node: ChunkingNode,
         parents: list[OnlineNode[Node[str], str]],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
+        storage_manager: StorageManager,
     ) -> None:
         super().__init__(
             node,
             parents,
-            evaluation_result_store_manager,
+            storage_manager,
             ParentValidationType.EXACTLY_ONE_PARENT,
         )
 
     def __chunk(
         self,
         text: str,
         chunk_size: int | None,
```

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/online_comparison_filter_node.py` & `superlinked-5.2.2/superlinked/framework/online/dag/online_comparison_filter_node.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,34 +15,32 @@
 from __future__ import annotations
 
 from beartype.typing import Sequence
 from typing_extensions import override
 
 from superlinked.framework.common.dag.comparison_filter_node import ComparisonFilterNode
 from superlinked.framework.common.dag.context import ExecutionContext
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.online.dag.default_online_node import DefaultOnlineNode
 from superlinked.framework.online.dag.evaluation_result import SingleEvaluationResult
 from superlinked.framework.online.dag.online_node import OnlineNode
 from superlinked.framework.online.dag.parent_validator import ParentValidationType
-from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
-    EvaluationResultStoreManager,
-)
 
 
 class OnlineComparisonFilterNode(DefaultOnlineNode[ComparisonFilterNode, bool]):
     def __init__(
         self,
         node: ComparisonFilterNode,
         parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
+        storage_manager: StorageManager,
     ) -> None:
         super().__init__(
             node,
             parents,
-            evaluation_result_store_manager,
+            storage_manager,
             ParentValidationType.EXACTLY_ONE_PARENT,
         )
 
     @override
     def _evaluate_singles(
         self,
         parent_results: list[dict[OnlineNode, SingleEvaluationResult]],
```

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/online_concatenation_node.py` & `superlinked-5.2.2/superlinked/framework/online/dag/online_concatenation_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,34 +25,32 @@
 from superlinked.framework.common.dag.context import (
     SPACE_WEIGHT_PARAM_NAME,
     ExecutionContext,
 )
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.exception import ValidationException
 from superlinked.framework.common.interface.has_length import HasLength
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.online.dag.default_online_node import DefaultOnlineNode
 from superlinked.framework.online.dag.evaluation_result import SingleEvaluationResult
 from superlinked.framework.online.dag.online_node import OnlineNode
 from superlinked.framework.online.dag.parent_validator import ParentValidationType
-from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
-    EvaluationResultStoreManager,
-)
 
 
 class OnlineConcatenationNode(DefaultOnlineNode[ConcatenationNode, Vector], HasLength):
     def __init__(
         self,
         node: ConcatenationNode,
         parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
+        storage_manager: StorageManager,
     ) -> None:
         super().__init__(
             node,
             parents,
-            evaluation_result_store_manager,
+            storage_manager,
             ParentValidationType.AT_LEAST_ONE_PARENT,
         )
 
     @property
     def length(self) -> int:
         return self.node.length
```

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/online_constant_node.py` & `superlinked-5.2.2/superlinked/framework/online/dag/online_constant_node.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,33 +16,31 @@
 
 from typing_extensions import override
 
 from superlinked.framework.common.dag.constant_node import ConstantNode
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.node import NDT
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.online.dag.evaluation_result import EvaluationResult
 from superlinked.framework.online.dag.online_node import OnlineNode
 from superlinked.framework.online.dag.parent_validator import ParentValidationType
-from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
-    EvaluationResultStoreManager,
-)
 
 
 class OnlineConstantNode(OnlineNode[ConstantNode[NDT], NDT]):
     def __init__(
         self,
         node: ConstantNode,
         parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
+        storage_manager: StorageManager,
     ) -> None:
         super().__init__(
             node,
             parents,
-            evaluation_result_store_manager,
+            storage_manager,
             ParentValidationType.NO_PARENTS,
         )
 
     @override
     def evaluate_self(
         self,
         parsed_schemas: list[ParsedSchema],
```

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/online_custom_node.py` & `superlinked-5.2.2/superlinked/framework/online/dag/online_custom_node.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,46 +12,42 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from typing import cast
 
-import numpy as np
-import numpy.typing as npt
 from typing_extensions import override
 
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.custom_node import CustomVectorEmbeddingNode
 from superlinked.framework.common.dag.node import Node
-from superlinked.framework.common.data_types import Vector
+from superlinked.framework.common.data_types import NPArray, Vector
 from superlinked.framework.common.exception import ValidationException
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.online.dag.evaluation_result import EvaluationResult
 from superlinked.framework.online.dag.online_node import OnlineNode
 from superlinked.framework.online.dag.parent_validator import ParentValidationType
-from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
-    EvaluationResultStoreManager,
-)
 
 
 class OnlineCustomVectorEmbeddingNode(
     OnlineNode[CustomVectorEmbeddingNode, Vector], HasLength
 ):
     def __init__(
         self,
         node: CustomVectorEmbeddingNode,
         parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
+        storage_manager: StorageManager,
     ) -> None:
         super().__init__(
             node,
             parents,
-            evaluation_result_store_manager,
+            storage_manager,
             ParentValidationType.LESS_THAN_TWO_PARENTS,
         )
 
     @property
     def length(self) -> int:
         return self.node.length
 
@@ -68,16 +64,16 @@
         parsed_schema: ParsedSchema,
         context: ExecutionContext,
     ) -> EvaluationResult[Vector]:
         if len(self.parents) == 0:
             stored_result = self.load_stored_result_or_raise_exception(parsed_schema)
             return EvaluationResult(self._get_single_evaluation_result(stored_result))
 
-        input_: EvaluationResult[npt.NDArray[np.float64]] = cast(
-            OnlineNode[Node[Vector], npt.NDArray[np.float64]], self.parents[0]
+        input_: EvaluationResult[NPArray] = cast(
+            OnlineNode[Node[Vector], NPArray], self.parents[0]
         ).evaluate_next_single(parsed_schema, context)
         input_value = input_.main.value
         if len(input_value) != self.length:
             raise ValidationException(
                 f"{self.class_name} can only process `Vector` inputs"
                 + f" of size {self.length}"
                 + f", got {len(input_value)}"
```

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/online_event_aggregation_node.py` & `superlinked-5.2.2/superlinked/framework/online/dag/online_event_aggregation_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,34 +24,32 @@
 from superlinked.framework.common.exception import (
     DagEvaluationException,
     ValidationException,
 )
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
 from superlinked.framework.common.schema.schema_object import SchemaObject
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.online.dag.evaluation_result import EvaluationResult
 from superlinked.framework.online.dag.online_comparison_filter_node import (
     OnlineComparisonFilterNode,
 )
 from superlinked.framework.online.dag.online_node import OnlineNode
-from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
-    EvaluationResultStoreManager,
-)
 
 
 class OnlineEventAggregationNode(OnlineNode[EventAggregationNode, Vector], HasLength):
     EFFECT_COUNT_KEY = "effect_count"
 
     def __init__(
         self,
         node: EventAggregationNode,
         parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
+        storage_manager: StorageManager,
     ) -> None:
-        super().__init__(node, parents, evaluation_result_store_manager)
+        super().__init__(node, parents, storage_manager)
         self.__init_named_parents()
 
     def __init_named_parents(self) -> None:
         inputs_to_aggregate = [
             parent
             for parent in self.parents
             if parent.node.node_id == self.node.input_to_aggregate.node_id
@@ -188,32 +186,26 @@
             for field in event_parsed_schema.fields
             if field.schema_field == self.node.affecting_schema.reference_field
         )
 
     def __store_effect_count(
         self, main_object_id: str, schema: SchemaObject, count: int
     ) -> None:
-        self.evaluation_result_store_manager.save_result_meta(
-            EvaluationResultStoreManager.SaveResultMetaArgs(
-                main_object_id,
-                schema._schema_name,
-                self.node_id,
-                OnlineEventAggregationNode.EFFECT_COUNT_KEY,
-                str(count),
-            )
+        self.storage_manager.write_node_data(
+            schema,
+            main_object_id,
+            self.node_id,
+            {OnlineEventAggregationNode.EFFECT_COUNT_KEY: count},
         )
 
     def __load_effect_count(
         self,
         main_object_id: str,
         schema: SchemaObject,
     ) -> int:
-        count = int(
-            self.evaluation_result_store_manager.load_result_meta(
-                main_object_id,
-                schema._schema_name,
-                self.node_id,
-                OnlineEventAggregationNode.EFFECT_COUNT_KEY,
-            )
-            or 0
+        node_data = self.storage_manager.read_node_data(
+            schema,
+            main_object_id,
+            self.node_id,
+            {OnlineEventAggregationNode.EFFECT_COUNT_KEY: int},
         )
-        return count
+        return node_data.get(OnlineEventAggregationNode.EFFECT_COUNT_KEY) or 0
```

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/online_index_node.py` & `superlinked-5.2.2/superlinked/framework/online/dag/online_index_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,32 +22,30 @@
 from superlinked.framework.common.dag.exception import ParentCountException
 from superlinked.framework.common.dag.index_node import IndexNode
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
 from superlinked.framework.common.schema.schema_object import SchemaObject
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.online.dag.evaluation_result import EvaluationResult
 from superlinked.framework.online.dag.online_concatenation_node import (
     OnlineConcatenationNode,
 )
 from superlinked.framework.online.dag.online_node import OnlineNode
-from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
-    EvaluationResultStoreManager,
-)
 
 
 class OnlineIndexNode(OnlineNode[IndexNode, Vector], HasLength):
     def __init__(
         self,
         node: IndexNode,
         parents: list[OnlineNode[Node[Vector], Vector]],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
+        storage_manager: StorageManager,
     ) -> None:
-        super().__init__(node, parents, evaluation_result_store_manager)
+        super().__init__(node, parents, storage_manager)
 
     @property
     def length(self) -> int:
         return self.node.length
 
     def get_parent_for_schema(self, schema: SchemaObject) -> OnlineNode:
         active_parents = [
```

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/online_named_function_node.py` & `superlinked-5.2.2/superlinked/framework/online/dag/online_named_function_node.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,36 +18,34 @@
 
 from typing_extensions import override
 
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.named_function_node import NamedFunctionNode
 from superlinked.framework.common.dag.node import NDT
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.common.util.named_function_evaluator import (
     NamedFunctionEvaluator,
 )
 from superlinked.framework.online.dag.evaluation_result import EvaluationResult
 from superlinked.framework.online.dag.online_node import OnlineNode
 from superlinked.framework.online.dag.parent_validator import ParentValidationType
-from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
-    EvaluationResultStoreManager,
-)
 
 
 class OnlineNamedFunctionNode(OnlineNode[NamedFunctionNode[NDT], NDT]):
     def __init__(
         self,
         node: NamedFunctionNode,
         parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
+        storage_manager: StorageManager,
     ) -> None:
         super().__init__(
             node,
             parents,
-            evaluation_result_store_manager,
+            storage_manager,
             ParentValidationType.NO_PARENTS,
         )
 
     @override
     def evaluate_self(
         self,
         parsed_schemas: list[ParsedSchema],
```

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/online_node.py` & `superlinked-5.2.2/superlinked/framework/online/dag/online_node.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,38 +19,36 @@
 
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.exception import ParentCountException
 from superlinked.framework.common.dag.node import NDT, NT
 from superlinked.framework.common.exception import DagEvaluationException
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
 from superlinked.framework.common.schema.schema_object import SchemaObject
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.online.dag.evaluation_result import (
     EvaluationResult,
     SingleEvaluationResult,
 )
 from superlinked.framework.online.dag.parent_validator import ParentValidationType
-from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
-    EvaluationResultStoreManager,
-)
 
 ONT = TypeVar("ONT", bound="OnlineNode")
 
 
 class OnlineNode(ABC, Generic[NT, NDT], metaclass=ABCMeta):
     def __init__(
         self,
         node: NT,
         parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
+        storage_manager: StorageManager,
         parent_validation_type: ParentValidationType = ParentValidationType.NO_VALIDATION,
     ) -> None:
         self.node = node
         self.children: list[OnlineNode] = []
         self.parents = parents
-        self.evaluation_result_store_manager = evaluation_result_store_manager
+        self.storage_manager = storage_manager
         self.validate_parents(parent_validation_type)
         for parent in self.parents:
             parent.children.append(self)
 
     @property
     def class_name(self) -> str:
         return self.__class__.__name__
@@ -89,29 +87,35 @@
         pass
 
     def persist(
         self,
         result: EvaluationResult[NDT],
         parsed_schema: ParsedSchema,
     ) -> None:
-        self.evaluation_result_store_manager.save_result(
-            result,
+        self.storage_manager.write_node_result(
+            parsed_schema.schema,
             parsed_schema.id_,
-            parsed_schema.schema._schema_name,
-            self.node.persistence_type,
+            result.main.node_id,
+            result.main.value,
         )
-
-    def load_stored_result(
-        self, main_object_id: str, schema: SchemaObject
-    ) -> NDT | None:
-        return self.evaluation_result_store_manager.load_stored_result(
-            main_object_id,
+        for chunk in result.chunks:
+            self.storage_manager.write_node_result(
+                parsed_schema.schema,
+                chunk.object_id,
+                chunk.node_id,
+                chunk.value,
+                parsed_schema.id_,
+            )
+
+    def load_stored_result(self, object_id: str, schema: SchemaObject) -> NDT | None:
+        return self.storage_manager.read_node_result(
+            schema,
+            object_id,
             self.node_id,
-            schema._schema_name,
-            self.node.persistence_type,
+            self.node.node_data_type,
         )
 
     def load_stored_result_or_raise_exception(
         self,
         parsed_schema: ParsedSchema,
     ) -> NDT:
         stored_result = self.load_stored_result(parsed_schema.id_, parsed_schema.schema)
```

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/online_node_registry.py` & `superlinked-5.2.2/superlinked/framework/online/dag/online_node_registry.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import inspect
 from pydoc import locate
 from typing import TypeVar, cast
 
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.exception import NotImplementedException
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.online.dag.online_aggregation_node import (
     OnlineAggregationNode,
 )
 from superlinked.framework.online.dag.online_categorical_similarity_node import (
     OnlineCategoricalSimilarityNode,
 )
 from superlinked.framework.online.dag.online_chunking_node import OnlineChunkingNode
@@ -52,17 +53,14 @@
 from superlinked.framework.online.dag.online_recency_node import OnlineRecencyNode
 from superlinked.framework.online.dag.online_schema_field_node import (
     OnlineSchemaFieldNode,
 )
 from superlinked.framework.online.dag.online_text_embedding_node import (
     OnlineTextEmbeddingNode,
 )
-from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
-    EvaluationResultStoreManager,
-)
 
 LNT = TypeVar("LNT", type[Node], type[OnlineNode])
 DEFAULT_NODE_TYPES: list[type[OnlineNode]] = [
     OnlineAggregationNode,
     OnlineChunkingNode,
     OnlineCategoricalSimilarityNode,
     OnlineComparisonFilterNode,
@@ -130,15 +128,15 @@
             )
         return cast(LNT, node_class)
 
     def init_online_node(
         self,
         node: Node,
         parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
+        storage_manager: StorageManager,
     ) -> OnlineNode:
         online_node_class = self.online_node_type_by_node_type.get(type(node))
         if not online_node_class:
             raise NotImplementedException(
                 f"Not implemented Node type: {node.__class__.__name__}"
             )
-        return online_node_class(node, parents, evaluation_result_store_manager)
+        return online_node_class(node, parents, storage_manager)
```

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/online_number_embedding_node.py` & `superlinked-5.2.2/superlinked/framework/online/dag/online_number_embedding_node.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,33 +20,31 @@
 
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.dag.number_embedding_node import NumberEmbeddingNode
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.online.dag.evaluation_result import EvaluationResult
 from superlinked.framework.online.dag.online_node import OnlineNode
 from superlinked.framework.online.dag.parent_validator import ParentValidationType
-from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
-    EvaluationResultStoreManager,
-)
 
 
 class OnlineNumberEmbeddingNode(OnlineNode[NumberEmbeddingNode, Vector], HasLength):
     def __init__(
         self,
         node: NumberEmbeddingNode,
         parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
+        storage_manager: StorageManager,
     ) -> None:
         super().__init__(
             node,
             parents,
-            evaluation_result_store_manager,
+            storage_manager,
             ParentValidationType.LESS_THAN_TWO_PARENTS,
         )
 
     @property
     def length(self) -> int:
         return self.node.length
```

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/online_number_similarity_node.py` & `superlinked-5.2.2/superlinked/framework/online/dag/online_number_similarity_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,33 +20,31 @@
 
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.dag.number_similarity_node import NumberSimilarityNode
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.online.dag.evaluation_result import EvaluationResult
 from superlinked.framework.online.dag.online_node import OnlineNode
 from superlinked.framework.online.dag.parent_validator import ParentValidationType
-from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
-    EvaluationResultStoreManager,
-)
 
 
 class OnlineNumberSimilarityNode(OnlineNode[NumberSimilarityNode, Vector], HasLength):
     def __init__(
         self,
         node: NumberSimilarityNode,
         parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
+        storage_manager: StorageManager,
     ) -> None:
         super().__init__(
             node,
             parents,
-            evaluation_result_store_manager,
+            storage_manager,
             ParentValidationType.LESS_THAN_TWO_PARENTS,
         )
 
     @property
     def length(self) -> int:
         return self.node.length
```

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/online_recency_node.py` & `superlinked-5.2.2/superlinked/framework/online/dag/online_recency_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,36 +17,34 @@
 from beartype.typing import Sequence
 from typing_extensions import override
 
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.recency_node import RecencyNode
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.interface.has_length import HasLength
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.online.dag.default_online_node import DefaultOnlineNode
 from superlinked.framework.online.dag.evaluation_result import SingleEvaluationResult
 from superlinked.framework.online.dag.online_node import OnlineNode
 from superlinked.framework.online.dag.parent_validator import ParentValidationType
-from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
-    EvaluationResultStoreManager,
-)
 
 DAY_IN_SECONDS: int = 24 * 60 * 60
 
 
 class OnlineRecencyNode(DefaultOnlineNode[RecencyNode, Vector], HasLength):
     def __init__(
         self,
         node: RecencyNode,
         parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
+        storage_manager: StorageManager,
     ) -> None:
         super().__init__(
             node,
             parents,
-            evaluation_result_store_manager,
+            storage_manager,
             ParentValidationType.EXACTLY_ONE_PARENT,
         )
 
     @property
     def length(self) -> int:
         return self.node.embedding.length
```

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/online_schema_dag.py` & `superlinked-5.2.2/superlinked/framework/online/dag/online_schema_dag.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/online_schema_field_node.py` & `superlinked-5.2.2/superlinked/framework/online/dag/online_schema_field_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,34 +21,32 @@
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.schema_field_node import SchemaFieldNode
 from superlinked.framework.common.parser.parsed_schema import (
     ParsedSchema,
     ParsedSchemaField,
 )
 from superlinked.framework.common.schema.schema_object import SFT, Timestamp
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.online.dag.evaluation_result import EvaluationResult
 from superlinked.framework.online.dag.exception import ValueNotProvidedException
 from superlinked.framework.online.dag.online_node import OnlineNode
 from superlinked.framework.online.dag.parent_validator import ParentValidationType
-from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
-    EvaluationResultStoreManager,
-)
 
 
 class OnlineSchemaFieldNode(Generic[SFT], OnlineNode[SchemaFieldNode, SFT]):
     def __init__(
         self,
         node: SchemaFieldNode,
         parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
+        storage_manager: StorageManager,
     ) -> None:
         super().__init__(
             node,
             parents,
-            evaluation_result_store_manager,
+            storage_manager,
             ParentValidationType.NO_PARENTS,
         )
 
     @override
     def evaluate_self(
         self,
         parsed_schemas: list[ParsedSchema],
```

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/online_text_embedding_node.py` & `superlinked-5.2.2/superlinked/framework/online/dag/online_text_embedding_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,33 +20,31 @@
 from typing_extensions import override
 
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.text_embedding_node import TextEmbeddingNode
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 from superlinked.framework.online.dag.default_online_node import DefaultOnlineNode
 from superlinked.framework.online.dag.evaluation_result import (
     EvaluationResult,
     SingleEvaluationResult,
 )
 from superlinked.framework.online.dag.online_node import OnlineNode
-from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
-    EvaluationResultStoreManager,
-)
 
 
 class OnlineTextEmbeddingNode(DefaultOnlineNode[TextEmbeddingNode, Vector], HasLength):
     def __init__(
         self,
         node: TextEmbeddingNode,
         parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
+        storage_manager: StorageManager,
     ) -> None:
-        super().__init__(node, parents, evaluation_result_store_manager)
+        super().__init__(node, parents, storage_manager)
 
     @property
     def length(self) -> int:
         return self.node.length
 
     @override
     def evaluate_self(
```

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/parent_results.py` & `superlinked-5.2.2/superlinked/framework/online/dag/parent_results.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/online/dag/parent_validator.py` & `superlinked-5.2.2/superlinked/framework/online/dag/parent_validator.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/online/source/in_memory_data_processor.py` & `superlinked-5.2.2/superlinked/framework/online/source/in_memory_data_processor.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/superlinked/framework/online/source/in_memory_object_writer.py` & `superlinked-5.2.2/superlinked/framework/online/source/in_memory_object_writer.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,29 +8,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from superlinked.framework.common.data_types import Json
 from superlinked.framework.common.observable import Subscriber
 from superlinked.framework.common.parser.json_parser import JsonParser
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
-from superlinked.framework.storage.object_store_manager import (
-    DataId,
-    ObjectStoreManager,
-)
+from superlinked.framework.common.storage_manager.storage_manager import StorageManager
 
 
 class InMemoryObjectWriter(Subscriber[ParsedSchema]):
-    def __init__(self, object_store_manager: ObjectStoreManager[Json]) -> None:
+    def __init__(self, storage_manager: StorageManager) -> None:
         super().__init__()
-        self.__object_store_manager = object_store_manager
+        self.__storage_manager = storage_manager
 
     def update(self, messages: list[ParsedSchema]) -> None:
         for message in messages:
             parser = JsonParser(message.schema)
             data = parser.marshal(message)
-            data_id = DataId(message.schema._schema_name, message.id_)
             for data_element in data:
-                self.__object_store_manager.save(data_id, data_element)
+                self.__storage_manager.write_object_blob(
+                    message.schema, message.id_, data_element
+                )
```

### Comparing `superlinked-4.1.0/superlinked/framework/online/source/in_memory_source.py` & `superlinked-5.2.2/superlinked/framework/online/source/in_memory_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-4.1.0/PKG-INFO` & `superlinked-5.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superlinked
-Version: 4.1.0
+Version: 5.2.2
 Summary: The Superlinked vector computing library
 License: Apache-2.0
 Author: Superlinked Release
 Author-email: release@superlinked.com
 Requires-Python: >=3.10,<=3.12.3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

