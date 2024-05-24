# Comparing `tmp/qianfan-0.3.8.2.tar.gz` & `tmp/qianfan-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qianfan-0.3.8.2.tar", max compression
+gzip compressed data, was "qianfan-0.3.9.tar", max compression
```

## Comparing `qianfan-0.3.8.2.tar` & `qianfan-0.3.9.tar`

### file list

```diff
@@ -1,166 +1,168 @@
--rw-r--r--   0        0        0     6443 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/README.pypi.md
--rw-r--r--   0        0        0     3774 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/pyproject.toml
--rw-r--r--   0        0        0     1578 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/__init__.py
--rw-r--r--   0        0        0      659 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/autotuner/__init__.py
--rw-r--r--   0        0        0     2451 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/autotuner/context.py
--rw-r--r--   0        0        0     4502 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/autotuner/launcher.py
--rw-r--r--   0        0        0      847 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/autotuner/runner/__init__.py
--rw-r--r--   0        0        0     1688 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/autotuner/runner/base.py
--rw-r--r--   0        0        0     6028 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/autotuner/runner/infer_runner.py
--rw-r--r--   0        0        0     6278 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/autotuner/runner/qianfan_runner.py
--rw-r--r--   0        0        0     1460 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/autotuner/space.py
--rw-r--r--   0        0        0      784 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/autotuner/suggestor/__init__.py
--rw-r--r--   0        0        0     3370 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/autotuner/suggestor/base.py
--rw-r--r--   0        0        0     3356 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/autotuner/suggestor/random_suggestor.py
--rw-r--r--   0        0        0     3973 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/autotuner/tune.py
--rw-r--r--   0        0        0     1357 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/autotuner/utils.py
--rw-r--r--   0        0        0      699 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/common/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/common/client/__init__.py
--rw-r--r--   0        0        0    15290 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/common/client/chat.py
--rw-r--r--   0        0        0     7120 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/common/client/completion.py
--rw-r--r--   0        0        0    14564 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/common/client/dataset.py
--rw-r--r--   0        0        0      790 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/common/client/embedding.py
--rw-r--r--   0        0        0     9595 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/common/client/evaluation.py
--rw-r--r--   0        0        0     6437 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/common/client/main.py
--rw-r--r--   0        0        0     4107 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/common/client/openai_adapter.py
--rw-r--r--   0        0        0    17018 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/common/client/plugin.py
--rw-r--r--   0        0        0    24762 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/common/client/trainer.py
--rw-r--r--   0        0        0     3265 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/common/client/txt2img.py
--rw-r--r--   0        0        0     9991 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/common/client/utils.py
--rw-r--r--   0        0        0        1 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/common/hub/__init__.py
--rw-r--r--   0        0        0     5823 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/common/hub/hub.py
--rw-r--r--   0        0        0     3512 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/common/hub/interface.py
--rw-r--r--   0        0        0        0 2024-04-15 16:01:59.713770 qianfan-0.3.8.2/qianfan/common/persister/__init__.py
--rw-r--r--   0        0        0      963 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/common/persister/base.py
--rw-r--r--   0        0        0     2982 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/common/persister/persist.py
--rw-r--r--   0        0        0        0 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/common/prompt/__init__.py
--rw-r--r--   0        0        0    30862 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/common/prompt/prompt.py
--rw-r--r--   0        0        0     2215 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/common/prompt/template.py
--rw-r--r--   0        0        0        0 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/common/runnable/__init__.py
--rw-r--r--   0        0        0     7049 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/common/runnable/base.py
--rw-r--r--   0        0        0     3698 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/common/tool/baidu_search_tool.py
--rw-r--r--   0        0        0     7561 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/common/tool/base_tool.py
--rw-r--r--   0        0        0     2962 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/common/tool/duckduckgo_search_tool.py
--rw-r--r--   0        0        0     3312 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/common/tool/wikipedia_tool.py
--rw-r--r--   0        0        0     9582 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/config.py
--rw-r--r--   0        0        0    12267 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/consts.py
--rw-r--r--   0        0        0     1367 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/__init__.py
--rw-r--r--   0        0        0     2786 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/consts.py
--rw-r--r--   0        0        0      600 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/data_insight/__init__.py
--rw-r--r--   0        0        0     2369 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/data_insight/assets/index.html
--rw-r--r--   0        0        0      841 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/data_insight/data_insight_utils.py
--rw-r--r--   0        0        0     8768 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/data_insight/insight.py
--rw-r--r--   0        0        0     4363 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/data_operator.py
--rw-r--r--   0        0        0     1013 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/data_source/__init__.py
--rw-r--r--   0        0        0    27521 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/data_source/baidu_qianfan.py
--rw-r--r--   0        0        0     2701 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/data_source/base.py
--rw-r--r--   0        0        0    13584 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/data_source/bos.py
--rw-r--r--   0        0        0     9436 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/data_source/chunk_reader.py
--rw-r--r--   0        0        0     9532 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/data_source/file.py
--rw-r--r--   0        0        0    26192 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/data_source/utils.py
--rw-r--r--   0        0        0    74145 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/dataset.py
--rw-r--r--   0        0        0    17893 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/dataset_utils.py
--rw-r--r--   0        0        0     1139 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/local_data_operators/__init__.py
--rw-r--r--   0        0        0     2237 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/local_data_operators/base.py
--rw-r--r--   0        0        0     3942 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/local_data_operators/check_character_repetition_filter.py
--rw-r--r--   0        0        0     4482 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/local_data_operators/check_flagged_words.py
--rw-r--r--   0        0        0     2443 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/local_data_operators/check_sentence_length_filter.py
--rw-r--r--   0        0        0     2504 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/local_data_operators/check_special_characters.py
--rw-r--r--   0        0        0     4313 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/local_data_operators/check_stopwords.py
--rw-r--r--   0        0        0     3085 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/local_data_operators/check_word_number.py
--rw-r--r--   0        0        0     3910 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/local_data_operators/check_word_repetition_filter.py
--rw-r--r--   0        0        0     4483 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/local_data_operators/consts.py
--rw-r--r--   0        0        0     4693 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/local_data_operators/utils.py
--rw-r--r--   0        0        0   136258 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/local_data_operators/word_list.py
--rw-r--r--   0        0        0     2832 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/process_interface.py
--rw-r--r--   0        0        0     4363 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/qianfan_data_operators.py
--rw-r--r--   0        0        0    10622 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/schema.py
--rw-r--r--   0        0        0     2010 2024-04-15 16:01:59.717770 qianfan-0.3.8.2/qianfan/dataset/summarization_method.py
--rw-r--r--   0        0        0    51483 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/dataset/table.py
--rw-r--r--   0        0        0     1302 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/dataset/table_utils.py
--rw-r--r--   0        0        0     2334 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/errors.py
--rw-r--r--   0        0        0      878 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/evaluation/__init__.py
--rw-r--r--   0        0        0     2748 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/evaluation/consts.py
--rw-r--r--   0        0        0    26399 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/evaluation/evaluation_manager.py
--rw-r--r--   0        0        0     1325 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/evaluation/evaluation_result.py
--rw-r--r--   0        0        0     4484 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/evaluation/evaluator.py
--rw-r--r--   0        0        0     4379 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/evaluation/local_evaluator.py
--rw-r--r--   0        0        0     2468 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/evaluation/opencompass_evaluator.py
--rw-r--r--   0        0        0       66 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/extensions/README.md
--rw-r--r--   0        0        0        0 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/extensions/__init__.py
--rw-r--r--   0        0        0      200 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/extensions/langchain/__init__.py
--rw-r--r--   0        0        0      212 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/extensions/langchain/agents/__init__.py
--rw-r--r--   0        0        0    13709 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/extensions/langchain/agents/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0        0 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/extensions/openai/__init__.py
--rw-r--r--   0        0        0    18554 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/extensions/openai/adapter.py
--rw-r--r--   0        0        0     1602 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/extensions/semantic_kernel/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/extensions/semantic_kernel/connectors/__init__.py
--rw-r--r--   0        0        0     7804 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/extensions/semantic_kernel/connectors/qianfan_chat_completion.py
--rw-r--r--   0        0        0     1627 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/extensions/semantic_kernel/connectors/qianfan_settings.py
--rw-r--r--   0        0        0     5365 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/extensions/semantic_kernel/connectors/qianfan_text_completion.py
--rw-r--r--   0        0        0     4056 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/extensions/semantic_kernel/connectors/qianfan_text_embedding.py
--rw-r--r--   0        0        0     2577 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/fake_pyarrow_replacer.py
--rw-r--r--   0        0        0      742 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/model/__init__.py
--rw-r--r--   0        0        0      923 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/model/configs.py
--rw-r--r--   0        0        0      938 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/model/consts.py
--rw-r--r--   0        0        0    23100 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/model/model.py
--rw-r--r--   0        0        0        0 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/py.typed
--rw-r--r--   0        0        0     1648 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/auth/__init__.py
--rw-r--r--   0        0        0     1656 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/auth/iam.py
--rw-r--r--   0        0        0    15255 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/auth/oauth.py
--rw-r--r--   0        0        0        0 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/console/__init__.py
--rw-r--r--   0        0        0     4183 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/console/charge.py
--rw-r--r--   0        0        0     7533 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/console/consts.py
--rw-r--r--   0        0        0    30894 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/console/data.py
--rw-r--r--   0        0        0    16673 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/console/finetune.py
--rw-r--r--   0        0        0    23132 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/console/model.py
--rw-r--r--   0        0        0    19491 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/console/prompt.py
--rw-r--r--   0        0        0     5607 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/console/service.py
--rw-r--r--   0        0        0     4941 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/console/utils.py
--rw-r--r--   0        0        0     3779 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/http_client.py
--rw-r--r--   0        0        0        0 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/images/__init__.py
--rw-r--r--   0        0        0    11411 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/images/image2text.py
--rw-r--r--   0        0        0    11777 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/images/text2image.py
--rw-r--r--   0        0        0        0 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/llm/__init__.py
--rw-r--r--   0        0        0    27287 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/llm/base.py
--rw-r--r--   0        0        0    42166 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/llm/chat_completion.py
--rw-r--r--   0        0        0    11545 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/llm/completion.py
--rw-r--r--   0        0        0    10678 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/llm/embedding.py
--rw-r--r--   0        0        0    13139 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/llm/plugin.py
--rw-r--r--   0        0        0    14096 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/rate_limiter.py
--rw-r--r--   0        0        0        0 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/requestor/__init__.py
--rw-r--r--   0        0        0    12846 2024-04-15 16:01:59.721770 qianfan-0.3.8.2/qianfan/resources/requestor/base.py
--rw-r--r--   0        0        0     3189 2024-04-15 16:01:59.725770 qianfan-0.3.8.2/qianfan/resources/requestor/console_requestor.py
--rw-r--r--   0        0        0    22255 2024-04-15 16:01:59.725770 qianfan-0.3.8.2/qianfan/resources/requestor/openapi_requestor.py
--rw-r--r--   0        0        0    10266 2024-04-15 16:01:59.725770 qianfan-0.3.8.2/qianfan/resources/token_limiter.py
--rw-r--r--   0        0        0        0 2024-04-15 16:01:59.725770 qianfan-0.3.8.2/qianfan/resources/tools/__init__.py
--rw-r--r--   0        0        0     4909 2024-04-15 16:01:59.725770 qianfan-0.3.8.2/qianfan/resources/tools/tokenizer.py
--rw-r--r--   0        0        0     3580 2024-04-15 16:01:59.725770 qianfan-0.3.8.2/qianfan/resources/tools/utils.py
--rw-r--r--   0        0        0     9199 2024-04-15 16:01:59.725770 qianfan-0.3.8.2/qianfan/resources/typing.py
--rw-r--r--   0        0        0     1141 2024-04-15 16:01:59.725770 qianfan-0.3.8.2/qianfan/trainer/__init__.py
--rw-r--r--   0        0        0    46962 2024-04-15 16:01:59.725770 qianfan-0.3.8.2/qianfan/trainer/actions.py
--rw-r--r--   0        0        0     6000 2024-04-15 16:01:59.725770 qianfan-0.3.8.2/qianfan/trainer/base.py
--rw-r--r--   0        0        0    38188 2024-04-15 16:01:59.725770 qianfan-0.3.8.2/qianfan/trainer/configs.py
--rw-r--r--   0        0        0     3600 2024-04-15 16:01:59.725770 qianfan-0.3.8.2/qianfan/trainer/consts.py
--rw-r--r--   0        0        0     3403 2024-04-15 16:01:59.725770 qianfan-0.3.8.2/qianfan/trainer/event.py
--rw-r--r--   0        0        0    13824 2024-04-15 16:01:59.725770 qianfan-0.3.8.2/qianfan/trainer/finetune.py
--rw-r--r--   0        0        0    10187 2024-04-15 16:01:59.725770 qianfan-0.3.8.2/qianfan/trainer/pipeline.py
--rw-r--r--   0        0        0     8360 2024-04-15 16:01:59.725770 qianfan-0.3.8.2/qianfan/trainer/post_pretrain.py
--rw-r--r--   0        0        0     1680 2024-04-15 16:01:59.725770 qianfan-0.3.8.2/qianfan/trainer/ppl.yaml
--rw-r--r--   0        0        0     4843 2024-04-15 16:01:59.725770 qianfan-0.3.8.2/qianfan/trainer/trainer.py
--rw-r--r--   0        0        0     1244 2024-04-15 16:01:59.729771 qianfan-0.3.8.2/qianfan/utils/__init__.py
--rw-r--r--   0        0        0     4647 2024-04-15 16:01:59.729771 qianfan-0.3.8.2/qianfan/utils/bos_uploader.py
--rw-r--r--   0        0        0      696 2024-04-15 16:01:59.729771 qianfan-0.3.8.2/qianfan/utils/cache/__init__.py
--rw-r--r--   0        0        0      787 2024-04-15 16:01:59.729771 qianfan-0.3.8.2/qianfan/utils/cache/base.py
--rw-r--r--   0        0        0      827 2024-04-15 16:01:59.729771 qianfan-0.3.8.2/qianfan/utils/fake_pyarrow/__init__.py
--rw-r--r--   0        0        0      946 2024-04-15 16:01:59.729771 qianfan-0.3.8.2/qianfan/utils/fake_pyarrow/compute.py
--rw-r--r--   0        0        0      812 2024-04-15 16:01:59.729771 qianfan-0.3.8.2/qianfan/utils/fake_pyarrow/functions.py
--rw-r--r--   0        0        0      869 2024-04-15 16:01:59.729771 qianfan-0.3.8.2/qianfan/utils/fake_pyarrow/ipc.py
--rw-r--r--   0        0        0      984 2024-04-15 16:01:59.729771 qianfan-0.3.8.2/qianfan/utils/fake_pyarrow/table.py
--rw-r--r--   0        0        0     1084 2024-04-15 16:01:59.729771 qianfan-0.3.8.2/qianfan/utils/helper.py
--rw-r--r--   0        0        0     5670 2024-04-15 16:01:59.729771 qianfan-0.3.8.2/qianfan/utils/logging.py
--rw-r--r--   0        0        0      734 2024-04-15 16:01:59.729771 qianfan-0.3.8.2/qianfan/utils/pydantic/__init__.py
--rw-r--r--   0        0        0     7230 2024-04-15 16:01:59.729771 qianfan-0.3.8.2/qianfan/utils/utils.py
--rw-r--r--   0        0        0      900 2024-04-15 16:01:59.729771 qianfan-0.3.8.2/qianfan/version.py
--rw-r--r--   0        0        0    10491 1970-01-01 00:00:00.000000 qianfan-0.3.8.2/PKG-INFO
+-rw-r--r--   0        0        0     6443 2024-04-18 15:03:12.506216 qianfan-0.3.9/README.pypi.md
+-rw-r--r--   0        0        0     3772 2024-04-18 15:03:12.506216 qianfan-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1578 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/__init__.py
+-rw-r--r--   0        0        0      659 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/autotuner/__init__.py
+-rw-r--r--   0        0        0     2451 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/autotuner/context.py
+-rw-r--r--   0        0        0     4502 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/autotuner/launcher.py
+-rw-r--r--   0        0        0      847 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/autotuner/runner/__init__.py
+-rw-r--r--   0        0        0     1688 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/autotuner/runner/base.py
+-rw-r--r--   0        0        0     6028 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/autotuner/runner/infer_runner.py
+-rw-r--r--   0        0        0     6278 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/autotuner/runner/qianfan_runner.py
+-rw-r--r--   0        0        0     1460 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/autotuner/space.py
+-rw-r--r--   0        0        0      784 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/autotuner/suggestor/__init__.py
+-rw-r--r--   0        0        0     3370 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/autotuner/suggestor/base.py
+-rw-r--r--   0        0        0     3356 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/autotuner/suggestor/random_suggestor.py
+-rw-r--r--   0        0        0     3973 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/autotuner/tune.py
+-rw-r--r--   0        0        0     1357 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/autotuner/utils.py
+-rw-r--r--   0        0        0      699 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/client/__init__.py
+-rw-r--r--   0        0        0    15290 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/client/chat.py
+-rw-r--r--   0        0        0     7120 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/client/completion.py
+-rw-r--r--   0        0        0    14564 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/client/dataset.py
+-rw-r--r--   0        0        0      790 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/client/embedding.py
+-rw-r--r--   0        0        0     9595 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/client/evaluation.py
+-rw-r--r--   0        0        0     6437 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/client/main.py
+-rw-r--r--   0        0        0     4136 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/client/openai_adapter.py
+-rw-r--r--   0        0        0    17018 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/client/plugin.py
+-rw-r--r--   0        0        0    31652 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/client/trainer.py
+-rw-r--r--   0        0        0     3265 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/client/txt2img.py
+-rw-r--r--   0        0        0     9991 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/client/utils.py
+-rw-r--r--   0        0        0        1 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/hub/__init__.py
+-rw-r--r--   0        0        0     5823 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/hub/hub.py
+-rw-r--r--   0        0        0     3512 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/hub/interface.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/persister/__init__.py
+-rw-r--r--   0        0        0      963 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/persister/base.py
+-rw-r--r--   0        0        0     2982 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/persister/persist.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/prompt/__init__.py
+-rw-r--r--   0        0        0    30862 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/prompt/prompt.py
+-rw-r--r--   0        0        0     2215 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/prompt/template.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/runnable/__init__.py
+-rw-r--r--   0        0        0     7049 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/runnable/base.py
+-rw-r--r--   0        0        0     3698 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/tool/baidu_search_tool.py
+-rw-r--r--   0        0        0     7561 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/tool/base_tool.py
+-rw-r--r--   0        0        0     2962 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/tool/duckduckgo_search_tool.py
+-rw-r--r--   0        0        0     3312 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/common/tool/wikipedia_tool.py
+-rw-r--r--   0        0        0     9582 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/config.py
+-rw-r--r--   0        0        0    12459 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/consts.py
+-rw-r--r--   0        0        0     1367 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/dataset/__init__.py
+-rw-r--r--   0        0        0     2786 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/dataset/consts.py
+-rw-r--r--   0        0        0      600 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/dataset/data_insight/__init__.py
+-rw-r--r--   0        0        0     2369 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/dataset/data_insight/assets/index.html
+-rw-r--r--   0        0        0      841 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/dataset/data_insight/data_insight_utils.py
+-rw-r--r--   0        0        0     8768 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/dataset/data_insight/insight.py
+-rw-r--r--   0        0        0     4363 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/dataset/data_operator.py
+-rw-r--r--   0        0        0     1013 2024-04-18 15:03:12.506216 qianfan-0.3.9/qianfan/dataset/data_source/__init__.py
+-rw-r--r--   0        0        0    27521 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/data_source/baidu_qianfan.py
+-rw-r--r--   0        0        0     2701 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/data_source/base.py
+-rw-r--r--   0        0        0    13584 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/data_source/bos.py
+-rw-r--r--   0        0        0     9436 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/data_source/chunk_reader.py
+-rw-r--r--   0        0        0    10077 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/data_source/file.py
+-rw-r--r--   0        0        0    26192 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/data_source/utils.py
+-rw-r--r--   0        0        0    74145 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/dataset.py
+-rw-r--r--   0        0        0    17893 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/dataset_utils.py
+-rw-r--r--   0        0        0     1139 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/local_data_operators/__init__.py
+-rw-r--r--   0        0        0     2237 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/local_data_operators/base.py
+-rw-r--r--   0        0        0     3942 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/local_data_operators/check_character_repetition_filter.py
+-rw-r--r--   0        0        0     4482 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/local_data_operators/check_flagged_words.py
+-rw-r--r--   0        0        0     2443 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/local_data_operators/check_sentence_length_filter.py
+-rw-r--r--   0        0        0     2504 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/local_data_operators/check_special_characters.py
+-rw-r--r--   0        0        0     4313 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/local_data_operators/check_stopwords.py
+-rw-r--r--   0        0        0     3085 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/local_data_operators/check_word_number.py
+-rw-r--r--   0        0        0     3910 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/local_data_operators/check_word_repetition_filter.py
+-rw-r--r--   0        0        0     4483 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/local_data_operators/consts.py
+-rw-r--r--   0        0        0     4693 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/local_data_operators/utils.py
+-rw-r--r--   0        0        0   136258 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/local_data_operators/word_list.py
+-rw-r--r--   0        0        0     2832 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/process_interface.py
+-rw-r--r--   0        0        0     4363 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/qianfan_data_operators.py
+-rw-r--r--   0        0        0    10622 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/schema.py
+-rw-r--r--   0        0        0     2010 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/summarization_method.py
+-rw-r--r--   0        0        0    51483 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/table.py
+-rw-r--r--   0        0        0     1302 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/dataset/table_utils.py
+-rw-r--r--   0        0        0     2334 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/errors.py
+-rw-r--r--   0        0        0      878 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/evaluation/__init__.py
+-rw-r--r--   0        0        0     2748 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/evaluation/consts.py
+-rw-r--r--   0        0        0    26399 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/evaluation/evaluation_manager.py
+-rw-r--r--   0        0        0     1325 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/evaluation/evaluation_result.py
+-rw-r--r--   0        0        0     4484 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/evaluation/evaluator.py
+-rw-r--r--   0        0        0     4379 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/evaluation/local_evaluator.py
+-rw-r--r--   0        0        0     2468 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/evaluation/opencompass_evaluator.py
+-rw-r--r--   0        0        0       66 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/extensions/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/extensions/__init__.py
+-rw-r--r--   0        0        0      200 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/extensions/langchain/__init__.py
+-rw-r--r--   0        0        0      212 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/extensions/langchain/agents/__init__.py
+-rw-r--r--   0        0        0    13709 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/extensions/langchain/agents/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/extensions/openai/__init__.py
+-rw-r--r--   0        0        0    18554 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/extensions/openai/adapter.py
+-rw-r--r--   0        0        0     1602 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/extensions/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/extensions/semantic_kernel/connectors/__init__.py
+-rw-r--r--   0        0        0     7804 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/extensions/semantic_kernel/connectors/qianfan_chat_completion.py
+-rw-r--r--   0        0        0     1627 2024-04-18 15:03:12.510216 qianfan-0.3.9/qianfan/extensions/semantic_kernel/connectors/qianfan_settings.py
+-rw-r--r--   0        0        0     5365 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/extensions/semantic_kernel/connectors/qianfan_text_completion.py
+-rw-r--r--   0        0        0     4056 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/extensions/semantic_kernel/connectors/qianfan_text_embedding.py
+-rw-r--r--   0        0        0     2577 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/fake_pyarrow_replacer.py
+-rw-r--r--   0        0        0      742 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/model/__init__.py
+-rw-r--r--   0        0        0      923 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/model/configs.py
+-rw-r--r--   0        0        0      938 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/model/consts.py
+-rw-r--r--   0        0        0    23100 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/model/model.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/py.typed
+-rw-r--r--   0        0        0     1714 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/auth/__init__.py
+-rw-r--r--   0        0        0     1656 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/auth/iam.py
+-rw-r--r--   0        0        0    15255 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/auth/oauth.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/console/__init__.py
+-rw-r--r--   0        0        0     4183 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/console/charge.py
+-rw-r--r--   0        0        0     7599 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/console/consts.py
+-rw-r--r--   0        0        0    30894 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/console/data.py
+-rw-r--r--   0        0        0    16673 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/console/finetune.py
+-rw-r--r--   0        0        0    23132 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/console/model.py
+-rw-r--r--   0        0        0    19491 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/console/prompt.py
+-rw-r--r--   0        0        0    10097 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/console/service.py
+-rw-r--r--   0        0        0     4941 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/console/utils.py
+-rw-r--r--   0        0        0     3779 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/http_client.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/images/__init__.py
+-rw-r--r--   0        0        0    11411 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/images/image2text.py
+-rw-r--r--   0        0        0    11777 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/images/text2image.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/llm/__init__.py
+-rw-r--r--   0        0        0    27287 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/llm/base.py
+-rw-r--r--   0        0        0    42166 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/llm/chat_completion.py
+-rw-r--r--   0        0        0    11545 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/llm/completion.py
+-rw-r--r--   0        0        0    10678 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/llm/embedding.py
+-rw-r--r--   0        0        0    13139 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/llm/plugin.py
+-rw-r--r--   0        0        0     7206 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/llm/rerank.py
+-rw-r--r--   0        0        0    14096 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/rate_limiter.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/requestor/__init__.py
+-rw-r--r--   0        0        0    12846 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/requestor/base.py
+-rw-r--r--   0        0        0     3189 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/requestor/console_requestor.py
+-rw-r--r--   0        0        0    22255 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/requestor/openapi_requestor.py
+-rw-r--r--   0        0        0    10266 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/token_limiter.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/tools/__init__.py
+-rw-r--r--   0        0        0     4909 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/tools/tokenizer.py
+-rw-r--r--   0        0        0     3580 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/tools/utils.py
+-rw-r--r--   0        0        0     9199 2024-04-18 15:03:12.514216 qianfan-0.3.9/qianfan/resources/typing.py
+-rw-r--r--   0        0        0     1188 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/trainer/__init__.py
+-rw-r--r--   0        0        0    46962 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/trainer/actions.py
+-rw-r--r--   0        0        0     6000 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/trainer/base.py
+-rw-r--r--   0        0        0    38772 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/trainer/configs.py
+-rw-r--r--   0        0        0     3600 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/trainer/consts.py
+-rw-r--r--   0        0        0    12180 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/trainer/dpo.py
+-rw-r--r--   0        0        0     3403 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/trainer/event.py
+-rw-r--r--   0        0        0    13854 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/trainer/finetune.py
+-rw-r--r--   0        0        0    10187 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/trainer/pipeline.py
+-rw-r--r--   0        0        0     8360 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/trainer/post_pretrain.py
+-rw-r--r--   0        0        0     1680 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/trainer/ppl.yaml
+-rw-r--r--   0        0        0     4843 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/trainer/trainer.py
+-rw-r--r--   0        0        0     1244 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/utils/__init__.py
+-rw-r--r--   0        0        0     4647 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/utils/bos_uploader.py
+-rw-r--r--   0        0        0      696 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/utils/cache/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/utils/cache/base.py
+-rw-r--r--   0        0        0      827 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/utils/fake_pyarrow/__init__.py
+-rw-r--r--   0        0        0      946 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/utils/fake_pyarrow/compute.py
+-rw-r--r--   0        0        0      812 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/utils/fake_pyarrow/functions.py
+-rw-r--r--   0        0        0      869 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/utils/fake_pyarrow/ipc.py
+-rw-r--r--   0        0        0      984 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/utils/fake_pyarrow/table.py
+-rw-r--r--   0        0        0     1084 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/utils/helper.py
+-rw-r--r--   0        0        0     5670 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/utils/logging.py
+-rw-r--r--   0        0        0      734 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/utils/pydantic/__init__.py
+-rw-r--r--   0        0        0     7230 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/utils/utils.py
+-rw-r--r--   0        0        0      900 2024-04-18 15:03:12.518216 qianfan-0.3.9/qianfan/version.py
+-rw-r--r--   0        0        0    10489 1970-01-01 00:00:00.000000 qianfan-0.3.9/PKG-INFO
```

### Comparing `qianfan-0.3.8.2/README.pypi.md` & `qianfan-0.3.9/README.pypi.md`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/pyproject.toml` & `qianfan-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qianfan"
-version = "0.3.8.2"
+version = "0.3.9"
 description = "文心千帆大模型平台 Python SDK"
 authors = []
 license = "Apache-2.0"
 readme = "README.pypi.md"
 exclude = [
     "qianfan/tests",
     "qianfan/docs",
```

