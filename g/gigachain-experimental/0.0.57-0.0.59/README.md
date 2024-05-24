# Comparing `tmp/gigachain_experimental-0.0.57.tar.gz` & `tmp/gigachain_experimental-0.0.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigachain_experimental-0.0.57.tar", max compression
+gzip compressed data, was "gigachain_experimental-0.0.59.tar", max compression
```

## Comparing `gigachain_experimental-0.0.57.tar` & `gigachain_experimental-0.0.59.tar`

### file list

```diff
@@ -1,159 +1,159 @@
--rw-r--r--   0        0        0     1067 2023-12-18 12:05:46.761829 gigachain_experimental-0.0.57/LICENSE
--rw-r--r--   0        0        0      731 2023-10-06 14:43:01.321479 gigachain_experimental-0.0.57/README.md
--rw-r--r--   0        0        0      271 2023-10-19 12:57:52.560036 gigachain_experimental-0.0.57/langchain_experimental/__init__.py
--rw-r--r--   0        0        0      643 2024-03-28 12:44:20.382264 gigachain_experimental-0.0.57/langchain_experimental/agents/__init__.py
--rw-r--r--   0        0        0      653 2023-11-10 13:07:49.949600 gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/__init__.py
--rw-r--r--   0        0        0       19 2023-10-30 16:05:53.796780 gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/csv/__init__.py
--rw-r--r--   0        0        0     2407 2024-02-22 08:54:03.015149 gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/csv/base.py
--rw-r--r--   0        0        0       22 2023-10-19 12:57:52.561598 gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/pandas/__init__.py
--rw-r--r--   0        0        0    11290 2024-03-28 12:44:20.383718 gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/pandas/base.py
--rw-r--r--   0        0        0     1113 2023-10-19 12:57:52.562307 gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/pandas/prompt.py
--rw-r--r--   0        0        0        0 2023-10-19 12:57:52.562706 gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/python/__init__.py
--rw-r--r--   0        0        0     2224 2024-01-18 15:16:40.505131 gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/python/base.py
--rw-r--r--   0        0        0      513 2023-10-19 12:57:52.563558 gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/python/prompt.py
--rw-r--r--   0        0        0       20 2023-10-19 12:57:52.564007 gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/spark/__init__.py
--rw-r--r--   0        0        0     2761 2024-01-18 15:16:40.506986 gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/spark/base.py
--rw-r--r--   0        0        0      295 2023-10-19 12:57:52.565847 gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/spark/prompt.py
--rw-r--r--   0        0        0       23 2023-10-19 12:57:52.566362 gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/xorbits/__init__.py
--rw-r--r--   0        0        0     3143 2024-01-18 15:16:40.507943 gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/xorbits/base.py
--rw-r--r--   0        0        0     1070 2023-10-19 12:57:52.567043 gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/xorbits/prompt.py
--rw-r--r--   0        0        0      866 2024-03-28 12:44:20.384386 gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/__init__.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.490847 gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/autogpt/__init__.py
--rw-r--r--   0        0        0     5443 2024-03-28 12:44:20.386884 gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/autogpt/agent.py
--rw-r--r--   0        0        0     1164 2024-02-22 08:54:03.020154 gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/autogpt/memory.py
--rw-r--r--   0        0        0     1909 2024-03-28 12:44:20.391604 gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/autogpt/output_parser.py
--rw-r--r--   0        0        0     5000 2024-02-22 08:54:03.022979 gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/autogpt/prompt.py
--rw-r--r--   0        0        0     7963 2024-03-28 12:44:20.393342 gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py
--rw-r--r--   0        0        0      514 2023-08-21 13:51:28.493975 gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/baby_agi/__init__.py
--rw-r--r--   0        0        0     8687 2024-02-22 08:54:03.024294 gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py
--rw-r--r--   0        0        0     1668 2024-03-28 12:44:20.393983 gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/baby_agi/task_creation.py
--rw-r--r--   0        0        0      967 2024-03-28 12:44:20.394699 gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/baby_agi/task_execution.py
--rw-r--r--   0        0        0     1283 2024-03-28 12:44:20.395266 gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.495536 gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/hugginggpt/__init__.py
--rw-r--r--   0        0        0     1133 2024-03-28 12:44:20.397027 gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py
--rw-r--r--   0        0        0     1742 2024-03-28 12:44:20.397664 gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py
--rw-r--r--   0        0        0     4598 2024-03-28 12:44:20.399096 gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py
--rw-r--r--   0        0        0     7859 2024-03-28 12:44:20.400788 gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py
--rw-r--r--   0        0        0      674 2024-03-28 12:44:20.401473 gigachain_experimental-0.0.57/langchain_experimental/chat_models/__init__.py
--rw-r--r--   0        0        0     6063 2024-03-28 12:44:20.402985 gigachain_experimental-0.0.57/langchain_experimental/chat_models/llm_wrapper.py
--rw-r--r--   0        0        0     2190 2024-03-28 12:44:20.403904 gigachain_experimental-0.0.57/langchain_experimental/comprehend_moderation/__init__.py
--rw-r--r--   0        0        0     6664 2024-04-10 15:22:17.420625 gigachain_experimental-0.0.57/langchain_experimental/comprehend_moderation/amazon_comprehend_moderation.py
--rw-r--r--   0        0        0     7411 2024-03-28 12:44:20.406460 gigachain_experimental-0.0.57/langchain_experimental/comprehend_moderation/base_moderation.py
--rw-r--r--   0        0        0     2390 2024-03-28 12:44:20.407747 gigachain_experimental-0.0.57/langchain_experimental/comprehend_moderation/base_moderation_callbacks.py
--rw-r--r--   0        0        0     1614 2024-03-28 12:44:20.409023 gigachain_experimental-0.0.57/langchain_experimental/comprehend_moderation/base_moderation_config.py
--rw-r--r--   0        0        0      192 2023-09-04 05:57:22.495380 gigachain_experimental-0.0.57/langchain_experimental/comprehend_moderation/base_moderation_enums.py
--rw-r--r--   0        0        0     1054 2024-03-28 12:44:20.409588 gigachain_experimental-0.0.57/langchain_experimental/comprehend_moderation/base_moderation_exceptions.py
--rw-r--r--   0        0        0     6834 2024-03-28 12:44:20.410890 gigachain_experimental-0.0.57/langchain_experimental/comprehend_moderation/pii.py
--rw-r--r--   0        0        0     3142 2024-03-28 12:44:20.411826 gigachain_experimental-0.0.57/langchain_experimental/comprehend_moderation/prompt_safety.py
--rw-r--r--   0        0        0     8134 2024-03-28 12:44:20.413206 gigachain_experimental-0.0.57/langchain_experimental/comprehend_moderation/toxicity.py
--rw-r--r--   0        0        0      103 2023-10-03 07:51:15.765558 gigachain_experimental-0.0.57/langchain_experimental/cpal/README.md
--rw-r--r--   0        0        0      750 2024-03-28 12:44:20.413845 gigachain_experimental-0.0.57/langchain_experimental/cpal/__init__.py
--rw-r--r--   0        0        0    11087 2024-03-28 12:44:20.415084 gigachain_experimental-0.0.57/langchain_experimental/cpal/base.py
--rw-r--r--   0        0        0      246 2023-08-21 13:51:28.498799 gigachain_experimental-0.0.57/langchain_experimental/cpal/constants.py
--rw-r--r--   0        0        0     9183 2024-03-28 12:44:20.416997 gigachain_experimental-0.0.57/langchain_experimental/cpal/models.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.499460 gigachain_experimental-0.0.57/langchain_experimental/cpal/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.499832 gigachain_experimental-0.0.57/langchain_experimental/cpal/templates/univariate/__init__.py
--rw-r--r--   0        0        0     2548 2023-10-19 12:57:52.577909 gigachain_experimental-0.0.57/langchain_experimental/cpal/templates/univariate/causal.py
--rw-r--r--   0        0        0      853 2023-10-19 12:57:52.579560 gigachain_experimental-0.0.57/langchain_experimental/cpal/templates/univariate/intervention.py
--rw-r--r--   0        0        0     2905 2023-10-19 12:57:52.581896 gigachain_experimental-0.0.57/langchain_experimental/cpal/templates/univariate/narrative.py
--rw-r--r--   0        0        0     5468 2023-10-19 12:57:52.583797 gigachain_experimental-0.0.57/langchain_experimental/cpal/templates/univariate/query.py
--rw-r--r--   0        0        0      631 2024-03-28 12:44:20.417734 gigachain_experimental-0.0.57/langchain_experimental/data_anonymizer/__init__.py
--rw-r--r--   0        0        0     1811 2024-03-28 12:44:20.419349 gigachain_experimental-0.0.57/langchain_experimental/data_anonymizer/base.py
--rw-r--r--   0        0        0     4793 2024-03-28 12:44:20.420547 gigachain_experimental-0.0.57/langchain_experimental/data_anonymizer/deanonymizer_mapping.py
--rw-r--r--   0        0        0     6801 2024-03-28 12:44:20.421773 gigachain_experimental-0.0.57/langchain_experimental/data_anonymizer/deanonymizer_matching_strategies.py
--rw-r--r--   0        0        0     2861 2024-03-28 12:44:20.422573 gigachain_experimental-0.0.57/langchain_experimental/data_anonymizer/faker_presidio_mapping.py
--rw-r--r--   0        0        0    17162 2024-03-28 12:44:20.423295 gigachain_experimental-0.0.57/langchain_experimental/data_anonymizer/presidio.py
--rw-r--r--   0        0        0      368 2024-03-28 12:44:20.423942 gigachain_experimental-0.0.57/langchain_experimental/fallacy_removal/__init__.py
--rw-r--r--   0        0        0      263 2024-03-28 12:44:20.424513 gigachain_experimental-0.0.57/langchain_experimental/generative_agents/__init__.py
--rw-r--r--   0        0        0    10252 2024-03-28 12:44:20.425251 gigachain_experimental-0.0.57/langchain_experimental/generative_agents/generative_agent.py
--rw-r--r--   0        0        0    13413 2024-03-28 12:44:20.425996 gigachain_experimental-0.0.57/langchain_experimental/generative_agents/memory.py
--rw-r--r--   0        0        0      308 2024-03-28 12:44:20.426581 gigachain_experimental-0.0.57/langchain_experimental/graph_transformers/__init__.py
--rw-r--r--   0        0        0    10723 2024-03-28 12:44:20.427932 gigachain_experimental-0.0.57/langchain_experimental/graph_transformers/diffbot.py
--rw-r--r--   0        0        0    12871 2024-04-10 15:22:17.421785 gigachain_experimental-0.0.57/langchain_experimental/graph_transformers/llm.py
--rw-r--r--   0        0        0       94 2024-03-28 12:44:20.429416 gigachain_experimental-0.0.57/langchain_experimental/llm_bash/__init__.py
--rw-r--r--   0        0        0     4454 2024-01-18 15:16:40.536504 gigachain_experimental-0.0.57/langchain_experimental/llm_bash/base.py
--rw-r--r--   0        0        0     5708 2024-03-28 12:44:20.431110 gigachain_experimental-0.0.57/langchain_experimental/llm_bash/bash.py
--rw-r--r--   0        0        0     2038 2024-03-28 12:44:20.431773 gigachain_experimental-0.0.57/langchain_experimental/llm_bash/prompt.py
--rw-r--r--   0        0        0      164 2024-03-28 12:44:20.432361 gigachain_experimental-0.0.57/langchain_experimental/llm_symbolic_math/__init__.py
--rw-r--r--   0        0        0     5791 2024-03-28 12:44:20.433601 gigachain_experimental-0.0.57/langchain_experimental/llm_symbolic_math/base.py
--rw-r--r--   0        0        0     1087 2023-10-06 14:43:01.344104 gigachain_experimental-0.0.57/langchain_experimental/llm_symbolic_math/prompt.py
--rw-r--r--   0        0        0      453 2024-03-28 12:44:20.434660 gigachain_experimental-0.0.57/langchain_experimental/llms/__init__.py
--rw-r--r--   0        0        0     8768 2024-03-28 12:44:20.436322 gigachain_experimental-0.0.57/langchain_experimental/llms/anthropic_functions.py
--rw-r--r--   0        0        0     2228 2024-03-28 12:44:20.438106 gigachain_experimental-0.0.57/langchain_experimental/llms/jsonformer_decoder.py
--rw-r--r--   0        0        0     4344 2024-03-28 12:44:20.439958 gigachain_experimental-0.0.57/langchain_experimental/llms/llamaapi.py
--rw-r--r--   0        0        0     2843 2024-03-28 12:44:20.440627 gigachain_experimental-0.0.57/langchain_experimental/llms/lmformatenforcer_decoder.py
--rw-r--r--   0        0        0     4932 2024-03-28 12:44:20.441319 gigachain_experimental-0.0.57/langchain_experimental/llms/ollama_functions.py
--rw-r--r--   0        0        0     2342 2024-03-28 12:44:20.441799 gigachain_experimental-0.0.57/langchain_experimental/llms/rellm_decoder.py
--rw-r--r--   0        0        0      346 2024-03-28 12:44:20.442410 gigachain_experimental-0.0.57/langchain_experimental/open_clip/__init__.py
--rw-r--r--   0        0        0     3383 2024-03-28 12:44:20.442806 gigachain_experimental-0.0.57/langchain_experimental/open_clip/open_clip.py
--rw-r--r--   0        0        0      120 2023-11-10 13:07:49.953805 gigachain_experimental-0.0.57/langchain_experimental/openai_assistant/__init__.py
--rw-r--r--   0        0        0      185 2023-11-15 10:30:09.322265 gigachain_experimental-0.0.57/langchain_experimental/openai_assistant/base.py
--rw-r--r--   0        0        0      330 2024-03-28 12:44:20.443329 gigachain_experimental-0.0.57/langchain_experimental/pal_chain/__init__.py
--rw-r--r--   0        0        0    13320 2024-03-28 12:44:20.444258 gigachain_experimental-0.0.57/langchain_experimental/pal_chain/base.py
--rw-r--r--   0        0        0     3537 2023-08-21 13:51:28.506235 gigachain_experimental-0.0.57/langchain_experimental/pal_chain/colored_object_prompt.py
--rw-r--r--   0        0        0     5767 2023-08-21 13:51:28.506905 gigachain_experimental-0.0.57/langchain_experimental/pal_chain/math_prompt.py
--rw-r--r--   0        0        0      488 2024-03-28 12:44:20.444965 gigachain_experimental-0.0.57/langchain_experimental/plan_and_execute/__init__.py
--rw-r--r--   0        0        0     3570 2023-08-21 13:51:28.507952 gigachain_experimental-0.0.57/langchain_experimental/plan_and_execute/agent_executor.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.508275 gigachain_experimental-0.0.57/langchain_experimental/plan_and_execute/executors/__init__.py
--rw-r--r--   0        0        0     1463 2024-01-18 15:16:40.555727 gigachain_experimental-0.0.57/langchain_experimental/plan_and_execute/executors/agent_executor.py
--rw-r--r--   0        0        0     1269 2023-08-21 13:51:28.508950 gigachain_experimental-0.0.57/langchain_experimental/plan_and_execute/executors/base.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.509270 gigachain_experimental-0.0.57/langchain_experimental/plan_and_execute/planners/__init__.py
--rw-r--r--   0        0        0     1567 2023-08-21 13:51:28.509627 gigachain_experimental-0.0.57/langchain_experimental/plan_and_execute/planners/base.py
--rw-r--r--   0        0        0     2314 2024-01-18 15:16:40.558911 gigachain_experimental-0.0.57/langchain_experimental/plan_and_execute/planners/chat_planner.py
--rw-r--r--   0        0        0     1439 2024-03-28 12:44:20.445521 gigachain_experimental-0.0.57/langchain_experimental/plan_and_execute/schema.py
--rw-r--r--   0        0        0      369 2024-03-28 12:44:20.446237 gigachain_experimental-0.0.57/langchain_experimental/prompt_injection_identifier/__init__.py
--rw-r--r--   0        0        0     3369 2024-03-28 12:44:20.447465 gigachain_experimental-0.0.57/langchain_experimental/prompt_injection_identifier/hugging_face_identifier.py
--rw-r--r--   0        0        0      174 2024-03-28 12:44:20.448585 gigachain_experimental-0.0.57/langchain_experimental/prompts/__init__.py
--rw-r--r--   0        0        0       77 2024-04-10 15:22:17.422607 gigachain_experimental-0.0.57/langchain_experimental/prompts/load.py
--rw-r--r--   0        0        0        0 2023-08-22 08:04:55.368181 gigachain_experimental-0.0.57/langchain_experimental/py.typed
--rw-r--r--   0        0        0     1285 2023-08-24 07:36:02.836411 gigachain_experimental-0.0.57/langchain_experimental/pydantic_v1/__init__.py
--rw-r--r--   0        0        0      548 2023-08-24 07:36:02.836900 gigachain_experimental-0.0.57/langchain_experimental/pydantic_v1/dataclasses.py
--rw-r--r--   0        0        0      520 2023-08-24 07:36:02.837404 gigachain_experimental-0.0.57/langchain_experimental/pydantic_v1/main.py
--rw-r--r--   0        0        0      518 2024-03-28 12:44:20.449970 gigachain_experimental-0.0.57/langchain_experimental/recommenders/__init__.py
--rw-r--r--   0        0        0     7967 2024-03-28 12:44:20.450624 gigachain_experimental-0.0.57/langchain_experimental/recommenders/amazon_personalize.py
--rw-r--r--   0        0        0     6964 2024-03-28 12:44:20.451327 gigachain_experimental-0.0.57/langchain_experimental/recommenders/amazon_personalize_chain.py
--rw-r--r--   0        0        0      200 2024-03-28 12:44:20.452015 gigachain_experimental-0.0.57/langchain_experimental/retrievers/__init__.py
--rw-r--r--   0        0        0     1248 2024-03-28 12:44:20.453407 gigachain_experimental-0.0.57/langchain_experimental/retrievers/vector_sql_database.py
--rw-r--r--   0        0        0     1447 2024-03-28 12:44:20.454189 gigachain_experimental-0.0.57/langchain_experimental/rl_chain/__init__.py
--rw-r--r--   0        0        0    23241 2024-03-28 12:44:20.455891 gigachain_experimental-0.0.57/langchain_experimental/rl_chain/base.py
--rw-r--r--   0        0        0     1989 2024-03-28 12:44:20.456634 gigachain_experimental-0.0.57/langchain_experimental/rl_chain/metrics.py
--rw-r--r--   0        0        0     2126 2024-03-28 12:44:20.457637 gigachain_experimental-0.0.57/langchain_experimental/rl_chain/model_repository.py
--rw-r--r--   0        0        0    16279 2024-03-28 12:44:20.459002 gigachain_experimental-0.0.57/langchain_experimental/rl_chain/pick_best_chain.py
--rw-r--r--   0        0        0      556 2024-03-28 12:44:20.459800 gigachain_experimental-0.0.57/langchain_experimental/rl_chain/vw_logger.py
--rw-r--r--   0        0        0      946 2024-03-28 12:44:20.460545 gigachain_experimental-0.0.57/langchain_experimental/smart_llm/__init__.py
--rw-r--r--   0        0        0    14423 2024-03-28 12:44:20.462679 gigachain_experimental-0.0.57/langchain_experimental/smart_llm/base.py
--rw-r--r--   0        0        0      202 2024-03-28 12:44:20.463580 gigachain_experimental-0.0.57/langchain_experimental/sql/__init__.py
--rw-r--r--   0        0        0    13247 2024-04-10 15:22:17.423800 gigachain_experimental-0.0.57/langchain_experimental/sql/base.py
--rw-r--r--   0        0        0     4658 2023-09-25 07:40:35.486005 gigachain_experimental-0.0.57/langchain_experimental/sql/prompt.py
--rw-r--r--   0        0        0     9846 2024-03-28 12:44:20.464697 gigachain_experimental-0.0.57/langchain_experimental/sql/vector_sql.py
--rw-r--r--   0        0        0     1576 2024-03-28 12:44:20.465321 gigachain_experimental-0.0.57/langchain_experimental/synthetic_data/__init__.py
--rw-r--r--   0        0        0      459 2023-09-25 07:40:35.486981 gigachain_experimental-0.0.57/langchain_experimental/synthetic_data/prompts.py
--rw-r--r--   0        0        0       75 2024-03-28 12:44:20.465865 gigachain_experimental-0.0.57/langchain_experimental/tabular_synthetic_data/__init__.py
--rw-r--r--   0        0        0     5341 2024-03-28 12:44:20.466662 gigachain_experimental-0.0.57/langchain_experimental/tabular_synthetic_data/base.py
--rw-r--r--   0        0        0     2523 2024-03-28 12:44:20.467247 gigachain_experimental-0.0.57/langchain_experimental/tabular_synthetic_data/openai.py
--rw-r--r--   0        0        0      412 2023-10-03 07:51:15.769901 gigachain_experimental-0.0.57/langchain_experimental/tabular_synthetic_data/prompts.py
--rw-r--r--   0        0        0     9717 2024-03-28 12:44:20.468288 gigachain_experimental-0.0.57/langchain_experimental/text_splitter.py
--rw-r--r--   0        0        0      180 2024-03-28 12:44:20.469622 gigachain_experimental-0.0.57/langchain_experimental/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-10-19 12:57:52.604149 gigachain_experimental-0.0.57/langchain_experimental/tools/python/__init__.py
--rw-r--r--   0        0        0     4763 2024-03-28 12:44:20.471048 gigachain_experimental-0.0.57/langchain_experimental/tools/python/tool.py
--rw-r--r--   0        0        0      425 2024-03-28 12:44:20.471866 gigachain_experimental-0.0.57/langchain_experimental/tot/__init__.py
--rw-r--r--   0        0        0     4853 2024-03-28 12:44:20.473425 gigachain_experimental-0.0.57/langchain_experimental/tot/base.py
--rw-r--r--   0        0        0     1405 2023-08-21 13:51:28.514934 gigachain_experimental-0.0.57/langchain_experimental/tot/checker.py
--rw-r--r--   0        0        0     1666 2023-08-21 13:51:28.515184 gigachain_experimental-0.0.57/langchain_experimental/tot/controller.py
--rw-r--r--   0        0        0     1467 2024-03-28 12:44:20.474461 gigachain_experimental-0.0.57/langchain_experimental/tot/memory.py
--rw-r--r--   0        0        0     4797 2024-03-28 12:44:20.475292 gigachain_experimental-0.0.57/langchain_experimental/tot/prompts.py
--rw-r--r--   0        0        0      504 2024-03-28 12:44:20.475874 gigachain_experimental-0.0.57/langchain_experimental/tot/thought.py
--rw-r--r--   0        0        0     3118 2024-03-28 12:44:20.476518 gigachain_experimental-0.0.57/langchain_experimental/tot/thought_generation.py
--rw-r--r--   0        0        0      148 2024-03-28 12:44:20.477224 gigachain_experimental-0.0.57/langchain_experimental/utilities/__init__.py
--rw-r--r--   0        0        0     2154 2023-10-19 12:57:52.605471 gigachain_experimental-0.0.57/langchain_experimental/utilities/python.py
--rw-r--r--   0        0        0      114 2024-04-10 15:22:17.424205 gigachain_experimental-0.0.57/langchain_experimental/video_captioning/__init__.py
--rw-r--r--   0        0        0     5034 2024-04-10 15:22:17.424804 gigachain_experimental-0.0.57/langchain_experimental/video_captioning/base.py
--rw-r--r--   0        0        0     4880 2024-04-10 15:22:17.425373 gigachain_experimental-0.0.57/langchain_experimental/video_captioning/models.py
--rw-r--r--   0        0        0     4369 2024-04-10 15:22:17.425922 gigachain_experimental-0.0.57/langchain_experimental/video_captioning/prompts.py
--rw-r--r--   0        0        0     3191 2024-04-10 15:22:17.426355 gigachain_experimental-0.0.57/langchain_experimental/video_captioning/services/audio_service.py
--rw-r--r--   0        0        0    11296 2024-04-10 15:22:17.427175 gigachain_experimental-0.0.57/langchain_experimental/video_captioning/services/caption_service.py
--rw-r--r--   0        0        0     4927 2024-04-10 15:22:17.427729 gigachain_experimental-0.0.57/langchain_experimental/video_captioning/services/combine_service.py
--rw-r--r--   0        0        0     3773 2024-04-10 15:22:17.428208 gigachain_experimental-0.0.57/langchain_experimental/video_captioning/services/image_service.py
--rw-r--r--   0        0        0      459 2024-04-10 15:22:17.428557 gigachain_experimental-0.0.57/langchain_experimental/video_captioning/services/srt_service.py
--rw-r--r--   0        0        0     3988 2024-04-11 07:25:45.794639 gigachain_experimental-0.0.57/pyproject.toml
--rw-r--r--   0        0        0     2076 1970-01-01 00:00:00.000000 gigachain_experimental-0.0.57/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-12-18 12:05:46.761829 gigachain_experimental-0.0.59/LICENSE
+-rw-r--r--   0        0        0      731 2023-10-06 14:43:01.321479 gigachain_experimental-0.0.59/README.md
+-rw-r--r--   0        0        0      271 2023-10-19 12:57:52.560036 gigachain_experimental-0.0.59/langchain_experimental/__init__.py
+-rw-r--r--   0        0        0      643 2024-04-19 07:38:33.791741 gigachain_experimental-0.0.59/langchain_experimental/agents/__init__.py
+-rw-r--r--   0        0        0      653 2023-11-10 13:07:49.949600 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/__init__.py
+-rw-r--r--   0        0        0       19 2023-10-30 16:05:53.796780 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/csv/__init__.py
+-rw-r--r--   0        0        0     2407 2024-02-22 08:54:03.015149 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/csv/base.py
+-rw-r--r--   0        0        0       22 2023-10-19 12:57:52.561598 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/pandas/__init__.py
+-rw-r--r--   0        0        0    11933 2024-05-06 14:45:38.336392 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/pandas/base.py
+-rw-r--r--   0        0        0     1113 2023-10-19 12:57:52.562307 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/pandas/prompt.py
+-rw-r--r--   0        0        0        0 2023-10-19 12:57:52.562706 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/python/__init__.py
+-rw-r--r--   0        0        0     2229 2024-04-19 07:38:33.794226 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/python/base.py
+-rw-r--r--   0        0        0      513 2023-10-19 12:57:52.563558 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/python/prompt.py
+-rw-r--r--   0        0        0       20 2023-10-19 12:57:52.564007 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/spark/__init__.py
+-rw-r--r--   0        0        0     2766 2024-04-19 07:38:33.794958 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/spark/base.py
+-rw-r--r--   0        0        0      295 2023-10-19 12:57:52.565847 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/spark/prompt.py
+-rw-r--r--   0        0        0       23 2023-10-19 12:57:52.566362 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/xorbits/__init__.py
+-rw-r--r--   0        0        0     3148 2024-04-19 07:38:33.795570 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/xorbits/base.py
+-rw-r--r--   0        0        0     1070 2023-10-19 12:57:52.567043 gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/xorbits/prompt.py
+-rw-r--r--   0        0        0      866 2024-04-19 07:38:33.796200 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.490847 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/autogpt/__init__.py
+-rw-r--r--   0        0        0     5448 2024-05-06 14:45:38.337698 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/autogpt/agent.py
+-rw-r--r--   0        0        0     1148 2024-05-06 14:45:38.338529 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/autogpt/memory.py
+-rw-r--r--   0        0        0     1909 2024-03-28 12:44:20.391604 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/autogpt/output_parser.py
+-rw-r--r--   0        0        0     4989 2024-05-06 14:45:38.339455 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/autogpt/prompt.py
+-rw-r--r--   0        0        0     7963 2024-03-28 12:44:20.393342 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py
+-rw-r--r--   0        0        0      514 2023-08-21 13:51:28.493975 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/baby_agi/__init__.py
+-rw-r--r--   0        0        0     8692 2024-04-19 07:38:33.797136 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py
+-rw-r--r--   0        0        0     1668 2024-04-19 07:38:33.797963 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/baby_agi/task_creation.py
+-rw-r--r--   0        0        0      967 2024-04-19 07:38:33.798539 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/baby_agi/task_execution.py
+-rw-r--r--   0        0        0     1283 2024-04-19 07:38:33.799080 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.495536 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/hugginggpt/__init__.py
+-rw-r--r--   0        0        0     1133 2024-03-28 12:44:20.397027 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py
+-rw-r--r--   0        0        0     1747 2024-04-19 07:38:33.800134 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py
+-rw-r--r--   0        0        0     4631 2024-05-06 14:45:38.340696 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py
+-rw-r--r--   0        0        0     7869 2024-05-06 14:45:38.342283 gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py
+-rw-r--r--   0        0        0      674 2024-04-19 07:38:33.803295 gigachain_experimental-0.0.59/langchain_experimental/chat_models/__init__.py
+-rw-r--r--   0        0        0     6068 2024-04-19 07:38:33.804258 gigachain_experimental-0.0.59/langchain_experimental/chat_models/llm_wrapper.py
+-rw-r--r--   0        0        0     2190 2024-04-19 07:38:33.804875 gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/__init__.py
+-rw-r--r--   0        0        0     6669 2024-04-19 07:38:33.805769 gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/amazon_comprehend_moderation.py
+-rw-r--r--   0        0        0     7416 2024-04-19 07:38:33.806215 gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/base_moderation.py
+-rw-r--r--   0        0        0     2390 2024-03-28 12:44:20.407747 gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/base_moderation_callbacks.py
+-rw-r--r--   0        0        0     1614 2024-03-28 12:44:20.409023 gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/base_moderation_config.py
+-rw-r--r--   0        0        0      192 2023-09-04 05:57:22.495380 gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/base_moderation_enums.py
+-rw-r--r--   0        0        0     1054 2024-03-28 12:44:20.409588 gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/base_moderation_exceptions.py
+-rw-r--r--   0        0        0     6834 2024-03-28 12:44:20.410890 gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/pii.py
+-rw-r--r--   0        0        0     3142 2024-03-28 12:44:20.411826 gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/prompt_safety.py
+-rw-r--r--   0        0        0     8134 2024-03-28 12:44:20.413206 gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/toxicity.py
+-rw-r--r--   0        0        0      103 2023-10-03 07:51:15.765558 gigachain_experimental-0.0.59/langchain_experimental/cpal/README.md
+-rw-r--r--   0        0        0      750 2024-04-19 07:38:33.806637 gigachain_experimental-0.0.59/langchain_experimental/cpal/__init__.py
+-rw-r--r--   0        0        0    11097 2024-05-06 14:45:38.343644 gigachain_experimental-0.0.59/langchain_experimental/cpal/base.py
+-rw-r--r--   0        0        0      246 2023-08-21 13:51:28.498799 gigachain_experimental-0.0.59/langchain_experimental/cpal/constants.py
+-rw-r--r--   0        0        0     9183 2024-03-28 12:44:20.416997 gigachain_experimental-0.0.59/langchain_experimental/cpal/models.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.499460 gigachain_experimental-0.0.59/langchain_experimental/cpal/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.499832 gigachain_experimental-0.0.59/langchain_experimental/cpal/templates/univariate/__init__.py
+-rw-r--r--   0        0        0     2548 2023-10-19 12:57:52.577909 gigachain_experimental-0.0.59/langchain_experimental/cpal/templates/univariate/causal.py
+-rw-r--r--   0        0        0      853 2023-10-19 12:57:52.579560 gigachain_experimental-0.0.59/langchain_experimental/cpal/templates/univariate/intervention.py
+-rw-r--r--   0        0        0     2905 2023-10-19 12:57:52.581896 gigachain_experimental-0.0.59/langchain_experimental/cpal/templates/univariate/narrative.py
+-rw-r--r--   0        0        0     5468 2023-10-19 12:57:52.583797 gigachain_experimental-0.0.59/langchain_experimental/cpal/templates/univariate/query.py
+-rw-r--r--   0        0        0      631 2024-04-19 07:38:33.808411 gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/__init__.py
+-rw-r--r--   0        0        0     1811 2024-03-28 12:44:20.419349 gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/base.py
+-rw-r--r--   0        0        0     4793 2024-03-28 12:44:20.420547 gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/deanonymizer_mapping.py
+-rw-r--r--   0        0        0     6801 2024-03-28 12:44:20.421773 gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/deanonymizer_matching_strategies.py
+-rw-r--r--   0        0        0     2861 2024-03-28 12:44:20.422573 gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/faker_presidio_mapping.py
+-rw-r--r--   0        0        0    17162 2024-03-28 12:44:20.423295 gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/presidio.py
+-rw-r--r--   0        0        0      368 2024-04-19 07:38:33.808667 gigachain_experimental-0.0.59/langchain_experimental/fallacy_removal/__init__.py
+-rw-r--r--   0        0        0      263 2024-04-19 07:38:33.809470 gigachain_experimental-0.0.59/langchain_experimental/generative_agents/__init__.py
+-rw-r--r--   0        0        0    10252 2024-04-19 07:38:33.810327 gigachain_experimental-0.0.59/langchain_experimental/generative_agents/generative_agent.py
+-rw-r--r--   0        0        0    13381 2024-05-06 14:45:38.345363 gigachain_experimental-0.0.59/langchain_experimental/generative_agents/memory.py
+-rw-r--r--   0        0        0      308 2024-04-19 07:38:33.811851 gigachain_experimental-0.0.59/langchain_experimental/graph_transformers/__init__.py
+-rw-r--r--   0        0        0    13383 2024-05-24 11:13:19.177918 gigachain_experimental-0.0.59/langchain_experimental/graph_transformers/diffbot.py
+-rw-r--r--   0        0        0    26322 2024-05-24 11:13:19.179496 gigachain_experimental-0.0.59/langchain_experimental/graph_transformers/llm.py
+-rw-r--r--   0        0        0       94 2024-04-19 07:38:33.814674 gigachain_experimental-0.0.59/langchain_experimental/llm_bash/__init__.py
+-rw-r--r--   0        0        0     4459 2024-04-19 07:38:33.815315 gigachain_experimental-0.0.59/langchain_experimental/llm_bash/base.py
+-rw-r--r--   0        0        0     5708 2024-03-28 12:44:20.431110 gigachain_experimental-0.0.59/langchain_experimental/llm_bash/bash.py
+-rw-r--r--   0        0        0     2043 2024-05-06 14:45:38.347288 gigachain_experimental-0.0.59/langchain_experimental/llm_bash/prompt.py
+-rw-r--r--   0        0        0      164 2024-04-19 07:38:33.815701 gigachain_experimental-0.0.59/langchain_experimental/llm_symbolic_math/__init__.py
+-rw-r--r--   0        0        0     5801 2024-05-06 14:45:38.348165 gigachain_experimental-0.0.59/langchain_experimental/llm_symbolic_math/base.py
+-rw-r--r--   0        0        0     1092 2024-05-06 14:45:38.348833 gigachain_experimental-0.0.59/langchain_experimental/llm_symbolic_math/prompt.py
+-rw-r--r--   0        0        0      453 2024-04-19 07:38:33.816657 gigachain_experimental-0.0.59/langchain_experimental/llms/__init__.py
+-rw-r--r--   0        0        0     8763 2024-05-24 11:13:19.180609 gigachain_experimental-0.0.59/langchain_experimental/llms/anthropic_functions.py
+-rw-r--r--   0        0        0     2233 2024-04-19 07:38:33.818900 gigachain_experimental-0.0.59/langchain_experimental/llms/jsonformer_decoder.py
+-rw-r--r--   0        0        0     4349 2024-04-19 07:38:33.820071 gigachain_experimental-0.0.59/langchain_experimental/llms/llamaapi.py
+-rw-r--r--   0        0        0     2848 2024-04-19 07:38:33.820539 gigachain_experimental-0.0.59/langchain_experimental/llms/lmformatenforcer_decoder.py
+-rw-r--r--   0        0        0    14354 2024-05-06 14:45:38.350675 gigachain_experimental-0.0.59/langchain_experimental/llms/ollama_functions.py
+-rw-r--r--   0        0        0     2347 2024-04-19 07:38:33.821338 gigachain_experimental-0.0.59/langchain_experimental/llms/rellm_decoder.py
+-rw-r--r--   0        0        0      346 2024-04-19 07:38:33.821711 gigachain_experimental-0.0.59/langchain_experimental/open_clip/__init__.py
+-rw-r--r--   0        0        0     3383 2024-03-28 12:44:20.442806 gigachain_experimental-0.0.59/langchain_experimental/open_clip/open_clip.py
+-rw-r--r--   0        0        0      120 2023-11-10 13:07:49.953805 gigachain_experimental-0.0.59/langchain_experimental/openai_assistant/__init__.py
+-rw-r--r--   0        0        0      185 2023-11-15 10:30:09.322265 gigachain_experimental-0.0.59/langchain_experimental/openai_assistant/base.py
+-rw-r--r--   0        0        0      330 2024-04-19 07:38:33.822200 gigachain_experimental-0.0.59/langchain_experimental/pal_chain/__init__.py
+-rw-r--r--   0        0        0    13325 2024-04-19 07:38:33.822709 gigachain_experimental-0.0.59/langchain_experimental/pal_chain/base.py
+-rw-r--r--   0        0        0     3542 2024-05-06 14:45:38.353511 gigachain_experimental-0.0.59/langchain_experimental/pal_chain/colored_object_prompt.py
+-rw-r--r--   0        0        0     5772 2024-05-06 14:45:38.355134 gigachain_experimental-0.0.59/langchain_experimental/pal_chain/math_prompt.py
+-rw-r--r--   0        0        0      488 2024-04-19 07:38:33.823092 gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/__init__.py
+-rw-r--r--   0        0        0     3575 2024-04-19 07:38:33.823608 gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/agent_executor.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.508275 gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/executors/__init__.py
+-rw-r--r--   0        0        0     1463 2024-01-18 15:16:40.555727 gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/executors/agent_executor.py
+-rw-r--r--   0        0        0     1274 2024-04-19 07:38:33.824068 gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/executors/base.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.509270 gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/planners/__init__.py
+-rw-r--r--   0        0        0     1572 2024-04-19 07:38:33.824672 gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/planners/base.py
+-rw-r--r--   0        0        0     2319 2024-05-06 14:45:38.356213 gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/planners/chat_planner.py
+-rw-r--r--   0        0        0     1439 2024-03-28 12:44:20.445521 gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/schema.py
+-rw-r--r--   0        0        0      369 2024-04-19 07:38:33.825351 gigachain_experimental-0.0.59/langchain_experimental/prompt_injection_identifier/__init__.py
+-rw-r--r--   0        0        0     3381 2024-05-06 14:45:38.356762 gigachain_experimental-0.0.59/langchain_experimental/prompt_injection_identifier/hugging_face_identifier.py
+-rw-r--r--   0        0        0      174 2024-04-19 07:38:33.826287 gigachain_experimental-0.0.59/langchain_experimental/prompts/__init__.py
+-rw-r--r--   0        0        0       82 2024-05-06 14:45:38.357304 gigachain_experimental-0.0.59/langchain_experimental/prompts/load.py
+-rw-r--r--   0        0        0        0 2023-08-22 08:04:55.368181 gigachain_experimental-0.0.59/langchain_experimental/py.typed
+-rw-r--r--   0        0        0     1285 2023-08-24 07:36:02.836411 gigachain_experimental-0.0.59/langchain_experimental/pydantic_v1/__init__.py
+-rw-r--r--   0        0        0      548 2023-08-24 07:36:02.836900 gigachain_experimental-0.0.59/langchain_experimental/pydantic_v1/dataclasses.py
+-rw-r--r--   0        0        0      520 2023-08-24 07:36:02.837404 gigachain_experimental-0.0.59/langchain_experimental/pydantic_v1/main.py
+-rw-r--r--   0        0        0      518 2024-04-19 07:38:33.827066 gigachain_experimental-0.0.59/langchain_experimental/recommenders/__init__.py
+-rw-r--r--   0        0        0     7967 2024-04-19 07:38:33.827709 gigachain_experimental-0.0.59/langchain_experimental/recommenders/amazon_personalize.py
+-rw-r--r--   0        0        0     6974 2024-05-06 14:45:38.359152 gigachain_experimental-0.0.59/langchain_experimental/recommenders/amazon_personalize_chain.py
+-rw-r--r--   0        0        0      200 2024-04-19 07:38:33.829182 gigachain_experimental-0.0.59/langchain_experimental/retrievers/__init__.py
+-rw-r--r--   0        0        0     1253 2024-04-19 07:38:33.829861 gigachain_experimental-0.0.59/langchain_experimental/retrievers/vector_sql_database.py
+-rw-r--r--   0        0        0     1447 2024-04-19 07:38:33.830696 gigachain_experimental-0.0.59/langchain_experimental/rl_chain/__init__.py
+-rw-r--r--   0        0        0    23251 2024-05-06 14:45:38.359748 gigachain_experimental-0.0.59/langchain_experimental/rl_chain/base.py
+-rw-r--r--   0        0        0     1989 2024-03-28 12:44:20.456634 gigachain_experimental-0.0.59/langchain_experimental/rl_chain/metrics.py
+-rw-r--r--   0        0        0     2126 2024-03-28 12:44:20.457637 gigachain_experimental-0.0.59/langchain_experimental/rl_chain/model_repository.py
+-rw-r--r--   0        0        0    16289 2024-05-06 14:45:38.360601 gigachain_experimental-0.0.59/langchain_experimental/rl_chain/pick_best_chain.py
+-rw-r--r--   0        0        0      556 2024-03-28 12:44:20.459800 gigachain_experimental-0.0.59/langchain_experimental/rl_chain/vw_logger.py
+-rw-r--r--   0        0        0      946 2024-04-19 07:38:33.832517 gigachain_experimental-0.0.59/langchain_experimental/smart_llm/__init__.py
+-rw-r--r--   0        0        0    14438 2024-05-06 14:45:38.362010 gigachain_experimental-0.0.59/langchain_experimental/smart_llm/base.py
+-rw-r--r--   0        0        0      202 2024-04-19 07:38:33.834385 gigachain_experimental-0.0.59/langchain_experimental/sql/__init__.py
+-rw-r--r--   0        0        0    13257 2024-05-06 14:45:38.362879 gigachain_experimental-0.0.59/langchain_experimental/sql/base.py
+-rw-r--r--   0        0        0     4663 2024-05-06 14:45:38.363512 gigachain_experimental-0.0.59/langchain_experimental/sql/prompt.py
+-rw-r--r--   0        0        0     9856 2024-05-06 14:45:38.364173 gigachain_experimental-0.0.59/langchain_experimental/sql/vector_sql.py
+-rw-r--r--   0        0        0     1576 2024-04-19 07:38:33.836627 gigachain_experimental-0.0.59/langchain_experimental/synthetic_data/__init__.py
+-rw-r--r--   0        0        0      464 2024-05-06 14:45:38.364970 gigachain_experimental-0.0.59/langchain_experimental/synthetic_data/prompts.py
+-rw-r--r--   0        0        0       75 2024-04-19 07:38:33.837144 gigachain_experimental-0.0.59/langchain_experimental/tabular_synthetic_data/__init__.py
+-rw-r--r--   0        0        0     5346 2024-05-06 14:45:38.365645 gigachain_experimental-0.0.59/langchain_experimental/tabular_synthetic_data/base.py
+-rw-r--r--   0        0        0     2523 2024-04-19 07:38:33.837650 gigachain_experimental-0.0.59/langchain_experimental/tabular_synthetic_data/openai.py
+-rw-r--r--   0        0        0      417 2024-05-06 14:45:38.366178 gigachain_experimental-0.0.59/langchain_experimental/tabular_synthetic_data/prompts.py
+-rw-r--r--   0        0        0     9850 2024-05-06 14:45:38.366807 gigachain_experimental-0.0.59/langchain_experimental/text_splitter.py
+-rw-r--r--   0        0        0      180 2024-04-19 07:38:33.839237 gigachain_experimental-0.0.59/langchain_experimental/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-19 12:57:52.604149 gigachain_experimental-0.0.59/langchain_experimental/tools/python/__init__.py
+-rw-r--r--   0        0        0     4768 2024-04-19 07:38:33.840630 gigachain_experimental-0.0.59/langchain_experimental/tools/python/tool.py
+-rw-r--r--   0        0        0      425 2024-04-19 07:38:33.841264 gigachain_experimental-0.0.59/langchain_experimental/tot/__init__.py
+-rw-r--r--   0        0        0     4858 2024-04-19 07:38:33.842457 gigachain_experimental-0.0.59/langchain_experimental/tot/base.py
+-rw-r--r--   0        0        0     1410 2024-04-19 07:38:33.843054 gigachain_experimental-0.0.59/langchain_experimental/tot/checker.py
+-rw-r--r--   0        0        0     1666 2023-08-21 13:51:28.515184 gigachain_experimental-0.0.59/langchain_experimental/tot/controller.py
+-rw-r--r--   0        0        0     1467 2024-03-28 12:44:20.474461 gigachain_experimental-0.0.59/langchain_experimental/tot/memory.py
+-rw-r--r--   0        0        0     4797 2024-04-19 07:38:33.843690 gigachain_experimental-0.0.59/langchain_experimental/tot/prompts.py
+-rw-r--r--   0        0        0      504 2024-03-28 12:44:20.475874 gigachain_experimental-0.0.59/langchain_experimental/tot/thought.py
+-rw-r--r--   0        0        0     3123 2024-05-06 14:45:38.367342 gigachain_experimental-0.0.59/langchain_experimental/tot/thought_generation.py
+-rw-r--r--   0        0        0      148 2024-04-19 07:38:33.844253 gigachain_experimental-0.0.59/langchain_experimental/utilities/__init__.py
+-rw-r--r--   0        0        0     2690 2024-05-06 14:45:38.367934 gigachain_experimental-0.0.59/langchain_experimental/utilities/python.py
+-rw-r--r--   0        0        0      114 2024-04-19 07:38:33.844644 gigachain_experimental-0.0.59/langchain_experimental/video_captioning/__init__.py
+-rw-r--r--   0        0        0     5034 2024-04-19 07:38:33.845065 gigachain_experimental-0.0.59/langchain_experimental/video_captioning/base.py
+-rw-r--r--   0        0        0     4880 2024-04-19 07:38:33.845525 gigachain_experimental-0.0.59/langchain_experimental/video_captioning/models.py
+-rw-r--r--   0        0        0     4369 2024-04-19 07:38:33.845977 gigachain_experimental-0.0.59/langchain_experimental/video_captioning/prompts.py
+-rw-r--r--   0        0        0     3196 2024-04-19 07:38:33.846553 gigachain_experimental-0.0.59/langchain_experimental/video_captioning/services/audio_service.py
+-rw-r--r--   0        0        0    11301 2024-04-19 07:38:33.847251 gigachain_experimental-0.0.59/langchain_experimental/video_captioning/services/caption_service.py
+-rw-r--r--   0        0        0     4932 2024-04-19 07:38:33.848536 gigachain_experimental-0.0.59/langchain_experimental/video_captioning/services/combine_service.py
+-rw-r--r--   0        0        0     3773 2024-04-19 07:38:33.848986 gigachain_experimental-0.0.59/langchain_experimental/video_captioning/services/image_service.py
+-rw-r--r--   0        0        0      459 2024-04-19 07:38:33.849333 gigachain_experimental-0.0.59/langchain_experimental/video_captioning/services/srt_service.py
+-rw-r--r--   0        0        0     4065 2024-05-24 11:13:58.827756 gigachain_experimental-0.0.59/pyproject.toml
+-rw-r--r--   0        0        0     2076 1970-01-01 00:00:00.000000 gigachain_experimental-0.0.59/PKG-INFO
```

### Comparing `gigachain_experimental-0.0.57/LICENSE` & `gigachain_experimental-0.0.59/LICENSE`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/README.md` & `gigachain_experimental-0.0.59/README.md`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/agents/__init__.py` & `gigachain_experimental-0.0.59/langchain_experimental/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/__init__.py` & `gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/csv/base.py` & `gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/csv/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/pandas/base.py` & `gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/pandas/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 """Agent for working with pandas objects."""
 import warnings
-from typing import Any, Dict, List, Literal, Optional, Sequence, Union
+from typing import Any, Dict, List, Literal, Optional, Sequence, Union, cast
 
-from langchain.agents import AgentType, create_openai_tools_agent, create_react_agent
+from langchain.agents import (
+    AgentType,
+    create_openai_tools_agent,
+    create_react_agent,
+    create_tool_calling_agent,
+)
 from langchain.agents.agent import (
     AgentExecutor,
     BaseMultiActionAgent,
     BaseSingleActionAgent,
     RunnableAgent,
     RunnableMultiActionAgent,
 )
 from langchain.agents.mrkl.prompt import FORMAT_INSTRUCTIONS
 from langchain.agents.openai_functions_agent.base import (
     OpenAIFunctionsAgent,
     create_openai_functions_agent,
 )
 from langchain_core.callbacks import BaseCallbackManager
-from langchain_core.language_models import LanguageModelLike
+from langchain_core.language_models import BaseLanguageModel, LanguageModelLike
 from langchain_core.messages import SystemMessage
 from langchain_core.prompts import (
     BasePromptTemplate,
     ChatPromptTemplate,
     PromptTemplate,
 )
 from langchain_core.tools import BaseTool
@@ -143,15 +148,15 @@
     )
 
 
 def create_pandas_dataframe_agent(
     llm: LanguageModelLike,
     df: Any,
     agent_type: Union[
-        AgentType, Literal["openai-tools"]
+        AgentType, Literal["openai-tools", "tool-calling"]
     ] = AgentType.ZERO_SHOT_REACT_DESCRIPTION,
     callback_manager: Optional[BaseCallbackManager] = None,
     prefix: Optional[str] = None,
     suffix: Optional[str] = None,
     input_variables: Optional[List[str]] = None,
     verbose: bool = False,
     return_intermediate_steps: bool = False,
@@ -164,19 +169,21 @@
     extra_tools: Sequence[BaseTool] = (),
     engine: Literal["pandas", "modin"] = "pandas",
     **kwargs: Any,
 ) -> AgentExecutor:
     """Construct a Pandas agent from an LLM and dataframe(s).
 
     Args:
-        llm: Language model to use for the agent.
+        llm: Language model to use for the agent. If agent_type is "tool-calling" then
+            llm is expected to support tool calling.
         df: Pandas dataframe or list of Pandas dataframes.
-        agent_type: One of "openai-tools", "openai-functions", or
+        agent_type: One of "tool-calling", "openai-tools", "openai-functions", or
             "zero-shot-react-description". Defaults to "zero-shot-react-description".
-            "openai-tools" is recommended over "openai-functions".
+            "tool-calling" is recommended over the legacy "openai-tools" and
+            "openai-functions" types.
         callback_manager: DEPRECATED. Pass "callbacks" key into 'agent_executor_kwargs'
             instead to pass constructor callbacks to AgentExecutor.
         prefix: Prompt prefix string.
         suffix: Prompt suffix string.
         input_variables: DEPRECATED. Input variables automatically inferred from
             constructed prompt.
         verbose: AgentExecutor verbosity.
@@ -205,15 +212,15 @@
             import pandas as pd
 
             df = pd.read_csv("titanic.csv")
             llm = ChatOpenAI(model="gpt-3.5-turbo", temperature=0)
             agent_executor = create_pandas_dataframe_agent(
                 llm,
                 df,
-                agent_type="openai-tools",
+                agent_type="tool-calling",
                 verbose=True
             )
 
     """  # noqa: E501
     try:
         if engine == "modin":
             import modin.pandas as pd