### Comparing `qianfan-0.3.8.2/qianfan/__init__.py` & `qianfan-0.3.9/qianfan/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/autotuner/__init__.py` & `qianfan-0.3.9/qianfan/autotuner/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/autotuner/context.py` & `qianfan-0.3.9/qianfan/autotuner/context.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/autotuner/launcher.py` & `qianfan-0.3.9/qianfan/autotuner/launcher.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/autotuner/runner/__init__.py` & `qianfan-0.3.9/qianfan/autotuner/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/autotuner/runner/base.py` & `qianfan-0.3.9/qianfan/autotuner/runner/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/autotuner/runner/infer_runner.py` & `qianfan-0.3.9/qianfan/autotuner/runner/infer_runner.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/autotuner/runner/qianfan_runner.py` & `qianfan-0.3.9/qianfan/autotuner/runner/qianfan_runner.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/autotuner/space.py` & `qianfan-0.3.9/qianfan/autotuner/space.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/autotuner/suggestor/__init__.py` & `qianfan-0.3.9/qianfan/autotuner/suggestor/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/autotuner/suggestor/base.py` & `qianfan-0.3.9/qianfan/autotuner/suggestor/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/autotuner/suggestor/random_suggestor.py` & `qianfan-0.3.9/qianfan/autotuner/suggestor/random_suggestor.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/autotuner/tune.py` & `qianfan-0.3.9/qianfan/autotuner/tune.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/autotuner/utils.py` & `qianfan-0.3.9/qianfan/autotuner/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/common/__init__.py` & `qianfan-0.3.9/qianfan/common/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/common/client/chat.py` & `qianfan-0.3.9/qianfan/common/client/chat.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/common/client/completion.py` & `qianfan-0.3.9/qianfan/common/client/completion.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/common/client/dataset.py` & `qianfan-0.3.9/qianfan/common/client/dataset.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/common/client/embedding.py` & `qianfan-0.3.9/qianfan/common/client/embedding.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/common/client/evaluation.py` & `qianfan-0.3.9/qianfan/common/client/evaluation.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/common/client/main.py` & `qianfan-0.3.9/qianfan/common/client/main.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/common/client/openai_adapter.py` & `qianfan-0.3.9/qianfan/common/client/openai_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 async def stream(resp: AsyncIterator[Any]) -> AsyncIterator[str]:
     """
     Convert an async iterator to a stream.
     """
     async for data in resp:
         yield "data: " + json.dumps(data) + "\n\n"
+    yield "data: [DONE]\n\n"
 
 
 @app.post("/v1/chat/completions")
 async def chat_completion(request: Request) -> Response:
     openai_params = await request.json()
     assert openai_params is not None
     resp = await adapter.chat(openai_params)
```

### Comparing `qianfan-0.3.8.2/qianfan/common/client/plugin.py` & `qianfan-0.3.9/qianfan/common/client/plugin.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/common/client/trainer.py` & `qianfan-0.3.9/qianfan/common/client/trainer.py`

 * *Files 18% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     replace_logger_handler,
 )
 from qianfan.dataset import Dataset
 from qianfan.errors import InternalError
 from qianfan.model.configs import DeployConfig
 from qianfan.model.consts import ServiceType
 from qianfan.resources.console.consts import DeployPoolType, FinetuneSupportModelType
-from qianfan.trainer import LLMFinetune, PostPreTrain
+from qianfan.trainer import DPO, LLMFinetune, PostPreTrain
 from qianfan.trainer.actions import (
     DeployAction,
     EvaluateAction,
     LoadDataSetAction,
     ModelPublishAction,
     TrainAction,
 )
@@ -217,14 +217,16 @@
                 "Command name is not specified. Might be an internal error."
             )
             raise typer.Exit(1)
         if cmd == "postpretrain":
             model_list = PostPreTrain.train_type_list()
         elif cmd in ["finetune", "run"]:
             model_list = LLMFinetune.train_type_list()
+        elif cmd in ["dpo"]:
+            model_list = DPO.train_type_list()
         else:
             print_error_msg(
                 f"Command {cmd} is not supported. Might be an internal error."
             )
             raise typer.Exit(1)
 
         model_type_map: Dict[FinetuneSupportModelType, Dict[str, List]] = {}
@@ -299,14 +301,16 @@
                 "Command name is not specified. Might be an internal error."
             )
             raise typer.Exit(1)
         if cmd == "postpretrain":
             model_list = PostPreTrain.train_type_list()
         elif cmd in ["finetune", "run"]:
             model_list = LLMFinetune.train_type_list()
+        elif cmd in ["dpo"]:
+            model_list = DPO.train_type_list()
         else:
             print_error_msg(
                 f"Command {cmd} is not supported. Might be an internal error."
             )
             raise typer.Exit(1)
 
         if value not in model_list:
@@ -653,7 +657,180 @@
     trainer.run()
 
     console.log("Trainer finished!")
     console.log(Pretty(trainer.output))
 
     # wait a second for the log to be flushed
     time.sleep(0.1)
+
+
+@trainer_app.command(
+    "run",
+    deprecated=True,
+    help="Run a dpo trainer task.",
+)
+@trainer_app.command()
+@credential_required
+def dpo(
+    dataset_id: Optional[str] = typer.Option(None, help="Dataset id"),
+    dataset_bos_path: Optional[str] = typer.Option(
+        None,
+        help="Dataset BOS path",
+    ),
+    train_type: Optional[str] = typer.Option(None, help="Train type"),
+    previous_task_id: Optional[str] = typer.Option(
+        None, help="Task id of previous trainer output."
+    ),
+    trainer_pipeline_file: Optional[str] = typer.Option(
+        None, help="Trainer pipeline file path"
+    ),
+    daemon: Optional[bool] = daemon_option,
+    list_train_type: Optional[bool] = list_train_type_option,
+    show_config_limit: Optional[str] = typer.Option(
+        None,
+        callback=show_config_limit,
+        is_eager=True,
+        help="Show config limit for specified train type.",
+    ),
+    train_config_file: Optional[str] = typer.Option(
+        None, help="Train config path, support \[json/yaml] "
+    ),
+    train_epoch: Optional[int] = typer.Option(
+        None, help="Train epoch", rich_help_panel=TRAIN_CONFIG_PANEL
+    ),
+    train_batch_size: Optional[int] = typer.Option(
+        None, help="Train batch size", rich_help_panel=TRAIN_CONFIG_PANEL
+    ),
+    train_learning_rate: Optional[float] = typer.Option(
+        None, help="Train learning rate", rich_help_panel=TRAIN_CONFIG_PANEL
+    ),
+    train_max_seq_len: Optional[int] = typer.Option(
+        None, help="Max sequence length", rich_help_panel=TRAIN_CONFIG_PANEL
+    ),
+    train_peft_type: Optional[PeftType] = typer.Option(
+        None,
+        help="Train peft type",
+        **enum_typer(PeftType),
+        rich_help_panel=TRAIN_CONFIG_PANEL,
+    ),
+    trainset_rate: int = typer.Option(
+        20, help="Trainset ratio", rich_help_panel=TRAIN_CONFIG_PANEL
+    ),
+    train_logging_steps: Optional[int] = typer.Option(
+        None, help="Logging steps", rich_help_panel=TRAIN_CONFIG_PANEL
+    ),
+    train_warmup_ratio: Optional[float] = typer.Option(
+        None, help="Warmup ratio", rich_help_panel=TRAIN_CONFIG_PANEL
+    ),
+    train_weight_decay: Optional[float] = typer.Option(
+        None, help="Weight decay", rich_help_panel=TRAIN_CONFIG_PANEL
+    ),
+    train_lora_rank: Optional[int] = typer.Option(
+        None, help="Lora rank", rich_help_panel=TRAIN_CONFIG_PANEL
+    ),
+    train_lora_all_linear: Optional[str] = typer.Option(
+        None,
+        help="Whether lora is all linear layer",
+        rich_help_panel=TRAIN_CONFIG_PANEL,
+    ),
+    deploy_name: Optional[str] = typer.Option(
+        None,
+        help="Deploy name. Set this value to enable deploy action.",
+        rich_help_panel=DEPLOY_CONFIG_PANEL,
+    ),
+    deploy_endpoint_prefix: Optional[str] = typer.Option(
+        None, help="Deploy endpoint prefix", rich_help_panel=DEPLOY_CONFIG_PANEL
+    ),
+    deploy_description: str = typer.Option(
+        "", help="Deploy description", rich_help_panel=DEPLOY_CONFIG_PANEL
+    ),
+    deploy_replicas: int = typer.Option(
+        1, help="Deploy replicas", rich_help_panel=DEPLOY_CONFIG_PANEL
+    ),
+    deploy_pool_type: str = typer.Option(
+        "private_resource",
+        help="Deploy pool type",
+        **enum_typer(DeployPoolType),
+        rich_help_panel=DEPLOY_CONFIG_PANEL,
+    ),
+    deploy_service_type: str = typer.Option(
+        "chat",
+        help="Service Type",
+        **enum_typer(ServiceType),
+        rich_help_panel=DEPLOY_CONFIG_PANEL,
+    ),
+) -> None:
+    """
+    Run a dpo trainer job.
+    """
+    console = replace_logger_handler()
+    callback = MyEventHandler(console=console)
+
+    if trainer_pipeline_file is not None:
+        trainer = LLMFinetune.load(file=trainer_pipeline_file)
+        trainer.register_event_handler(callback)
+    else:
+        ds = None
+        if dataset_id is not None:
+            ds = Dataset.load(qianfan_dataset_id=dataset_id, does_release=True)
+        deploy_config = None
+        if deploy_name is not None:
+            if deploy_endpoint_prefix is None:
+                print_error_msg("Deploy endpoint prefix is required")
+                raise typer.Exit(code=1)
+
+            deploy_config = DeployConfig(
+                name=deploy_name,
+                endpoint_prefix=deploy_endpoint_prefix,
+                description=deploy_description,
+                replicas=deploy_replicas,
+                pool_type=DeployPoolType[deploy_pool_type],
+                service_type=ServiceType[deploy_service_type],
+            )
+        trainer = LLMFinetune(
+            dataset=ds,
+            train_type=train_type,
+            event_handler=callback,
+            train_config=train_config_file,
+            deploy_config=deploy_config,
+            dataset_bos_path=dataset_bos_path,
+            previous_task_id=previous_task_id,
+        )
+        if trainer.train_action.train_config is None:
+            raise InternalError("Train config not found in trainer.")
+        if train_epoch is not None:
+            trainer.train_action.train_config.epoch = train_epoch
+        if train_batch_size is not None:
+            trainer.train_action.train_config.batch_size = train_batch_size
+        if train_learning_rate is not None:
+            trainer.train_action.train_config.learning_rate = train_learning_rate
+        if train_max_seq_len is not None:
+            trainer.train_action.train_config.max_seq_len = train_max_seq_len
+        if train_peft_type is not None:
+            trainer.train_action.train_config.peft_type = train_peft_type
+        if trainset_rate is not None:
+            trainer.train_action.train_config.trainset_rate = trainset_rate
+        if train_logging_steps is not None:
+            trainer.train_action.train_config.logging_steps = train_logging_steps
+        if train_warmup_ratio is not None:
+            trainer.train_action.train_config.warmup_ratio = train_warmup_ratio
+        if train_weight_decay is not None:
+            trainer.train_action.train_config.weight_decay = train_weight_decay
+        if train_lora_rank is not None:
+            trainer.train_action.train_config.lora_rank = train_lora_rank
+        if train_lora_all_linear is not None:
+            trainer.train_action.train_config.lora_all_linear = train_lora_all_linear
+
+    if daemon:
+        trainer.start()
+        console.print(
+            f"trainer[{trainer.id}] started with pid:"
+            f" {trainer.info().get('process_id')}"
+        )
+        console.print(f"check running log in: {trainer.ppls[0]._get_log_path()}")
+    else:
+        trainer.run()
+        console.log("Trainer finished!")
+        console.log(Pretty(trainer.output))
+
+    # wait a second for the log to be flushed
+    time.sleep(0.1)
```