@@ -264,38 +271,50 @@
             number_of_head_rows=number_of_head_rows,
         )
         agent: Union[BaseSingleActionAgent, BaseMultiActionAgent] = RunnableAgent(
             runnable=create_react_agent(llm, tools, prompt),  # type: ignore
             input_keys_arg=["input"],
             return_keys_arg=["output"],
         )
-    elif agent_type in (AgentType.OPENAI_FUNCTIONS, "openai-tools"):
+    elif agent_type in (AgentType.OPENAI_FUNCTIONS, "openai-tools", "tool-calling"):
         prompt = _get_functions_prompt(
             df,
             prefix=prefix,
             suffix=suffix,
             include_df_in_prompt=include_df_in_prompt,
             number_of_head_rows=number_of_head_rows,
         )
         if agent_type == AgentType.OPENAI_FUNCTIONS:
+            runnable = create_openai_functions_agent(
+                cast(BaseLanguageModel, llm), tools, prompt
+            )
             agent = RunnableAgent(
-                runnable=create_openai_functions_agent(llm, tools, prompt),  # type: ignore
+                runnable=runnable,
                 input_keys_arg=["input"],
                 return_keys_arg=["output"],
             )
         else:
+            if agent_type == "openai-tools":
+                runnable = create_openai_tools_agent(
+                    cast(BaseLanguageModel, llm), tools, prompt
+                )
+            else:
+                runnable = create_tool_calling_agent(
+                    cast(BaseLanguageModel, llm), tools, prompt
+                )
             agent = RunnableMultiActionAgent(
-                runnable=create_openai_tools_agent(llm, tools, prompt),  # type: ignore
+                runnable=runnable,
                 input_keys_arg=["input"],
                 return_keys_arg=["output"],
             )
     else:
         raise ValueError(
             f"Agent type {agent_type} not supported at the moment. Must be one of "
-            "'openai-tools', 'openai-functions', or 'zero-shot-react-description'."
+            "'tool-calling', 'openai-tools', 'openai-functions', or "
+            "'zero-shot-react-description'."
         )
     return AgentExecutor(
         agent=agent,
         tools=tools,
         callback_manager=callback_manager,
         verbose=verbose,
         return_intermediate_steps=return_intermediate_steps,
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/pandas/prompt.py` & `gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/pandas/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/python/base.py` & `gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/python/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from typing import Any, Dict, Optional
 
 from langchain.agents.agent import AgentExecutor, BaseSingleActionAgent
 from langchain.agents.mrkl.base import ZeroShotAgent
 from langchain.agents.openai_functions_agent.base import OpenAIFunctionsAgent
 from langchain.agents.types import AgentType
-from langchain.callbacks.base import BaseCallbackManager
 from langchain.chains.llm import LLMChain
+from langchain_core.callbacks.base import BaseCallbackManager
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.messages import SystemMessage
 
 from langchain_experimental.agents.agent_toolkits.python.prompt import PREFIX
 from langchain_experimental.tools.python.tool import PythonREPLTool
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/python/prompt.py` & `gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/python/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/spark/base.py` & `gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/spark/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Agent for working with pandas objects."""
 from typing import Any, Dict, List, Optional
 
 from langchain.agents.agent import AgentExecutor
 from langchain.agents.mrkl.base import ZeroShotAgent
-from langchain.callbacks.base import BaseCallbackManager
 from langchain.chains.llm import LLMChain
+from langchain_core.callbacks.base import BaseCallbackManager
 from langchain_core.language_models import BaseLLM
 
 from langchain_experimental.agents.agent_toolkits.spark.prompt import PREFIX, SUFFIX
 from langchain_experimental.tools.python.tool import PythonAstREPLTool
 
 
 def _validate_spark_df(df: Any) -> bool:
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/xorbits/base.py` & `gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/xorbits/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Agent for working with xorbits objects."""
 from typing import Any, Dict, List, Optional
 
 from langchain.agents.agent import AgentExecutor
 from langchain.agents.mrkl.base import ZeroShotAgent
-from langchain.callbacks.base import BaseCallbackManager
 from langchain.chains.llm import LLMChain
+from langchain_core.callbacks.base import BaseCallbackManager
 from langchain_core.language_models import BaseLLM
 
 from langchain_experimental.agents.agent_toolkits.xorbits.prompt import (
     NP_PREFIX,
     NP_SUFFIX,
     PD_PREFIX,
     PD_SUFFIX,
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/agents/agent_toolkits/xorbits/prompt.py` & `gigachain_experimental-0.0.59/langchain_experimental/agents/agent_toolkits/xorbits/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/__init__.py` & `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/autogpt/agent.py` & `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/autogpt/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
                     f"и отвечай только в требуемом JSON формате."
                 )
 
             memory_to_add = (
                 f"Ответ ассистента: {assistant_reply} " f"\nResult: {result} "
             )
             if self.feedback_tool is not None:
-                feedback = f"\n{self.feedback_tool.run('Input: ')}"
+                feedback = f"{self.feedback_tool.run('Input: ')}"
                 if feedback in {"q", "stop"}:
                     print("EXITING")  # noqa: T201
                     return "EXITING"
-                memory_to_add += feedback
+                memory_to_add += f"\n{feedback}"
 
             self.memory.add_documents([Document(page_content=memory_to_add)])
             self.chat_history_memory.add_message(HumanMessage(content=result))
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/autogpt/memory.py` & `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/autogpt/memory.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,12 +22,12 @@
         if self.input_key is None:
             return get_prompt_input_key(inputs, self.memory_variables)
         return self.input_key
 
     def load_memory_variables(self, inputs: Dict[str, Any]) -> Dict[str, Any]:
         input_key = self._get_prompt_input_key(inputs)
         query = inputs[input_key]
-        docs = self.retriever.get_relevant_documents(query)
+        docs = self.retriever.invoke(query)
         return {
             "chat_history": self.chat_memory.messages[-10:],
             "relevant_context": docs,
         }
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/autogpt/output_parser.py` & `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/autogpt/output_parser.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/autogpt/prompt.py` & `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/autogpt/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import time
 from typing import Any, Callable, List, cast
 
-from langchain.prompts.chat import (
-    BaseChatPromptTemplate,
-)
 from langchain.tools.base import BaseTool
 from langchain_core.messages import BaseMessage, HumanMessage, SystemMessage
+from langchain_core.prompts.chat import (
+    BaseChatPromptTemplate,
+)
 from langchain_core.vectorstores import VectorStoreRetriever
 
 from langchain_experimental.autonomous_agents.autogpt.prompt_generator import get_prompt
 from langchain_experimental.pydantic_v1 import BaseModel
 
 
 # This class has a metaclass conflict: both `BaseChatPromptTemplate` and `BaseModel`
@@ -67,15 +67,15 @@
             content=f"Текущее время и дата {time.strftime('%c')}"
         )
         used_tokens = self.token_counter(
             cast(str, base_prompt.content)
         ) + self.token_counter(cast(str, time_prompt.content))
         memory: VectorStoreRetriever = kwargs["memory"]
         previous_messages = kwargs["messages"]