### Comparing `qianfan-0.3.8.2/qianfan/common/client/txt2img.py` & `qianfan-0.3.9/qianfan/common/client/txt2img.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/common/client/utils.py` & `qianfan-0.3.9/qianfan/common/client/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/common/hub/hub.py` & `qianfan-0.3.9/qianfan/common/hub/hub.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/common/hub/interface.py` & `qianfan-0.3.9/qianfan/common/hub/interface.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/common/persister/base.py` & `qianfan-0.3.9/qianfan/common/persister/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/common/persister/persist.py` & `qianfan-0.3.9/qianfan/common/persister/persist.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/common/prompt/prompt.py` & `qianfan-0.3.9/qianfan/common/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/common/prompt/template.py` & `qianfan-0.3.9/qianfan/common/prompt/template.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/common/runnable/base.py` & `qianfan-0.3.9/qianfan/common/runnable/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/common/tool/baidu_search_tool.py` & `qianfan-0.3.9/qianfan/common/tool/baidu_search_tool.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/common/tool/base_tool.py` & `qianfan-0.3.9/qianfan/common/tool/base_tool.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/common/tool/duckduckgo_search_tool.py` & `qianfan-0.3.9/qianfan/common/tool/duckduckgo_search_tool.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/common/tool/wikipedia_tool.py` & `qianfan-0.3.9/qianfan/common/tool/wikipedia_tool.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/config.py` & `qianfan-0.3.9/qianfan/config.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/consts.py` & `qianfan-0.3.9/qianfan/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     AuthTimeout: float = 5
     DisableErnieBotSDK: bool = True
     IAMSignExpirationSeconds: int = 300
     ConsoleAPIBaseURL: str = "https://qianfan.baidubce.com"
     AccessTokenRefreshMinInterval: float = 3600
     InferResourceRefreshMinInterval: float = 600
     RetryCount: int = 3
-    RetryTimeout: float = 60
+    RetryTimeout: float = 300
     RetryBackoffFactor: float = 1
     RetryJitter: float = 1
     RetryMaxWaitInterval: float = 120
     ConsoleRetryCount: int = 1
     ConsoleRetryTimeout: float = 60
     ConsoleRetryBackoffFactor: float = 0
     ConsoleRetryJitter: int = 1
@@ -189,14 +189,18 @@
     FineTuneCreateJobAction: str = "CreateFineTuningJob"
     FineTuneCreateTaskAction: str = "CreateFineTuningTask"
     FineTuneJobListAction: str = "DescribeFineTuningJobs"
     FineTuneTaskListAction: str = "DescribeFineTuningTasks"
     FineTuneTaskDetailAction: str = "DescribeFineTuningTask"
     FineTuneStopTaskAction: str = "StopFineTuningTask"
     FineTuneSupportedModelsAction: str = "DescribeFineTuningSupportModels"
+    ServiceV2BaseRouteAPI: str = "/v2/service"
+    ServiceCreateAction: str = "CreateService"
+    ServiceListAction: str = "DescribeServices"
+    ServiceDetailAction: str = "DescribeService"
     ModelDetailAPI: str = "/wenxinworkshop/modelrepo/modelDetail"
     ModelVersionDetailAPI: str = "/wenxinworkshop/modelrepo/modelVersionDetail"
     ModelPublishAPI: str = "/wenxinworkshop/modelrepo/publishTrainModel"
     ModelEvalCreateAPI: str = "/wenxinworkshop/modelrepo/eval/create"
     ModelEvalInfoAPI: str = "/wenxinworkshop/modelrepo/eval/detail"
     ModelEvalResultAPI: str = "/wenxinworkshop/modelrepo/eval/report"
     ModelEvalStopAPI: str = "/wenxinworkshop/modelrepo/eval/cancel"