-        relevant_docs = memory.get_relevant_documents(str(previous_messages[-10:]))
+        relevant_docs = memory.invoke(str(previous_messages[-10:]))
         relevant_memory = [d.page_content for d in relevant_docs]
         relevant_memory_tokens = sum(
             [self.token_counter(doc) for doc in relevant_memory]
         )
         while used_tokens + relevant_memory_tokens > 2500:
             relevant_memory = relevant_memory[:-1]
             relevant_memory_tokens = sum(
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py` & `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/baby_agi/__init__.py` & `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/baby_agi/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py` & `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """BabyAGI agent."""
 
 from collections import deque
 from typing import Any, Dict, List, Optional
 
-from langchain.callbacks.manager import CallbackManagerForChainRun
 from langchain.chains.base import Chain
+from langchain_core.callbacks.manager import CallbackManagerForChainRun
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.vectorstores import VectorStore
 
 from langchain_experimental.autonomous_agents.baby_agi.task_creation import (
     TaskCreationChain,
 )
 from langchain_experimental.autonomous_agents.baby_agi.task_execution import (
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/baby_agi/task_creation.py` & `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/baby_agi/task_creation.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/baby_agi/task_execution.py` & `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/baby_agi/task_execution.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py` & `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py` & `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py` & `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, List, Optional
 
 from langchain.base_language import BaseLanguageModel
-from langchain.callbacks.manager import Callbacks
 from langchain.chains import LLMChain
+from langchain_core.callbacks.manager import Callbacks
 from langchain_core.prompts import PromptTemplate
 
 
 class ResponseGenerationChain(LLMChain):
     """Chain to execute tasks."""
 
     @classmethod
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py` & `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,16 @@
             if self.task in ["video_generator", "image_generator", "text_reader"]:
                 self.product = self.tool(**new_args)
             else:
                 self.result = self.tool(**new_args)
         except Exception as e:
             self.status = "failed"
             self.message = str(e)
+            return self.message
+
         self.status = "completed"
         self.save_product()
 
         return self.result
 
 
 class TaskExecutor:
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py` & `gigachain_experimental-0.0.59/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import json
 import re
 from abc import abstractmethod
 from typing import Any, Dict, List, Optional, Union
 
 from langchain.base_language import BaseLanguageModel
-from langchain.callbacks.manager import Callbacks
 from langchain.chains import LLMChain
-from langchain.prompts.chat import (
+from langchain.tools.base import BaseTool
+from langchain_core.callbacks.manager import Callbacks
+from langchain_core.prompts.chat import (
     AIMessagePromptTemplate,
     ChatPromptTemplate,
     HumanMessagePromptTemplate,
     SystemMessagePromptTemplate,
 )
-from langchain.tools.base import BaseTool
 
 from langchain_experimental.pydantic_v1 import BaseModel
 
 DEMONSTRATIONS = [
     {
         "role": "user",
         "content": "покажи мне видео и изображение на основе текста 'мальчик бежит' и озвучь это",  # noqa: E501
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/chat_models/__init__.py` & `gigachain_experimental-0.0.59/langchain_experimental/chat_models/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/chat_models/llm_wrapper.py` & `gigachain_experimental-0.0.59/langchain_experimental/chat_models/llm_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Generic Wrapper for chat LLMs, with sample implementations
 for Llama-2-chat, Llama-2-instruct and Vicuna models.
 """
 from typing import Any, List, Optional, cast
 
-from langchain.callbacks.manager import (
-    AsyncCallbackManagerForLLMRun,
-    CallbackManagerForLLMRun,
-)
 from langchain.schema import (
     AIMessage,
     BaseMessage,
     ChatGeneration,
     ChatResult,
     HumanMessage,
     LLMResult,
     SystemMessage,
 )
+from langchain_core.callbacks.manager import (
+    AsyncCallbackManagerForLLMRun,
+    CallbackManagerForLLMRun,
+)
 from langchain_core.language_models import LLM, BaseChatModel
 
 DEFAULT_SYSTEM_PROMPT = """You are a helpful, respectful and honest assistant. Always answer as helpfully as possible, while being safe. Your answers should not include any harmful, unethical, racist, sexist, toxic, dangerous, or illegal content. Please ensure that your responses are socially unbiased and positive in nature.
 
 If a question does not make any sense, or is not factually coherent, explain why instead of answering something not correct. If you don't know the answer to a question, please don't share false information."""  # noqa: E501
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/comprehend_moderation/__init__.py` & `gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/comprehend_moderation/amazon_comprehend_moderation.py` & `gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/amazon_comprehend_moderation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Dict, List, Optional
 
-from langchain.callbacks.manager import CallbackManagerForChainRun
 from langchain.chains.base import Chain
+from langchain_core.callbacks.manager import CallbackManagerForChainRun
 
 from langchain_experimental.comprehend_moderation.base_moderation import (
     BaseModeration,
 )
 from langchain_experimental.comprehend_moderation.base_moderation_callbacks import (
     BaseModerationCallbackHandler,
 )
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/comprehend_moderation/base_moderation.py` & `gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/base_moderation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import uuid
 from typing import Any, Callable, Optional, cast
 
-from langchain.callbacks.manager import CallbackManagerForChainRun
+from langchain_core.callbacks.manager import CallbackManagerForChainRun
 from langchain_core.messages import AIMessage, HumanMessage
 from langchain_core.prompt_values import ChatPromptValue, StringPromptValue
 
 from langchain_experimental.comprehend_moderation.pii import ComprehendPII
 from langchain_experimental.comprehend_moderation.prompt_safety import (
     ComprehendPromptSafety,
 )
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/comprehend_moderation/base_moderation_callbacks.py` & `gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/base_moderation_callbacks.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/comprehend_moderation/base_moderation_config.py` & `gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/base_moderation_config.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/comprehend_moderation/base_moderation_exceptions.py` & `gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/base_moderation_exceptions.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/comprehend_moderation/pii.py` & `gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/pii.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/comprehend_moderation/prompt_safety.py` & `gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/prompt_safety.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/comprehend_moderation/toxicity.py` & `gigachain_experimental-0.0.59/langchain_experimental/comprehend_moderation/toxicity.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/cpal/__init__.py` & `gigachain_experimental-0.0.59/langchain_experimental/cpal/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/cpal/base.py` & `gigachain_experimental-0.0.59/langchain_experimental/cpal/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 """
 from __future__ import annotations
 
 import json
 from typing import Any, ClassVar, Dict, List, Optional, Type
 
 from langchain.base_language import BaseLanguageModel
-from langchain.callbacks.manager import CallbackManagerForChainRun
 from langchain.chains.base import Chain
 from langchain.chains.llm import LLMChain
 from langchain.output_parsers import PydanticOutputParser
-from langchain.prompts.prompt import PromptTemplate
+from langchain_core.callbacks.manager import CallbackManagerForChainRun
+from langchain_core.prompts.prompt import PromptTemplate
 
 from langchain_experimental import pydantic_v1 as pydantic
 from langchain_experimental.cpal.constants import Constant
 from langchain_experimental.cpal.models import (
     CausalModel,
     InterventionModel,
     NarrativeModel,
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/cpal/models.py` & `gigachain_experimental-0.0.59/langchain_experimental/cpal/models.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/cpal/templates/univariate/causal.py` & `gigachain_experimental-0.0.59/langchain_experimental/cpal/templates/univariate/causal.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/cpal/templates/univariate/intervention.py` & `gigachain_experimental-0.0.59/langchain_experimental/cpal/templates/univariate/intervention.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/cpal/templates/univariate/narrative.py` & `gigachain_experimental-0.0.59/langchain_experimental/cpal/templates/univariate/narrative.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/cpal/templates/univariate/query.py` & `gigachain_experimental-0.0.59/langchain_experimental/cpal/templates/univariate/query.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/data_anonymizer/__init__.py` & `gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/data_anonymizer/base.py` & `gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/data_anonymizer/deanonymizer_mapping.py` & `gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/deanonymizer_mapping.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/data_anonymizer/deanonymizer_matching_strategies.py` & `gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/deanonymizer_matching_strategies.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/data_anonymizer/faker_presidio_mapping.py` & `gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/faker_presidio_mapping.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/data_anonymizer/presidio.py` & `gigachain_experimental-0.0.59/langchain_experimental/data_anonymizer/presidio.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/generative_agents/generative_agent.py` & `gigachain_experimental-0.0.59/langchain_experimental/generative_agents/generative_agent.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/generative_agents/memory.py` & `gigachain_experimental-0.0.59/langchain_experimental/generative_agents/memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,17 +221,17 @@
 
     def fetch_memories(
         self, observation: str, now: Optional[datetime] = None
     ) -> List[Document]:
         """Fetch related memories."""
         if now is not None:
             with mock_now(now):
-                return self.memory_retriever.get_relevant_documents(observation)
+                return self.memory_retriever.invoke(observation)
         else:
-            return self.memory_retriever.get_relevant_documents(observation)
+            return self.memory_retriever.invoke(observation)
 
     def format_memories_detail(self, relevant_memories: List[Document]) -> str:
         content = []
         for mem in relevant_memories:
             content.append(self._format_memory_detail(mem, prefix="- "))
         return "\n".join([f"{mem}" for mem in content])
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/graph_transformers/diffbot.py` & `gigachain_experimental-0.0.59/langchain_experimental/graph_transformers/diffbot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,22 @@
+from enum import Enum
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 import requests
 from langchain.utils import get_from_env
 from langchain_community.graphs.graph_document import GraphDocument, Node, Relationship
 from langchain_core.documents import Document
 
 
+class TypeOption(str, Enum):
+    FACTS = "facts"
+    ENTITIES = "entities"
+    SENTIMENT = "sentiment"
+
+
 def format_property_key(s: str) -> str:
     """Formats a string to be used as a property key."""
 
     words = s.split()
     if not words:
         return s
     first_word = words[0].lower()
@@ -137,14 +144,17 @@
     def __init__(
         self,
         diffbot_api_key: Optional[str] = None,
         fact_confidence_threshold: float = 0.7,
         include_qualifiers: bool = True,
         include_evidence: bool = True,
         simplified_schema: bool = True,
+        extract_types: List[TypeOption] = [TypeOption.FACTS],
+        *,
+        include_confidence: bool = False,
     ) -> None:
         """
         Initialize the graph transformer with various options.
 
         Args:
             diffbot_api_key (str):
                The API key for Diffbot's NLP services.
@@ -153,24 +163,39 @@
                 Minimum confidence level for facts to be included.
             include_qualifiers (bool):
                 Whether to include qualifiers in the relationships.
             include_evidence (bool):
                 Whether to include evidence for the relationships.
             simplified_schema (bool):
                 Whether to use a simplified schema for relationships.
+            extract_types (List[TypeOption]):
+                A list of data types to extract. Facts, entities, and
+                sentiment are supported. By default, the option is
+                set to facts. A fact represents a combination of
+                source and target nodes with a relationship type.
+            include_confidence (bool):
+                Whether to include confidence scores on nodes and rels
         """
         self.diffbot_api_key = diffbot_api_key or get_from_env(
             "diffbot_api_key", "DIFFBOT_API_KEY"
         )
         self.fact_threshold_confidence = fact_confidence_threshold
         self.include_qualifiers = include_qualifiers
         self.include_evidence = include_evidence
+        self.include_confidence = include_confidence
         self.simplified_schema = None
         if simplified_schema:
             self.simplified_schema = SimplifiedSchema()
+        if not extract_types:
+            raise ValueError(
+                "`extract_types` cannot be an empty array. "
+                "Allowed values are 'facts', 'entities', or both."
+            )
+
+        self.extract_types = extract_types
 
     def nlp_request(self, text: str) -> Dict[str, Any]:
         """
         Make an API request to the Diffbot NLP endpoint.
 
         Args:
             text (str): The text to be processed.
@@ -181,15 +206,15 @@
 
         # Relationship extraction only works for English
         payload = {
             "content": text,
             "lang": "en",
         }
 
-        FIELDS = "facts"
+        FIELDS = ",".join(self.extract_types)
         HOST = "nl.diffbot.com"
         url = (
             f"https://{HOST}/v1/?fields={FIELDS}&"
             f"token={self.diffbot_api_key}&language=en"
         )
         result = requests.post(url, data=payload)
         return result.json()
@@ -205,85 +230,118 @@
             document (Document): The original document.
 
         Returns:
             GraphDocument: The transformed document as a graph.
         """
 
         # Return empty result if there are no facts
-        if "facts" not in payload or not payload["facts"]:
+        if ("facts" not in payload or not payload["facts"]) and (
+            "entities" not in payload or not payload["entities"]
+        ):
             return GraphDocument(nodes=[], relationships=[], source=document)
 
         # Nodes are a custom class because we need to deduplicate
         nodes_list = NodesList()
-        # Relationships are a list because we don't deduplicate nor anything else
-        relationships = list()
-        for record in payload["facts"]:
-            # Skip if the fact is below the threshold confidence
-            if record["confidence"] < self.fact_threshold_confidence:
-                continue
-
-            # TODO: It should probably be treated as a node property
-            if not record["value"]["allTypes"]:
-                continue
-
-            # Define source node
-            source_id = (
-                record["entity"]["allUris"][0]
-                if record["entity"]["allUris"]
-                else record["entity"]["name"]
-            )
-            source_label = record["entity"]["allTypes"][0]["name"].capitalize()
-            source_name = record["entity"]["name"]
-            source_node = Node(id=source_id, type=source_label)
-            nodes_list.add_node_property(
-                (source_id, source_label), {"name": source_name}
-            )
-
-            # Define target node
-            target_id = (
-                record["value"]["allUris"][0]
-                if record["value"]["allUris"]
-                else record["value"]["name"]
-            )
-            target_label = record["value"]["allTypes"][0]["name"].capitalize()
-            target_name = record["value"]["name"]
-            # Some facts are better suited as node properties
-            if target_label in FACT_TO_PROPERTY_TYPE:
+        if "entities" in payload and payload["entities"]:
+            for record in payload["entities"]:
+                # Ignore if it doesn't have a type
+                if not record["allTypes"]:
+                    continue
+
+                # Define source node
+                source_id = (
+                    record["allUris"][0] if record["allUris"] else record["name"]
+                )
+                source_label = record["allTypes"][0]["name"].capitalize()
+                source_name = record["name"]
                 nodes_list.add_node_property(
-                    (source_id, source_label),
-                    {format_property_key(record["property"]["name"]): target_name},
+                    (source_id, source_label), {"name": source_name}
+                )
+                if record.get("sentiment") is not None:
+                    nodes_list.add_node_property(
+                        (source_id, source_label),
+                        {"sentiment": record.get("sentiment")},
+                    )
+                if self.include_confidence:
+                    nodes_list.add_node_property(
+                        (source_id, source_label),
+                        {"confidence": record.get("confidence")},
+                    )
+
+        relationships = list()
+        # Relationships are a list because we don't deduplicate nor anything else
+        if "facts" in payload and payload["facts"]:
+            for record in payload["facts"]:
+                # Skip if the fact is below the threshold confidence
+                if record["confidence"] < self.fact_threshold_confidence:
+                    continue
+
+                # TODO: It should probably be treated as a node property
+                if not record["value"]["allTypes"]:
+                    continue
+
+                # Define source node
+                source_id = (
+                    record["entity"]["allUris"][0]
+                    if record["entity"]["allUris"]
+                    else record["entity"]["name"]
                 )
-            else:  # Define relationship
-                # Define target node object
-                target_node = Node(id=target_id, type=target_label)
+                source_label = record["entity"]["allTypes"][0]["name"].capitalize()
+                source_name = record["entity"]["name"]
+                source_node = Node(id=source_id, type=source_label)
                 nodes_list.add_node_property(
-                    (target_id, target_label), {"name": target_name}
+                    (source_id, source_label), {"name": source_name}
                 )
-                # Define relationship type
-                rel_type = record["property"]["name"].replace(" ", "_").upper()
-                if self.simplified_schema:
-                    rel_type = self.simplified_schema.get_type(rel_type)
-
-                # Relationship qualifiers/properties
-                rel_properties = dict()
-                relationship_evidence = [el["passage"] for el in record["evidence"]][0]
-                if self.include_evidence:
-                    rel_properties.update({"evidence": relationship_evidence})
-                if self.include_qualifiers and record.get("qualifiers"):
-                    for property in record["qualifiers"]:
-                        prop_key = format_property_key(property["property"]["name"])
-                        rel_properties[prop_key] = property["value"]["name"]
-
-                relationship = Relationship(
-                    source=source_node,
-                    target=target_node,
-                    type=rel_type,
-                    properties=rel_properties,
+
+                # Define target node
+                target_id = (
+                    record["value"]["allUris"][0]
+                    if record["value"]["allUris"]
+                    else record["value"]["name"]
                 )
-                relationships.append(relationship)
+                target_label = record["value"]["allTypes"][0]["name"].capitalize()
+                target_name = record["value"]["name"]
+                # Some facts are better suited as node properties
+                if target_label in FACT_TO_PROPERTY_TYPE:
+                    nodes_list.add_node_property(
+                        (source_id, source_label),
+                        {format_property_key(record["property"]["name"]): target_name},
+                    )
+                else:  # Define relationship
+                    # Define target node object
+                    target_node = Node(id=target_id, type=target_label)
+                    nodes_list.add_node_property(
+                        (target_id, target_label), {"name": target_name}
+                    )
+                    # Define relationship type
+                    rel_type = record["property"]["name"].replace(" ", "_").upper()
+                    if self.simplified_schema:
+                        rel_type = self.simplified_schema.get_type(rel_type)
+
+                    # Relationship qualifiers/properties
+                    rel_properties = dict()
+                    relationship_evidence = [
+                        el["passage"] for el in record["evidence"]
+                    ][0]
+                    if self.include_evidence:
+                        rel_properties.update({"evidence": relationship_evidence})
+                    if self.include_confidence:
+                        rel_properties.update({"confidence": record["confidence"]})
+                    if self.include_qualifiers and record.get("qualifiers"):
+                        for property in record["qualifiers"]:
+                            prop_key = format_property_key(property["property"]["name"])
+                            rel_properties[prop_key] = property["value"]["name"]
+
+                    relationship = Relationship(
+                        source=source_node,
+                        target=target_node,
+                        type=rel_type,
+                        properties=rel_properties,
+                    )
+                    relationships.append(relationship)
 
         return GraphDocument(
             nodes=nodes_list.return_node_list(),
             relationships=relationships,
             source=document,
         )
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/llm_bash/base.py` & `gigachain_experimental-0.0.59/langchain_experimental/llm_bash/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Chain that interprets a prompt and executes bash operations."""
 from __future__ import annotations
 
 import logging
 import warnings
 from typing import Any, Dict, List, Optional
 
-from langchain.callbacks.manager import CallbackManagerForChainRun
 from langchain.chains.base import Chain
 from langchain.chains.llm import LLMChain
 from langchain.schema import BasePromptTemplate, OutputParserException
+from langchain_core.callbacks.manager import CallbackManagerForChainRun
 from langchain_core.language_models import BaseLanguageModel
 
 from langchain_experimental.llm_bash.bash import BashProcess
 from langchain_experimental.llm_bash.prompt import PROMPT
 from langchain_experimental.pydantic_v1 import Extra, Field, root_validator
 
 logger = logging.getLogger(__name__)
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/llm_bash/bash.py` & `gigachain_experimental-0.0.59/langchain_experimental/llm_bash/bash.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/llm_bash/prompt.py` & `gigachain_experimental-0.0.59/langchain_experimental/llm_bash/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # flake8: noqa
 from __future__ import annotations
 
 import re
 from typing import List
 
-from langchain.prompts.prompt import PromptTemplate
+from langchain_core.prompts.prompt import PromptTemplate
 from langchain_core.output_parsers import BaseOutputParser
 from langchain_core.exceptions import OutputParserException
 
 _PROMPT_TEMPLATE = """If someone asks you to perform a task, your job is to come up with a series of bash commands that will perform the task. There is no need to put "#!/bin/bash" in your answer. Make sure to reason step by step, using this format:
 
 Question: "copy the files in the directory named 'target' into a new directory at the same level as target called 'myNewDirectory'"
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/llm_symbolic_math/base.py` & `gigachain_experimental-0.0.59/langchain_experimental/llm_symbolic_math/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Chain that interprets a prompt and executes python code to do symbolic math."""
 from __future__ import annotations
 
 import re
 from typing import Any, Dict, List, Optional
 
 from langchain.base_language import BaseLanguageModel
-from langchain.callbacks.manager import (
+from langchain.chains.base import Chain
+from langchain.chains.llm import LLMChain
+from langchain_core.callbacks.manager import (
     AsyncCallbackManagerForChainRun,
     CallbackManagerForChainRun,
 )
-from langchain.chains.base import Chain
-from langchain.chains.llm import LLMChain
-from langchain.prompts.base import BasePromptTemplate
+from langchain_core.prompts.base import BasePromptTemplate
 
 from langchain_experimental.llm_symbolic_math.prompt import PROMPT
 from langchain_experimental.pydantic_v1 import Extra
 
 
 class LLMSymbolicMathChain(Chain):
     """Chain that interprets a prompt and executes python code to do symbolic math.
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/llm_symbolic_math/prompt.py` & `gigachain_experimental-0.0.59/langchain_experimental/llm_symbolic_math/prompt.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # flake8: noqa
-from langchain.prompts.prompt import PromptTemplate
+from langchain_core.prompts.prompt import PromptTemplate
 
 _PROMPT_TEMPLATE = """Translate a math problem into a expression that can be executed using Python's SymPy library. Use the output of running this code to answer the question.
 
 Question: ${{Question with math problem.}}
 ```text
 ${{single line sympy expression that solves the problem}}
 ```
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/llms/anthropic_functions.py` & `gigachain_experimental-0.0.59/langchain_experimental/llms/anthropic_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import json
 from collections import defaultdict
 from html.parser import HTMLParser
 from typing import Any, DefaultDict, Dict, List, Optional, cast
 
-from langchain.callbacks.manager import (
-    CallbackManagerForLLMRun,
-)
 from langchain.schema import (
     ChatGeneration,
     ChatResult,
 )
 from langchain_community.chat_models.anthropic import ChatAnthropic
 from langchain_core._api.deprecation import deprecated
+from langchain_core.callbacks.manager import (
+    CallbackManagerForLLMRun,
+)
 from langchain_core.language_models import BaseChatModel
 from langchain_core.messages import (
     AIMessage,
     BaseMessage,
     SystemMessage,
 )
 
@@ -123,15 +123,15 @@
             raise ValueError
     else:
         raise ValueError
 
 
 @deprecated(
     since="0.0.54",
-    removal="0.2",
+    removal="0.3",
     alternative_import="langchain_anthropic.experimental.ChatAnthropicTools",
 )
 class AnthropicFunctions(BaseChatModel):
     """Chat model for interacting with Anthropic functions."""
 
     llm: BaseChatModel
 
@@ -180,15 +180,15 @@
             else:
                 stop.append("</tool_input>")
         else:
             if "function_call" in kwargs:
                 raise ValueError(
                     "if `function_call` provided, `functions` must also be"
                 )
-        response = self.model.predict_messages(
+        response = self.model.invoke(
             messages, stop=stop, callbacks=run_manager, **kwargs
         )
         completion = cast(str, response.content)
         if forced:
             tag_parser = TagParser()
 
             if "<tool_input>" in completion:
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/llms/jsonformer_decoder.py` & `gigachain_experimental-0.0.59/langchain_experimental/llms/jsonformer_decoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Experimental implementation of jsonformer wrapped LLM."""
 from __future__ import annotations
 
 import json
 from typing import TYPE_CHECKING, Any, List, Optional, cast
 
-from langchain.callbacks.manager import CallbackManagerForLLMRun
 from langchain_community.llms.huggingface_pipeline import HuggingFacePipeline
+from langchain_core.callbacks.manager import CallbackManagerForLLMRun
 
 from langchain_experimental.pydantic_v1 import Field, root_validator
 
 if TYPE_CHECKING:
     import jsonformer
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/llms/llamaapi.py` & `gigachain_experimental-0.0.59/langchain_experimental/llms/llamaapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,19 @@
     Dict,
     List,
     Mapping,
     Optional,
     Tuple,
 )
 
-from langchain.callbacks.manager import CallbackManagerForLLMRun
 from langchain.schema import (
     ChatGeneration,
     ChatResult,
 )
+from langchain_core.callbacks.manager import CallbackManagerForLLMRun
 from langchain_core.language_models import BaseChatModel
 from langchain_core.messages import (
     AIMessage,
     BaseMessage,
     ChatMessage,
     FunctionMessage,
     HumanMessage,
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/llms/lmformatenforcer_decoder.py` & `gigachain_experimental-0.0.59/langchain_experimental/llms/lmformatenforcer_decoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Experimental implementation of lm-format-enforcer wrapped LLM."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, List, Optional
 
-from langchain.callbacks.manager import CallbackManagerForLLMRun
 from langchain.schema import LLMResult
 from langchain_community.llms.huggingface_pipeline import HuggingFacePipeline
+from langchain_core.callbacks.manager import CallbackManagerForLLMRun
 
 from langchain_experimental.pydantic_v1 import Field
 
 if TYPE_CHECKING:
     import lmformatenforcer
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/llms/rellm_decoder.py` & `gigachain_experimental-0.0.59/langchain_experimental/llms/rellm_decoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Experimental implementation of RELLM wrapped LLM."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, List, Optional, cast
 
-from langchain.callbacks.manager import CallbackManagerForLLMRun
 from langchain_community.llms.huggingface_pipeline import HuggingFacePipeline
 from langchain_community.llms.utils import enforce_stop_tokens
+from langchain_core.callbacks.manager import CallbackManagerForLLMRun
 
 from langchain_experimental.pydantic_v1 import Field, root_validator
 
 if TYPE_CHECKING:
     import rellm
     from regex import Pattern as RegexPattern
 else:
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/open_clip/open_clip.py` & `gigachain_experimental-0.0.59/langchain_experimental/open_clip/open_clip.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/pal_chain/base.py` & `gigachain_experimental-0.0.59/langchain_experimental/pal_chain/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 """
 
 from __future__ import annotations
 
 import ast
 from typing import Any, Dict, List, Optional
 
-from langchain.callbacks.manager import CallbackManagerForChainRun
 from langchain.chains.base import Chain
 from langchain.chains.llm import LLMChain
 from langchain_community.utilities import PythonREPL
+from langchain_core.callbacks.manager import CallbackManagerForChainRun
 from langchain_core.language_models import BaseLanguageModel
 
 from langchain_experimental.pal_chain.colored_object_prompt import COLORED_OBJECT_PROMPT
 from langchain_experimental.pal_chain.math_prompt import MATH_PROMPT
 from langchain_experimental.pydantic_v1 import Extra, Field
 
 COMMAND_EXECUTION_FUNCTIONS = ["system", "exec", "execfile", "eval", "__import__"]
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/pal_chain/colored_object_prompt.py` & `gigachain_experimental-0.0.59/langchain_experimental/pal_chain/colored_object_prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # flake8: noqa
-from langchain.prompts.prompt import PromptTemplate
+from langchain_core.prompts.prompt import PromptTemplate
 
 template = (
     """
 # Генерация кода Python3 для решения задач
 # Q: На тумбочке находятся красный карандаш, фиолетовая кружка, бордовый брелок, розовый мишка, черная тарелка и синий мяч для снятия стресса. Какого цвета мяч для снятия стресса?
 # Поместим объекты в словарь для быстрого поиска
 objects = dict()
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/pal_chain/math_prompt.py` & `gigachain_experimental-0.0.59/langchain_experimental/pal_chain/math_prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # flake8: noqa
-from langchain.prompts.prompt import PromptTemplate
+from langchain_core.prompts.prompt import PromptTemplate
 
 template = (
     '''
 Q: У Оливии было $23. Она купила пять бейглов по $3 каждый. Сколько денег у неё осталось?
 
 # solution in Python:
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/plan_and_execute/agent_executor.py` & `gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/agent_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Optional
 
-from langchain.callbacks.manager import (
+from langchain.chains.base import Chain
+from langchain_core.callbacks.manager import (
     AsyncCallbackManagerForChainRun,
     CallbackManagerForChainRun,
 )
-from langchain.chains.base import Chain
 
 from langchain_experimental.plan_and_execute.executors.base import BaseExecutor
 from langchain_experimental.plan_and_execute.planners.base import BasePlanner
 from langchain_experimental.plan_and_execute.schema import (
     BaseStepContainer,
     ListStepContainer,
 )
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/plan_and_execute/executors/agent_executor.py` & `gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/executors/agent_executor.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/plan_and_execute/executors/base.py` & `gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/executors/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import abstractmethod
 from typing import Any
 
-from langchain.callbacks.manager import Callbacks
 from langchain.chains.base import Chain
+from langchain_core.callbacks.manager import Callbacks
 
 from langchain_experimental.plan_and_execute.schema import StepResponse
 from langchain_experimental.pydantic_v1 import BaseModel
 
 
 class BaseExecutor(BaseModel):
     """Base executor."""
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/plan_and_execute/planners/base.py` & `gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/planners/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import abstractmethod
 from typing import Any, List, Optional
 
-from langchain.callbacks.manager import Callbacks
 from langchain.chains.llm import LLMChain
+from langchain_core.callbacks.manager import Callbacks
 
 from langchain_experimental.plan_and_execute.schema import Plan, PlanOutputParser
 from langchain_experimental.pydantic_v1 import BaseModel
 
 
 class BasePlanner(BaseModel):
     """Base planner."""
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/plan_and_execute/planners/chat_planner.py` & `gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/planners/chat_planner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 
 from langchain.chains import LLMChain
-from langchain.prompts import ChatPromptTemplate, HumanMessagePromptTemplate
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.messages import SystemMessage
+from langchain_core.prompts import ChatPromptTemplate, HumanMessagePromptTemplate
 
 from langchain_experimental.plan_and_execute.planners.base import LLMPlanner
 from langchain_experimental.plan_and_execute.schema import (
     Plan,
     PlanOutputParser,
     Step,
 )
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/plan_and_execute/schema.py` & `gigachain_experimental-0.0.59/langchain_experimental/plan_and_execute/schema.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/prompt_injection_identifier/hugging_face_identifier.py` & `gigachain_experimental-0.0.59/langchain_experimental/prompt_injection_identifier/hugging_face_identifier.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self.message = message
         self.score = score
 
         super().__init__(self.message)
 
 
 def _model_default_factory(
-    model_name: str = "laiyer/deberta-v3-base-prompt-injection",
+    model_name: str = "protectai/deberta-v3-base-prompt-injection-v2",
 ) -> Pipeline:
     try:
         from transformers import (
             AutoModelForSequenceClassification,
             AutoTokenizer,
             pipeline,
         )
@@ -60,15 +60,15 @@
         "Input should be any message from the user."
     )
     model: Union[Pipeline, str, None] = Field(default_factory=_model_default_factory)
     """Model to use for prompt injection detection. 
     
     Can be specified as transformers Pipeline or string. String should correspond to the
         model name of a text-classification transformers model. Defaults to 
-        ``laiyer/deberta-v3-base-prompt-injection`` model.
+        ``protectai/deberta-v3-base-prompt-injection-v2`` model.
     """
     threshold: float = Field(
         description="Threshold for prompt injection detection.", default=0.5
     )
     """Threshold for prompt injection detection.
     
     Defaults to 0.5."""
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/pydantic_v1/__init__.py` & `gigachain_experimental-0.0.59/langchain_experimental/pydantic_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/pydantic_v1/dataclasses.py` & `gigachain_experimental-0.0.59/langchain_experimental/pydantic_v1/dataclasses.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/pydantic_v1/main.py` & `gigachain_experimental-0.0.59/langchain_experimental/pydantic_v1/main.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/recommenders/__init__.py` & `gigachain_experimental-0.0.59/langchain_experimental/recommenders/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/recommenders/amazon_personalize.py` & `gigachain_experimental-0.0.59/langchain_experimental/recommenders/amazon_personalize.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/recommenders/amazon_personalize_chain.py` & `gigachain_experimental-0.0.59/langchain_experimental/recommenders/amazon_personalize_chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from typing import Any, Dict, List, Mapping, Optional, cast
 
-from langchain.callbacks.manager import (
-    CallbackManagerForChainRun,
-)
 from langchain.chains import LLMChain
 from langchain.chains.base import Chain
-from langchain.prompts.prompt import PromptTemplate
 from langchain.schema.language_model import BaseLanguageModel
+from langchain_core.callbacks.manager import (
+    CallbackManagerForChainRun,
+)
+from langchain_core.prompts.prompt import PromptTemplate
 
 from langchain_experimental.recommenders.amazon_personalize import AmazonPersonalize
 
 SUMMARIZE_PROMPT_QUERY = """
 Summarize the recommended items for a user from the items list in tag <result> below.
 Make correlation into the items in the list and provide a summary.
     <result>
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/retrievers/vector_sql_database.py` & `gigachain_experimental-0.0.59/langchain_experimental/retrievers/vector_sql_database.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Vector SQL Database Chain Retriever"""
 
 from typing import Any, Dict, List
 
-from langchain.callbacks.manager import (
+from langchain_core.callbacks.manager import (
     AsyncCallbackManagerForRetrieverRun,
     CallbackManagerForRetrieverRun,
 )
 from langchain_core.documents import Document
 from langchain_core.retrievers import BaseRetriever
 
 from langchain_experimental.sql.vector_sql import VectorSQLDatabaseChain
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/rl_chain/__init__.py` & `gigachain_experimental-0.0.59/langchain_experimental/rl_chain/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/rl_chain/base.py` & `gigachain_experimental-0.0.59/langchain_experimental/rl_chain/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,18 +12,18 @@
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
-from langchain.callbacks.manager import CallbackManagerForChainRun
 from langchain.chains.base import Chain
 from langchain.chains.llm import LLMChain
-from langchain.prompts import (
+from langchain_core.callbacks.manager import CallbackManagerForChainRun
+from langchain_core.prompts import (
     BasePromptTemplate,
     ChatPromptTemplate,
     HumanMessagePromptTemplate,
     SystemMessagePromptTemplate,
 )
 
 from langchain_experimental.pydantic_v1 import BaseModel, Extra, root_validator
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/rl_chain/metrics.py` & `gigachain_experimental-0.0.59/langchain_experimental/rl_chain/metrics.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/rl_chain/model_repository.py` & `gigachain_experimental-0.0.59/langchain_experimental/rl_chain/model_repository.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/rl_chain/pick_best_chain.py` & `gigachain_experimental-0.0.59/langchain_experimental/rl_chain/pick_best_chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import logging
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 from langchain.base_language import BaseLanguageModel
-from langchain.callbacks.manager import CallbackManagerForChainRun
 from langchain.chains.llm import LLMChain
-from langchain.prompts import BasePromptTemplate
+from langchain_core.callbacks.manager import CallbackManagerForChainRun
+from langchain_core.prompts import BasePromptTemplate
 
 import langchain_experimental.rl_chain.base as base
 
 logger = logging.getLogger(__name__)
 
 # sentinel object used to distinguish between
 # user didn't supply anything or user explicitly supplied None
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/rl_chain/vw_logger.py` & `gigachain_experimental-0.0.59/langchain_experimental/rl_chain/vw_logger.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/smart_llm/__init__.py` & `gigachain_experimental-0.0.59/langchain_experimental/smart_llm/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/smart_llm/base.py` & `gigachain_experimental-0.0.59/langchain_experimental/smart_llm/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Chain for applying self-critique using the SmartGPT workflow."""
 from typing import Any, Dict, List, Optional, Tuple, Type
 
 from langchain.base_language import BaseLanguageModel
-from langchain.callbacks.manager import CallbackManagerForChainRun
 from langchain.chains.base import Chain
 from langchain.input import get_colored_text
-from langchain.prompts.base import BasePromptTemplate
-from langchain.prompts.chat import (
+from langchain.schema import LLMResult, PromptValue
+from langchain_core.callbacks.manager import CallbackManagerForChainRun
+from langchain_core.prompts.base import BasePromptTemplate
+from langchain_core.prompts.chat import (
     AIMessagePromptTemplate,
     BaseMessagePromptTemplate,
     ChatPromptTemplate,
     HumanMessagePromptTemplate,
 )
-from langchain.schema import LLMResult, PromptValue
 
 from langchain_experimental.pydantic_v1 import Extra, root_validator
 
 
 class SmartLLMChain(Chain):
     """Chain for applying self-critique using the SmartGPT workflow.
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/sql/base.py` & `gigachain_experimental-0.0.59/langchain_experimental/sql/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Chain for interacting with SQL Database."""
 from __future__ import annotations
 
 import warnings
 from typing import Any, Dict, List, Optional
 
-from langchain.callbacks.manager import CallbackManagerForChainRun
 from langchain.chains.base import Chain
 from langchain.chains.llm import LLMChain
 from langchain.chains.sql_database.prompt import DECIDER_PROMPT, PROMPT, SQL_PROMPTS
-from langchain.prompts.prompt import PromptTemplate
 from langchain.schema import BasePromptTemplate
 from langchain_community.tools.sql_database.prompt import QUERY_CHECKER
 from langchain_community.utilities.sql_database import SQLDatabase
+from langchain_core.callbacks.manager import CallbackManagerForChainRun
 from langchain_core.language_models import BaseLanguageModel
+from langchain_core.prompts.prompt import PromptTemplate
 
 from langchain_experimental.pydantic_v1 import Extra, Field, root_validator
 
 INTERMEDIATE_STEPS_KEY = "intermediate_steps"
 SQL_QUERY = "SQLQuery:"
 SQL_RESULT = "SQLResult:"
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/sql/prompt.py` & `gigachain_experimental-0.0.59/langchain_experimental/sql/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # flake8: noqa
-from langchain.prompts.prompt import PromptTemplate
+from langchain_core.prompts.prompt import PromptTemplate
 
 
 PROMPT_SUFFIX = """Only use the following tables:
 {table_info}
 
 Question: {input}"""
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/sql/vector_sql.py` & `gigachain_experimental-0.0.59/langchain_experimental/sql/vector_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Vector SQL Database Chain Retriever"""
 
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Sequence, Union
 
-from langchain.callbacks.manager import CallbackManagerForChainRun
 from langchain.chains.llm import LLMChain
 from langchain.chains.sql_database.prompt import PROMPT, SQL_PROMPTS
-from langchain.prompts.prompt import PromptTemplate
 from langchain_community.tools.sql_database.prompt import QUERY_CHECKER
 from langchain_community.utilities.sql_database import SQLDatabase
+from langchain_core.callbacks.manager import CallbackManagerForChainRun
 from langchain_core.embeddings import Embeddings
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.output_parsers import BaseOutputParser
 from langchain_core.prompts import BasePromptTemplate
+from langchain_core.prompts.prompt import PromptTemplate
 
 from langchain_experimental.sql.base import INTERMEDIATE_STEPS_KEY, SQLDatabaseChain
 
 
 class VectorSQLOutputParser(BaseOutputParser[str]):
     """Output Parser for Vector SQL.
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/synthetic_data/__init__.py` & `gigachain_experimental-0.0.59/langchain_experimental/synthetic_data/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/tabular_synthetic_data/base.py` & `gigachain_experimental-0.0.59/langchain_experimental/tabular_synthetic_data/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 from typing import Any, Dict, List, Optional, Union
 
 from langchain.chains.base import Chain
 from langchain.chains.llm import LLMChain
-from langchain.prompts.few_shot import FewShotPromptTemplate
 from langchain.pydantic_v1 import BaseModel, root_validator
 from langchain_core.language_models import BaseLanguageModel
+from langchain_core.prompts.few_shot import FewShotPromptTemplate
 
 
 class SyntheticDataGenerator(BaseModel):
     """Generate synthetic data using the given LLM and few-shot template.
 
     Utilizes the provided LLM to produce synthetic data based on the
     few-shot prompt template.
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/tabular_synthetic_data/openai.py` & `gigachain_experimental-0.0.59/langchain_experimental/tabular_synthetic_data/openai.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/text_splitter.py` & `gigachain_experimental-0.0.59/langchain_experimental/text_splitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,20 +108,22 @@
         self,
         embeddings: Embeddings,
         buffer_size: int = 1,
         add_start_index: bool = False,
         breakpoint_threshold_type: BreakpointThresholdType = "percentile",
         breakpoint_threshold_amount: Optional[float] = None,
         number_of_chunks: Optional[int] = None,
+        sentence_split_regex: str = r"(?<=[.?!])\s+",
     ):
         self._add_start_index = add_start_index
         self.embeddings = embeddings
         self.buffer_size = buffer_size
         self.breakpoint_threshold_type = breakpoint_threshold_type
         self.number_of_chunks = number_of_chunks
+        self.sentence_split_regex = sentence_split_regex
         if breakpoint_threshold_amount is None:
             self.breakpoint_threshold_amount = BREAKPOINT_DEFAULTS[
                 breakpoint_threshold_type
             ]
         else:
             self.breakpoint_threshold_amount = breakpoint_threshold_amount
 
@@ -185,16 +187,16 @@
 
         return calculate_cosine_distances(sentences)
 
     def split_text(
         self,
         text: str,
     ) -> List[str]:
-        # Splitting the essay on '.', '?', and '!'
-        single_sentences_list = re.split(r"(?<=[.?!])\s+", text)
+        # Splitting the essay (by default on '.', '?', and '!')
+        single_sentences_list = re.split(self.sentence_split_regex, text)
 
         # having len(single_sentences_list) == 1 would cause the following
         # np.percentile to fail.
         if len(single_sentences_list) == 1:
             return single_sentences_list
         distances, sentences = self._calculate_sentence_distances(single_sentences_list)
         if self.number_of_chunks is not None:
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/tools/python/tool.py` & `gigachain_experimental-0.0.59/langchain_experimental/tools/python/tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import ast
 import re
 import sys
 from contextlib import redirect_stdout
 from io import StringIO
 from typing import Any, Dict, Optional, Type
 
-from langchain.callbacks.manager import (
+from langchain.pydantic_v1 import BaseModel, Field, root_validator
+from langchain.tools.base import BaseTool
+from langchain_core.callbacks.manager import (
     AsyncCallbackManagerForToolRun,
     CallbackManagerForToolRun,
 )
-from langchain.pydantic_v1 import BaseModel, Field, root_validator
-from langchain.tools.base import BaseTool
 from langchain_core.runnables.config import run_in_executor
 
 from langchain_experimental.utilities.python import PythonREPL
 
 
 def _get_default_python_repl() -> PythonREPL:
     return PythonREPL(_globals=globals(), _locals=None)
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/tot/base.py` & `gigachain_experimental-0.0.59/langchain_experimental/tot/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from textwrap import indent
 from typing import Any, Dict, List, Optional, Type
 
 from langchain.base_language import BaseLanguageModel
-from langchain.callbacks.manager import (
+from langchain.chains.base import Chain
+from langchain_core.callbacks.manager import (
     AsyncCallbackManagerForChainRun,
     CallbackManagerForChainRun,
 )
-from langchain.chains.base import Chain
 
 from langchain_experimental.pydantic_v1 import Extra
 from langchain_experimental.tot.checker import ToTChecker
 from langchain_experimental.tot.controller import ToTController
 from langchain_experimental.tot.memory import ToTDFSMemory
 from langchain_experimental.tot.thought import Thought, ThoughtValidity
 from langchain_experimental.tot.thought_generation import (
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/tot/checker.py` & `gigachain_experimental-0.0.59/langchain_experimental/tot/checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Optional, Tuple
 
-from langchain.callbacks.manager import CallbackManagerForChainRun
 from langchain.chains.base import Chain
+from langchain_core.callbacks.manager import CallbackManagerForChainRun
 
 from langchain_experimental.tot.thought import ThoughtValidity
 
 
 class ToTChecker(Chain, ABC):
     """
     Tree of Thought (ToT) checker.
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/tot/controller.py` & `gigachain_experimental-0.0.59/langchain_experimental/tot/controller.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/tot/memory.py` & `gigachain_experimental-0.0.59/langchain_experimental/tot/memory.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/tot/prompts.py` & `gigachain_experimental-0.0.59/langchain_experimental/tot/prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/tot/thought_generation.py` & `gigachain_experimental-0.0.59/langchain_experimental/tot/thought_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 non-repeating thoughts, which are crucial for problem-solving tasks that require
 exploration.
 """
 from abc import abstractmethod
 from typing import Any, Dict, List, Tuple
 
 from langchain.chains.llm import LLMChain
-from langchain.prompts.base import BasePromptTemplate
+from langchain_core.prompts.base import BasePromptTemplate
 
 from langchain_experimental.pydantic_v1 import Field
 from langchain_experimental.tot.prompts import get_cot_prompt, get_propose_prompt
 
 
 class BaseThoughtGenerationStrategy(LLMChain):
     """
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/utilities/python.py` & `gigachain_experimental-0.0.59/langchain_experimental/utilities/python.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import functools
 import logging
 import multiprocessing
+import re
 import sys
 from io import StringIO
 from typing import Dict, Optional
 
 from langchain.pydantic_v1 import BaseModel, Field
 
 logger = logging.getLogger(__name__)
@@ -18,26 +19,44 @@
 
 class PythonREPL(BaseModel):
     """Simulates a standalone Python REPL."""
 
     globals: Optional[Dict] = Field(default_factory=dict, alias="_globals")
     locals: Optional[Dict] = Field(default_factory=dict, alias="_locals")
 
+    @staticmethod
+    def sanitize_input(query: str) -> str:
+        """Sanitize input to the python REPL.
+
+        Remove whitespace, backtick & python
+        (if llm mistakes python console as terminal)
+
+        Args:
+            query: The query to sanitize
+
+        Returns:
+            str: The sanitized query
+        """
+        query = re.sub(r"^(\s|`)*(?i:python)?\s*", "", query)
+        query = re.sub(r"(\s|`)*$", "", query)
+        return query
+
     @classmethod
     def worker(
         cls,
         command: str,
         globals: Optional[Dict],
         locals: Optional[Dict],
         queue: multiprocessing.Queue,
     ) -> None:
         old_stdout = sys.stdout
         sys.stdout = mystdout = StringIO()
         try:
-            exec(command, globals, locals)
+            cleaned_command = cls.sanitize_input(command)
+            exec(cleaned_command, globals, locals)
             sys.stdout = old_stdout
             queue.put(mystdout.getvalue())
         except Exception as e:
             sys.stdout = old_stdout
             queue.put(repr(e))
 
     def run(self, command: str, timeout: Optional[int] = None) -> str:
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/video_captioning/base.py` & `gigachain_experimental-0.0.59/langchain_experimental/video_captioning/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/video_captioning/models.py` & `gigachain_experimental-0.0.59/langchain_experimental/video_captioning/models.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/video_captioning/prompts.py` & `gigachain_experimental-0.0.59/langchain_experimental/video_captioning/prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/video_captioning/services/audio_service.py` & `gigachain_experimental-0.0.59/langchain_experimental/video_captioning/services/audio_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import subprocess
 from pathlib import Path
 from typing import List, Optional
 
-from langchain.callbacks.manager import CallbackManagerForChainRun
 from langchain.schema import Document
 from langchain_community.document_loaders import AssemblyAIAudioTranscriptLoader
 from langchain_community.document_loaders.assemblyai import TranscriptFormat
+from langchain_core.callbacks.manager import CallbackManagerForChainRun
 
 from langchain_experimental.video_captioning.models import AudioModel, BaseModel
 
 
 class AudioProcessor:
     def __init__(
         self,
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/video_captioning/services/caption_service.py` & `gigachain_experimental-0.0.59/langchain_experimental/video_captioning/services/caption_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, List, Optional, Tuple
 
-from langchain.callbacks.manager import CallbackManagerForChainRun
 from langchain.chains.llm import LLMChain
+from langchain_core.callbacks.manager import CallbackManagerForChainRun
 from langchain_core.language_models import BaseLanguageModel
 
 from langchain_experimental.video_captioning.models import VideoModel
 from langchain_experimental.video_captioning.prompts import (
     JOIN_SIMILAR_VIDEO_MODELS_PROMPT,
     REMOVE_VIDEO_MODEL_DESCRIPTION_PROMPT,
 )
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/video_captioning/services/combine_service.py` & `gigachain_experimental-0.0.59/langchain_experimental/video_captioning/services/combine_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, List, Optional, Tuple
 
-from langchain.callbacks.manager import CallbackManagerForChainRun
 from langchain.chains.llm import LLMChain
 from langchain.schema.language_model import BaseLanguageModel
+from langchain_core.callbacks.manager import CallbackManagerForChainRun
 
 from langchain_experimental.video_captioning.models import (
     AudioModel,
     CaptionModel,
     VideoModel,
 )
 from langchain_experimental.video_captioning.prompts import (
```

### Comparing `gigachain_experimental-0.0.57/langchain_experimental/video_captioning/services/image_service.py` & `gigachain_experimental-0.0.59/langchain_experimental/video_captioning/services/image_service.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.57/pyproject.toml` & `gigachain_experimental-0.0.59/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "gigachain-experimental"
-version = "0.0.57"
+version = "0.0.59"
 description = "Building applications with LLMs through composability"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ai-forever/gigachain"
 packages = [
     {include = "langchain_experimental"}
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-gigachain-core = "^0.1.41"
-gigachain = "^0.1.15"
+gigachain-core = "^0.2"
+gigachain-community = "^0.2"
 presidio-anonymizer = {version = "^2.2.352", optional = true}
 presidio-analyzer = {version = "^2.2.352", optional = true}
 faker = {version = "^19.3.1", optional = true}
 vowpal-wabbit-next = {version = "0.6.0", optional = true}
 sentence-transformers = {version = "^2", optional = true}
 jinja2 = {version = "^3", optional = true}
 pandas = { version = "^2.0.1", optional = true }
@@ -58,15 +58,17 @@
 # dependencies used for running tests (e.g., pytest, freezegun, response).
 # Any dependencies that do not meet that criteria will be removed.
 pytest = "^7.3.0"
 pytest-asyncio = "^0.20.3"
 gigachain = {path = "../langchain", develop = true}
 gigachain-core = {path = "../core", develop = true}
 gigachain-community = {path = "../community", develop = true}
-gigachat = "^0.1.22"
+gigachain-text-splitters = {path = "../text-splitters", develop = true}
+gigachat = "^0.1.27"
+
 
 [tool.poetry.group.test_integration]
 optional = true
 
 [tool.poetry.group.test_integration.dependencies]
 gigachain = {path = "../langchain", develop = true}
 gigachain-core = {path = "../core", develop = true}
```

### Comparing `gigachain_experimental-0.0.57/PKG-INFO` & `gigachain_experimental-0.0.59/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gigachain-experimental
-Version: 0.0.57
+Version: 0.0.59
 Summary: Building applications with LLMs through composability
 Home-page: https://github.com/ai-forever/gigachain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: extended-testing
 Requires-Dist: faker (>=19.3.1,<20.0.0) ; extra == "extended-testing"
-Requires-Dist: gigachain (>=0.1.15,<0.2.0)
-Requires-Dist: gigachain-core (>=0.1.41,<0.2.0)
+Requires-Dist: gigachain-community (>=0.2,<0.3)
+Requires-Dist: gigachain-core (>=0.2,<0.3)
 Requires-Dist: jinja2 (>=3,<4) ; extra == "extended-testing"
 Requires-Dist: pandas (>=2.0.1,<3.0.0) ; extra == "extended-testing"
 Requires-Dist: presidio-analyzer (>=2.2.352,<3.0.0) ; extra == "extended-testing"
 Requires-Dist: presidio-anonymizer (>=2.2.352,<3.0.0) ; extra == "extended-testing"
 Requires-Dist: sentence-transformers (>=2,<3) ; extra == "extended-testing"
 Requires-Dist: tabulate (>=0.9.0,<0.10.0) ; extra == "extended-testing"
 Requires-Dist: vowpal-wabbit-next (==0.6.0) ; extra == "extended-testing"
```