```

### Comparing `qianfan-0.3.8.2/qianfan/dataset/__init__.py` & `qianfan-0.3.9/qianfan/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/consts.py` & `qianfan-0.3.9/qianfan/dataset/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/data_insight/__init__.py` & `qianfan-0.3.9/qianfan/dataset/data_insight/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/data_insight/assets/index.html` & `qianfan-0.3.9/qianfan/dataset/data_insight/assets/index.html`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/data_insight/data_insight_utils.py` & `qianfan-0.3.9/qianfan/dataset/data_insight/data_insight_utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/data_insight/insight.py` & `qianfan-0.3.9/qianfan/dataset/data_insight/insight.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/data_operator.py` & `qianfan-0.3.9/qianfan/dataset/data_operator.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/data_source/__init__.py` & `qianfan-0.3.9/qianfan/dataset/data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/data_source/baidu_qianfan.py` & `qianfan-0.3.9/qianfan/dataset/data_source/baidu_qianfan.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/data_source/base.py` & `qianfan-0.3.9/qianfan/dataset/data_source/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/data_source/bos.py` & `qianfan-0.3.9/qianfan/dataset/data_source/bos.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/data_source/chunk_reader.py` & `qianfan-0.3.9/qianfan/dataset/data_source/chunk_reader.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/data_source/file.py` & `qianfan-0.3.9/qianfan/dataset/data_source/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,24 @@
 
 try:
     import clevercsv
 except ImportError:
     log_warn("clevercsv isn't installed, only online function can be used")
 
 
+def _remove_none_values(entry: Union[List[Dict[str, Any]], Dict[str, Any], str]) -> Any:
+    if isinstance(entry, str):
+        return entry
+
+    if isinstance(entry, dict):
+        return {k: v for k, v in entry.items() if v is not None}
+
+    return [_remove_none_values(item) for item in entry]
+
+
 class FileDataSource(DataSource, BaseModel):
     """file data source"""
 
     path: str
     file_format: Optional[FormatType] = Field(default=None)
 
     # Available only when 'file_format' is Text
@@ -63,30 +73,38 @@
         use_qianfan_special_jsonl_format: bool,
     ) -> None:
         lines: List[str] = []
         if self.file_format == FormatType.Json:
             if index != 0:
                 lines.append(",\n")
             for i in range(len(data)):
-                lines.append(json.dumps(data[i], ensure_ascii=False))
+                lines.append(
+                    json.dumps(_remove_none_values(data[i]), ensure_ascii=False)
+                )
                 if i != len(data) - 1:
                     lines.append(",\n")
 
             fd.writelines(lines)
 
         elif self.file_format == FormatType.Jsonl:
             if index != 0:
                 lines.append("\n")
 
             is_list = True if data and isinstance(data[0], list) else False
             for i in range(len(data)):
                 if use_qianfan_special_jsonl_format and not is_list:
-                    lines.append(f"[{json.dumps(data[i], ensure_ascii=False)}]")
+                    lines.append(
+                        "["
+                        + json.dumps(_remove_none_values(data[i]), ensure_ascii=False)
+                        + "]"
+                    )
                 else:
-                    lines.append(json.dumps(data[i], ensure_ascii=False))
+                    lines.append(
+                        json.dumps(_remove_none_values(data[i]), ensure_ascii=False)
+                    )
                 if i != len(data) - 1:
                     lines.append("\n")
 
             fd.writelines(lines)
 
         elif self.file_format == FormatType.Csv:
             assert isinstance(data[0], dict)
```

### Comparing `qianfan-0.3.8.2/qianfan/dataset/data_source/utils.py` & `qianfan-0.3.9/qianfan/dataset/data_source/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/dataset.py` & `qianfan-0.3.9/qianfan/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/dataset_utils.py` & `qianfan-0.3.9/qianfan/dataset/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/local_data_operators/__init__.py` & `qianfan-0.3.9/qianfan/dataset/local_data_operators/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/local_data_operators/base.py` & `qianfan-0.3.9/qianfan/dataset/local_data_operators/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/local_data_operators/check_character_repetition_filter.py` & `qianfan-0.3.9/qianfan/dataset/local_data_operators/check_character_repetition_filter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/local_data_operators/check_flagged_words.py` & `qianfan-0.3.9/qianfan/dataset/local_data_operators/check_flagged_words.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/local_data_operators/check_sentence_length_filter.py` & `qianfan-0.3.9/qianfan/dataset/local_data_operators/check_sentence_length_filter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/local_data_operators/check_special_characters.py` & `qianfan-0.3.9/qianfan/dataset/local_data_operators/check_special_characters.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/local_data_operators/check_stopwords.py` & `qianfan-0.3.9/qianfan/dataset/local_data_operators/check_stopwords.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/local_data_operators/check_word_number.py` & `qianfan-0.3.9/qianfan/dataset/local_data_operators/check_word_number.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/local_data_operators/check_word_repetition_filter.py` & `qianfan-0.3.9/qianfan/dataset/local_data_operators/check_word_repetition_filter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/local_data_operators/consts.py` & `qianfan-0.3.9/qianfan/dataset/local_data_operators/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/local_data_operators/utils.py` & `qianfan-0.3.9/qianfan/dataset/local_data_operators/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/local_data_operators/word_list.py` & `qianfan-0.3.9/qianfan/dataset/local_data_operators/word_list.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/process_interface.py` & `qianfan-0.3.9/qianfan/dataset/process_interface.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/qianfan_data_operators.py` & `qianfan-0.3.9/qianfan/dataset/qianfan_data_operators.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/schema.py` & `qianfan-0.3.9/qianfan/dataset/schema.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/summarization_method.py` & `qianfan-0.3.9/qianfan/dataset/summarization_method.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/table.py` & `qianfan-0.3.9/qianfan/dataset/table.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/dataset/table_utils.py` & `qianfan-0.3.9/qianfan/dataset/table_utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/errors.py` & `qianfan-0.3.9/qianfan/errors.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/evaluation/__init__.py` & `qianfan-0.3.9/qianfan/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/evaluation/consts.py` & `qianfan-0.3.9/qianfan/evaluation/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/evaluation/evaluation_manager.py` & `qianfan-0.3.9/qianfan/evaluation/evaluation_manager.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/evaluation/evaluation_result.py` & `qianfan-0.3.9/qianfan/evaluation/evaluation_result.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/evaluation/evaluator.py` & `qianfan-0.3.9/qianfan/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/evaluation/local_evaluator.py` & `qianfan-0.3.9/qianfan/evaluation/local_evaluator.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/evaluation/opencompass_evaluator.py` & `qianfan-0.3.9/qianfan/evaluation/opencompass_evaluator.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/extensions/langchain/agents/baidu_qianfan_endpoint.py` & `qianfan-0.3.9/qianfan/extensions/langchain/agents/baidu_qianfan_endpoint.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/extensions/openai/adapter.py` & `qianfan-0.3.9/qianfan/extensions/openai/adapter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/extensions/semantic_kernel/__init__.py` & `qianfan-0.3.9/qianfan/extensions/semantic_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/extensions/semantic_kernel/connectors/qianfan_chat_completion.py` & `qianfan-0.3.9/qianfan/extensions/semantic_kernel/connectors/qianfan_chat_completion.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/extensions/semantic_kernel/connectors/qianfan_settings.py` & `qianfan-0.3.9/qianfan/extensions/semantic_kernel/connectors/qianfan_settings.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/extensions/semantic_kernel/connectors/qianfan_text_completion.py` & `qianfan-0.3.9/qianfan/extensions/semantic_kernel/connectors/qianfan_text_completion.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/extensions/semantic_kernel/connectors/qianfan_text_embedding.py` & `qianfan-0.3.9/qianfan/extensions/semantic_kernel/connectors/qianfan_text_embedding.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/fake_pyarrow_replacer.py` & `qianfan-0.3.9/qianfan/fake_pyarrow_replacer.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/model/__init__.py` & `qianfan-0.3.9/qianfan/model/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/model/configs.py` & `qianfan-0.3.9/qianfan/model/configs.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/model/consts.py` & `qianfan-0.3.9/qianfan/model/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/model/model.py` & `qianfan-0.3.9/qianfan/model/model.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/__init__.py` & `qianfan-0.3.9/qianfan/resources/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from qianfan.resources.console.service import Service
 from qianfan.resources.images.image2text import Image2Text
 from qianfan.resources.images.text2image import Text2Image
 from qianfan.resources.llm.chat_completion import ChatCompletion
 from qianfan.resources.llm.completion import Completion
 from qianfan.resources.llm.embedding import Embedding
 from qianfan.resources.llm.plugin import Plugin
+from qianfan.resources.llm.rerank import Reranker
 from qianfan.resources.tools.tokenizer import Tokenizer
 from qianfan.resources.typing import QfMessages, QfResponse, QfRole
 
 __all__ = [
     "Data",
     "Model",
     "Service",
@@ -34,14 +35,15 @@
     "ChatCompletion",
     "Embedding",
     "Completion",
     "Plugin",
     "Text2Image",
     "Image2Text",
     "Tokenizer",
+    "Reranker",
     "AK",
     "SK",
     "Role",
     "Messages",
     "Response",
     "QfRole",
     "QfMessages",
```

### Comparing `qianfan-0.3.8.2/qianfan/resources/auth/iam.py` & `qianfan-0.3.9/qianfan/resources/auth/iam.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/auth/oauth.py` & `qianfan-0.3.9/qianfan/resources/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/console/charge.py` & `qianfan-0.3.9/qianfan/resources/console/charge.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/console/consts.py` & `qianfan-0.3.9/qianfan/resources/console/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 
 
 class DataTemplateType(int, Enum):
     """
     Template type used by Qianfan Data
     """
 
+    PromptChosenRejected: int = 2002
+    """对话偏好问答"""
     NonSortedConversation: int = 2000
     """非排序对话"""
     SortedConversation: int = 2001
     """含排序对话"""
     GenericText: int = 40100
     """泛文本"""
     QuerySet: int = 40200
```

### Comparing `qianfan-0.3.8.2/qianfan/resources/console/data.py` & `qianfan-0.3.9/qianfan/resources/console/data.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/console/finetune.py` & `qianfan-0.3.9/qianfan/resources/console/finetune.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/console/model.py` & `qianfan-0.3.9/qianfan/resources/console/model.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/console/prompt.py` & `qianfan-0.3.9/qianfan/resources/console/prompt.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/console/service.py` & `qianfan-0.3.9/qianfan/resources/tools/tokenizer.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,152 +9,143 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Service API
+Tokenizer
 """
 
-from typing import Any, List, Optional, Union
+import unicodedata
+from typing import Any
 
+from qianfan import get_config
 from qianfan.consts import Consts
-from qianfan.errors import InvalidArgumentError
-from qianfan.resources.console.consts import DeployPoolType, ServiceType
-from qianfan.resources.console.utils import console_api_request
-from qianfan.resources.typing import QfRequest
+from qianfan.errors import InternalError, InvalidArgumentError
+from qianfan.resources.tools.utils import qianfan_api_request
+from qianfan.resources.typing import Literal, QfRequest
 
 
-class Service(object):
+class Tokenizer(object):
     """
-    Class for Service API
+    Class for Tokenizer API
     """
 
     @classmethod
-    @console_api_request
-    def create(
+    def count_tokens(
         cls,
-        model_id: Union[int, str],
-        model_version_id: Union[int, str],
-        name: str,
-        uri: str,
-        replicas: int,
-        pool_type: DeployPoolType = DeployPoolType.PrivateResource,
-        description: Optional[str] = None,
-        **kwargs: Any
-    ) -> QfRequest:
+        text: str,
+        mode: Literal["local", "remote"] = "local",
+        model: str = "ERNIE-Bot",
+        **kwargs: Any,
+    ) -> int:
         """
-        Create a service for the given model.
-
-        This function creates a service associated with the specified model and
-        iteration.
+        Count the number of tokens in a given text.
 
         Parameters:
-          model_id (int):
-            The ID of the model for which the service is to be created.
-          model_version_id (int):
-            The ID of the version of the model.
-          name (str):
-            The name for the created service.
-          uri (str):
-            The URI (Uniform Resource Identifier) for accessing the service.
-          replicas (int):
-            The number of replicas for the service.
-          pool_type (int):
-            The type of pooling for the service (1 for public and 2 for private).
-          description (Optional[str], optional):
-            An optional description for the service.
+          text (str):
+            The input text for which tokens need to be counted.
+          mode (str, optional):
+            `local` (default):
+              local **SIMULATION**
+              (Chinese characters count * 0.625 + English word count * 1)
+            `remote`:
+              use qianfan api to calculate the token count. API will return accurate
+              token count, but only ERNIE-Bot series models are supported.
+          model (str, optional):
+            The name of the model to be used for token counting, which
+            may influence the counting strategy. Default is 'ERNIE-Bot'.
           kwargs (Any):
             Additional keyword arguments that can be passed to customize the request.
 
-        Note:
-        The `@console_api_request` decorator is applied to this method, enabling it to
-        send the generated QfRequest and return a QfResponse to the user.
-
-        API Doc: https://cloud.baidu.com/doc/WENXINWORKSHOP/s/Plnlmxdgy
-        """
-        req = QfRequest(method="POST", url=Consts.ServiceCreateAPI)
-        req.json_body = {
-            "modelId": model_id,
-            "modelVersionId": model_version_id,
-            "name": name,
-            "uri": uri,
-            "replicas": replicas,
-            "poolType": pool_type.value,
-            **kwargs,
-        }
-        if description is not None:
-            req.json_body["description"] = description
-        return req
+        """
+        if mode not in ["local", "remote"]:
+            raise InvalidArgumentError(
+                f"Mode `{mode}` is not supported for count token, supported mode:"
+                " `local`"
+            )
+        if mode == "local":
+            return cls._local_count_tokens(text, **kwargs)
+        if mode == "remote":
+            return cls._remote_count_tokens_eb(text, model, **kwargs)
+
+        # unreachable
+        raise InternalError
+
+    @staticmethod
+    @qianfan_api_request
+    def _eb_tokenizer(text: str, model: str = "ERNIE-Bot", **kwargs: Any) -> QfRequest:
+        """
+        create the request and use `qianfan_api_request` to get the response
+        """
+        request = QfRequest(
+            method="POST", url=get_config().BASE_URL + Consts.EBTokenizerAPI
+        )
+        request.json_body = {"prompt": text, "model": model, **kwargs}
+        return request
 
     @classmethod
-    @console_api_request
-    def get(cls, id: int, **kwargs: Any) -> QfRequest:
+    def _remote_count_tokens_eb(cls, text: str, model: str, **kwargs: Any) -> int:
         """
-        Retrieve information for a specific service.
-
-        This method allows retrieval of information pertaining to a specific service
-        based on its unique identifier.
-
-        Parameters:
-          id (int):
-            The unique identifier for the service.
-          kwargs (Any):
-            Additional keyword arguments that can be passed to customize the request.
-
-        Note:
-        The `@console_api_request` decorator is applied to this method, enabling it to
-        send the generated QfRequest and return a QfResponse to the user.
-
-        API Doc: https://cloud.baidu.com/doc/WENXINWORKSHOP/s/llnlmyp8o
-        """
-        req = QfRequest(method="POST", url=Consts.ServiceDetailAPI)
-        req.json_body = {
-            "serviceId": id,
-            **kwargs,
-        }
-        return req
+        call the api to get the token count
+        """
+        resp = cls._eb_tokenizer(text, model, **kwargs)
+        return resp["usage"]["total_tokens"]
 
     @classmethod
-    @console_api_request
-    def list(
+    def _local_count_tokens(
         cls,
-        api_type_filter: Optional[List[Union[str, ServiceType]]] = None,
-        **kwargs: Any
-    ) -> QfRequest:
-        """
-        list all services.
-
-        This method allows calling list API to get all services, including
-        `common`: preset model services.
-        `custom` user-deployed model services.
-
-        Parameters:
-          api_type_filter (Optional[List[str]]):
-            Optional, filter the services by ServiceType.
-              Concretely, the value of this parameter can be one or more of:
-                'chat', 'completions', 'embeddings', 'text2image', 'image2text'
-              If the value is `None`, all services will be returned.
-          kwargs (Any):
-            Additional keyword arguments that can be passed to customize the request.
-
-        Note:
-        The `@console_api_request` decorator is applied to this method, enabling it to
-        send the generated QfRequest and return a QfResponse to the user.
-
-        API Doc: https://cloud.baidu.com/doc/WENXINWORKSHOP/s/4lqoklvr1
-        """
-        req = QfRequest(method="POST", url=Consts.ServiceListAPI)
-        req.json_body = {
-            **kwargs,
-        }
-        if api_type_filter is not None:
-            for i, type in enumerate(api_type_filter):
-                if isinstance(type, str):
-                    pass
-                elif isinstance(type, ServiceType):
-                    api_type_filter[i] = type.value
-                else:
-                    raise InvalidArgumentError("Invalid api type: {}".format(type))
-            req.json_body["apiTypefilter"] = api_type_filter
-        return req
+        text: str,
+        model: str = "ERNIE-Bot",
+        han_tokens: float = 0.625,
+        word_tokens: float = 1,
+    ) -> int:
+        """
+        Calculate the token count for a given text using a local simulation.
+
+        ** THIS IS CALCULATED BY LOCAL SIMULATION, NOT REAL TOKEN COUNT **
+
+        The token count is computed as follows:
+        (Chinese characters count * 0.625) + (English word count * 1)
+        """
+        han_count = 0
+        text_only_word = ""
+        for ch in text:
+            if cls._is_cjk_character(ch):
+                han_count += 1
+                text_only_word += " "
+            elif cls._is_punctuation(ch) or cls._is_space(ch):
+                text_only_word += " "
+            else:
+                text_only_word += ch
+        word_count = len(list(filter(lambda x: x != "", text_only_word.split(" "))))
+        return int(han_count * han_tokens + word_count * word_tokens)
+
+    @staticmethod
+    def _is_cjk_character(ch: str) -> bool:
+        """
+        Check if the character is CJK character.
+        """
+        code = ord(ch)
+        return 0x4E00 <= code <= 0x9FFF
+
+    @staticmethod
+    def _is_space(ch: str) -> bool:
+        """
+        Check if the character is space.
+        """
+        return ch in {" ", "\n", "\r", "\t"} or unicodedata.category(ch) == "Zs"
+
+    @staticmethod
+    def _is_punctuation(ch: str) -> bool:
+        """
+        Check if the character is punctuation.
+        """
+        code = ord(ch)
+        return (
+            33 <= code <= 47
+            or 58 <= code <= 64
+            or 91 <= code <= 96
+            or 123 <= code <= 126
+            or unicodedata.category(ch).startswith("P")
+        )
```

### Comparing `qianfan-0.3.8.2/qianfan/resources/console/utils.py` & `qianfan-0.3.9/qianfan/resources/console/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/http_client.py` & `qianfan-0.3.9/qianfan/resources/http_client.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/images/image2text.py` & `qianfan-0.3.9/qianfan/resources/images/image2text.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/images/text2image.py` & `qianfan-0.3.9/qianfan/resources/images/text2image.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/llm/base.py` & `qianfan-0.3.9/qianfan/resources/llm/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/llm/chat_completion.py` & `qianfan-0.3.9/qianfan/resources/llm/chat_completion.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/llm/completion.py` & `qianfan-0.3.9/qianfan/resources/llm/completion.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/llm/embedding.py` & `qianfan-0.3.9/qianfan/resources/llm/embedding.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/llm/plugin.py` & `qianfan-0.3.9/qianfan/resources/llm/plugin.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/rate_limiter.py` & `qianfan-0.3.9/qianfan/resources/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/requestor/base.py` & `qianfan-0.3.9/qianfan/resources/requestor/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/requestor/console_requestor.py` & `qianfan-0.3.9/qianfan/resources/requestor/console_requestor.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/requestor/openapi_requestor.py` & `qianfan-0.3.9/qianfan/resources/requestor/openapi_requestor.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/token_limiter.py` & `qianfan-0.3.9/qianfan/resources/token_limiter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/tools/utils.py` & `qianfan-0.3.9/qianfan/resources/tools/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/resources/typing.py` & `qianfan-0.3.9/qianfan/resources/typing.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/trainer/__init__.py` & `qianfan-0.3.9/qianfan/trainer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from qianfan.trainer.actions import (
     BaseAction,
     DeployAction,
     LoadDataSetAction,
     ModelPublishAction,
     TrainAction,
 )
+from qianfan.trainer.dpo import DPO
 from qianfan.trainer.event import Event, EventHandler
 from qianfan.trainer.finetune import Finetune, LLMFinetune, Trainer
 from qianfan.trainer.post_pretrain import PostPreTrain
 
 __all__ = [
     "Finetune",
     "LLMFinetune",
@@ -30,8 +31,9 @@
     "EventHandler",
     "Event",
     "TrainAction",
     "LoadDataSetAction",
     "DeployAction",
     "ModelPublishAction",
     "PostPreTrain",
+    "DPO",
 ]
```

### Comparing `qianfan-0.3.8.2/qianfan/trainer/actions.py` & `qianfan-0.3.9/qianfan/trainer/actions.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/trainer/base.py` & `qianfan-0.3.9/qianfan/trainer/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/trainer/configs.py` & `qianfan-0.3.9/qianfan/trainer/configs.py`

 * *Files 8% similar despite different names*

```diff
@@ -438,29 +438,34 @@
                 learning_rate=(0.00001, 0.00004),
                 max_seq_len=[4096, 8192],
             ),
         },
         deprecated=True,
     ),
     "Qianfan-Chinese-Llama-2-13B": ModelInfo(
+        model="Qianfan-Chinese-Llama-2-13B-v1",
         short_name="Llama2_13b",
         base_model_type="Llama-2",
         support_peft_types=[PeftType.ALL],
         common_params_limit=TrainLimit(),
         specific_peft_types_params_limit={
             PeftType.ALL: TrainLimit(
                 batch_size=(48, 960),
                 epoch=(1, 1),
                 learning_rate=(0.0000002, 0.0002),
                 weight_decay=(0.0001, 0.05),
             ),
         },
+        deprecated=True,
     ),
 }
 
+
+DPOTrainModelInfoMapping: Dict[str, ModelInfo] = {}
+
 # model train type -> default train config
 ModelInfoMapping: Dict[str, ModelInfo] = {
     "ERNIE-Speed": ModelInfo(
         model="ERNIE-Speed-8K",
         short_name="ERNIE_Speed",
         base_model_type="ERNIE Speed",
         support_peft_types=[PeftType.ALL, PeftType.LoRA],
@@ -834,15 +839,15 @@
             batch_size=192,
             learning_rate=0.000020,
             weight_decay=0.01,
         )
     },
 }
 
-tc = TrainConfig(learning_rate=0.333)
+DefaultDPOTrainConfigMapping: Dict[str, TrainConfig] = {}
 
 # finetune model train type -> default finetune train config
 DefaultTrainConfigMapping: Dict[str, Dict[PeftType, TrainConfig]] = {
     "ERNIE-Speed": {
         PeftType.ALL: TrainConfig(
             epoch=1,
             learning_rate=0.00003,
@@ -1148,31 +1153,41 @@
         # 更新模型的类型和校验参数
         sft_model_info = _get_online_supported_model_info_mapping(
             model_info_list, console_consts.TrainMode.SFT
         )
         ppt_model_info = _get_online_supported_model_info_mapping(
             model_info_list, console_consts.TrainMode.PostPretrain
         )
+        dpo_model_info = _get_online_supported_model_info_mapping(
+            model_info_list, console_consts.TrainMode.DPO
+        )
         # 更新模型默认配置：
         default_configs_mapping = _update_default_config(model_info_list)
     except Exception:
         return
     global ModelInfoMapping
     ModelInfoMapping = {**ModelInfoMapping, **sft_model_info}
     global PostPreTrainModelInfoMapping
     PostPreTrainModelInfoMapping = {
         **PostPreTrainModelInfoMapping,
         **ppt_model_info,
     }
+    global DPOTrainModelInfoMapping
+    DPOTrainModelInfoMapping = {**DPOTrainModelInfoMapping, **dpo_model_info}
     global DefaultTrainConfigMapping
     DefaultTrainConfigMapping = {
         **DefaultTrainConfigMapping,
         **default_configs_mapping[console_consts.TrainMode.SFT],
     }
     global DefaultPostPretrainTrainConfigMapping
     DefaultPostPretrainTrainConfigMapping = {
         **DefaultPostPretrainTrainConfigMapping,
         **default_configs_mapping[console_consts.TrainMode.PostPretrain],
     }
+    global DefaultDPOTrainConfigMapping
+    DefaultDPOTrainConfigMapping = {
+        **DefaultDPOTrainConfigMapping,
+        **default_configs_mapping[console_consts.TrainMode.DPO],
+    }
 
 
 update_all_train_configs()
```

### Comparing `qianfan-0.3.8.2/qianfan/trainer/consts.py` & `qianfan-0.3.9/qianfan/trainer/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/trainer/event.py` & `qianfan-0.3.9/qianfan/trainer/event.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/trainer/finetune.py` & `qianfan-0.3.9/qianfan/trainer/finetune.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,14 +197,15 @@
         ppl = Pipeline(
             actions=actions,
             event_handler=event_handler,
             case_init_params={"case_type": Finetune.__name__},
         )
         self.ppls = [ppl]
         self.result = [None]
+        g_persister.save(ppl)
 
     def from_ppl(self, ppl: Optional[Pipeline]) -> "Trainer":
         """
         create a trainer from pipeline.
         Returns:
             Trainer: self, for chain invocation.
         """
```

### Comparing `qianfan-0.3.8.2/qianfan/trainer/pipeline.py` & `qianfan-0.3.9/qianfan/trainer/pipeline.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/trainer/post_pretrain.py` & `qianfan-0.3.9/qianfan/trainer/post_pretrain.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/trainer/ppl.yaml` & `qianfan-0.3.9/qianfan/trainer/ppl.yaml`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/trainer/trainer.py` & `qianfan-0.3.9/qianfan/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/utils/__init__.py` & `qianfan-0.3.9/qianfan/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/utils/bos_uploader.py` & `qianfan-0.3.9/qianfan/utils/bos_uploader.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/utils/cache/__init__.py` & `qianfan-0.3.9/qianfan/utils/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/utils/cache/base.py` & `qianfan-0.3.9/qianfan/utils/cache/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/utils/fake_pyarrow/__init__.py` & `qianfan-0.3.9/qianfan/utils/fake_pyarrow/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/utils/fake_pyarrow/compute.py` & `qianfan-0.3.9/qianfan/utils/fake_pyarrow/compute.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/utils/fake_pyarrow/functions.py` & `qianfan-0.3.9/qianfan/utils/fake_pyarrow/functions.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/utils/fake_pyarrow/ipc.py` & `qianfan-0.3.9/qianfan/utils/fake_pyarrow/ipc.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/utils/fake_pyarrow/table.py` & `qianfan-0.3.9/qianfan/utils/fake_pyarrow/table.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/utils/helper.py` & `qianfan-0.3.9/qianfan/utils/helper.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/utils/logging.py` & `qianfan-0.3.9/qianfan/utils/logging.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/utils/pydantic/__init__.py` & `qianfan-0.3.9/qianfan/utils/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/utils/utils.py` & `qianfan-0.3.9/qianfan/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/qianfan/version.py` & `qianfan-0.3.9/qianfan/version.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.8.2/PKG-INFO` & `qianfan-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qianfan
-Version: 0.3.8.2
+Version: 0.3.9
 Summary: 文心千帆大模型平台 Python SDK
 Home-page: https://cloud.baidu.com/product/wenxinworkshop
 License: Apache-2.0
 Keywords: baidu,qianfan
 Requires-Python: >=3.7,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

