# Comparing `tmp/gigachain-0.1.9.tar.gz` & `tmp/gigachain-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigachain-0.1.9.tar", max compression
+gzip compressed data, was "gigachain-0.2.0.tar", max compression
```

## Comparing `gigachain-0.1.9.tar` & `gigachain-0.2.0.tar`

### file list

```diff
@@ -1,1338 +1,1352 @@
--rw-r--r--   0        0        0     1067 2023-11-15 10:30:09.324245 gigachain-0.1.9/LICENSE
--rw-r--r--   0        0        0     5879 2024-02-22 08:54:03.058827 gigachain-0.1.9/README.md
--rw-r--r--   0        0        0    14039 2024-02-22 08:54:03.062847 gigachain-0.1.9/langchain/__init__.py
--rw-r--r--   0        0        0      667 2023-10-03 14:24:35.511215 gigachain-0.1.9/langchain/_api/__init__.py
--rw-r--r--   0        0        0      471 2023-12-18 12:05:46.810499 gigachain-0.1.9/langchain/_api/deprecation.py
--rw-r--r--   0        0        0      122 2023-12-18 12:05:46.811728 gigachain-0.1.9/langchain/_api/path.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.531593 gigachain-0.1.9/langchain/adapters/__init__.py
--rw-r--r--   0        0        0      653 2024-01-10 09:04:40.316153 gigachain-0.1.9/langchain/adapters/openai.py
--rw-r--r--   0        0        0     4952 2024-02-22 08:54:03.066384 gigachain-0.1.9/langchain/agents/__init__.py
--rw-r--r--   0        0        0    54823 2024-02-22 08:54:03.070466 gigachain-0.1.9/langchain/agents/agent.py
--rw-r--r--   0        0        0    15135 2024-02-22 08:54:03.072200 gigachain-0.1.9/langchain/agents/agent_iterator.py
--rw-r--r--   0        0        0     3678 2024-02-22 08:54:03.075025 gigachain-0.1.9/langchain/agents/agent_toolkits/__init__.py
--rw-r--r--   0        0        0       25 2023-08-24 07:36:02.856871 gigachain-0.1.9/langchain/agents/agent_toolkits/ainetwork/__init__.py
--rw-r--r--   0        0        0      114 2023-12-18 12:05:46.824912 gigachain-0.1.9/langchain/agents/agent_toolkits/ainetwork/toolkit.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:46.825868 gigachain-0.1.9/langchain/agents/agent_toolkits/amadeus/toolkit.py
--rw-r--r--   0        0        0      156 2023-12-18 12:05:46.826776 gigachain-0.1.9/langchain/agents/agent_toolkits/azure_cognitive_services.py
--rw-r--r--   0        0        0       91 2023-12-18 12:05:46.827627 gigachain-0.1.9/langchain/agents/agent_toolkits/base.py
--rw-r--r--   0        0        0        0 2023-10-06 14:43:01.368502 gigachain-0.1.9/langchain/agents/agent_toolkits/clickup/__init__.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:46.828657 gigachain-0.1.9/langchain/agents/agent_toolkits/clickup/toolkit.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.534160 gigachain-0.1.9/langchain/agents/agent_toolkits/conversational_retrieval/__init__.py
--rw-r--r--   0        0        0     3235 2023-12-18 12:05:46.830026 gigachain-0.1.9/langchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py
--rw-r--r--   0        0        0       97 2023-10-30 16:05:53.823759 gigachain-0.1.9/langchain/agents/agent_toolkits/conversational_retrieval/tool.py
--rw-r--r--   0        0        0     1091 2023-12-18 12:05:46.831119 gigachain-0.1.9/langchain/agents/agent_toolkits/csv/__init__.py
--rw-r--r--   0        0        0      177 2024-01-18 15:16:40.601939 gigachain-0.1.9/langchain/agents/agent_toolkits/file_management/__init__.py
--rw-r--r--   0        0        0      139 2024-01-10 09:04:40.318190 gigachain-0.1.9/langchain/agents/agent_toolkits/file_management/toolkit.py
--rw-r--r--   0        0        0       22 2023-08-21 13:51:28.536932 gigachain-0.1.9/langchain/agents/agent_toolkits/github/__init__.py
--rw-r--r--   0        0        0      617 2023-12-18 12:05:46.832827 gigachain-0.1.9/langchain/agents/agent_toolkits/github/toolkit.py
--rw-r--r--   0        0        0       22 2023-09-19 14:33:02.213182 gigachain-0.1.9/langchain/agents/agent_toolkits/gitlab/__init__.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:46.833490 gigachain-0.1.9/langchain/agents/agent_toolkits/gitlab/toolkit.py
--rw-r--r--   0        0        0       21 2023-08-21 13:51:28.537602 gigachain-0.1.9/langchain/agents/agent_toolkits/gmail/__init__.py
--rw-r--r--   0        0        0      120 2023-12-18 12:05:46.834225 gigachain-0.1.9/langchain/agents/agent_toolkits/gmail/toolkit.py
--rw-r--r--   0        0        0       20 2023-08-21 13:51:28.538134 gigachain-0.1.9/langchain/agents/agent_toolkits/jira/__init__.py
--rw-r--r--   0        0        0       99 2023-12-18 12:05:46.834919 gigachain-0.1.9/langchain/agents/agent_toolkits/jira/toolkit.py
--rw-r--r--   0        0        0       18 2023-08-21 13:51:28.538568 gigachain-0.1.9/langchain/agents/agent_toolkits/json/__init__.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:46.835830 gigachain-0.1.9/langchain/agents/agent_toolkits/json/base.py
--rw-r--r--   0        0        0      126 2023-12-18 12:05:46.837036 gigachain-0.1.9/langchain/agents/agent_toolkits/json/prompt.py
--rw-r--r--   0        0        0       99 2023-12-18 12:05:46.841473 gigachain-0.1.9/langchain/agents/agent_toolkits/json/toolkit.py
--rw-r--r--   0        0        0       23 2023-08-21 13:51:28.539651 gigachain-0.1.9/langchain/agents/agent_toolkits/multion/__init__.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:46.842445 gigachain-0.1.9/langchain/agents/agent_toolkits/multion/toolkit.py
--rw-r--r--   0        0        0       19 2023-12-18 12:05:46.842756 gigachain-0.1.9/langchain/agents/agent_toolkits/nasa/__init__.py
--rw-r--r--   0        0        0       99 2023-12-18 12:05:46.843062 gigachain-0.1.9/langchain/agents/agent_toolkits/nasa/toolkit.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.540099 gigachain-0.1.9/langchain/agents/agent_toolkits/nla/__init__.py
--rw-r--r--   0        0        0       87 2023-12-18 12:05:46.843983 gigachain-0.1.9/langchain/agents/agent_toolkits/nla/tool.py
--rw-r--r--   0        0        0       96 2023-12-18 12:05:46.844896 gigachain-0.1.9/langchain/agents/agent_toolkits/nla/toolkit.py
--rw-r--r--   0        0        0       25 2023-08-21 13:51:28.541150 gigachain-0.1.9/langchain/agents/agent_toolkits/office365/__init__.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:46.845738 gigachain-0.1.9/langchain/agents/agent_toolkits/office365/toolkit.py
--rw-r--r--   0        0        0       26 2023-08-21 13:51:28.541736 gigachain-0.1.9/langchain/agents/agent_toolkits/openapi/__init__.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:46.846914 gigachain-0.1.9/langchain/agents/agent_toolkits/openapi/base.py
--rw-r--r--   0        0        0      530 2024-01-10 09:04:40.319042 gigachain-0.1.9/langchain/agents/agent_toolkits/openapi/planner.py
--rw-r--r--   0        0        0     1153 2023-12-18 12:05:46.848467 gigachain-0.1.9/langchain/agents/agent_toolkits/openapi/planner_prompt.py
--rw-r--r--   0        0        0      186 2023-12-18 12:05:46.849502 gigachain-0.1.9/langchain/agents/agent_toolkits/openapi/prompt.py
--rw-r--r--   0        0        0      170 2023-12-18 12:05:46.850112 gigachain-0.1.9/langchain/agents/agent_toolkits/openapi/spec.py
--rw-r--r--   0        0        0      157 2023-12-18 12:05:46.850853 gigachain-0.1.9/langchain/agents/agent_toolkits/openapi/toolkit.py
--rw-r--r--   0        0        0     1104 2023-12-18 12:05:46.851835 gigachain-0.1.9/langchain/agents/agent_toolkits/pandas/__init__.py
--rw-r--r--   0        0        0      174 2024-01-18 15:16:40.603187 gigachain-0.1.9/langchain/agents/agent_toolkits/playwright/__init__.py
--rw-r--r--   0        0        0      140 2023-12-18 12:05:46.852728 gigachain-0.1.9/langchain/agents/agent_toolkits/playwright/toolkit.py
--rw-r--r--   0        0        0       22 2023-08-21 13:51:28.545958 gigachain-0.1.9/langchain/agents/agent_toolkits/powerbi/__init__.py
--rw-r--r--   0        0        0      109 2023-12-18 12:05:46.853881 gigachain-0.1.9/langchain/agents/agent_toolkits/powerbi/base.py
--rw-r--r--   0        0        0      124 2023-12-18 12:05:46.854708 gigachain-0.1.9/langchain/agents/agent_toolkits/powerbi/chat_base.py
--rw-r--r--   0        0        0      269 2023-12-18 12:05:46.855739 gigachain-0.1.9/langchain/agents/agent_toolkits/powerbi/prompt.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:46.856940 gigachain-0.1.9/langchain/agents/agent_toolkits/powerbi/toolkit.py
--rw-r--r--   0        0        0     1094 2023-12-18 12:05:46.857872 gigachain-0.1.9/langchain/agents/agent_toolkits/python/__init__.py
--rw-r--r--   0        0        0       21 2023-12-18 12:05:46.858297 gigachain-0.1.9/langchain/agents/agent_toolkits/slack/__init__.py
--rw-r--r--   0        0        0      102 2023-12-18 12:05:46.859032 gigachain-0.1.9/langchain/agents/agent_toolkits/slack/toolkit.py
--rw-r--r--   0        0        0     1103 2023-12-18 12:05:46.860134 gigachain-0.1.9/langchain/agents/agent_toolkits/spark/__init__.py
--rw-r--r--   0        0        0       23 2023-08-21 13:51:28.548199 gigachain-0.1.9/langchain/agents/agent_toolkits/spark_sql/__init__.py
--rw-r--r--   0        0        0      123 2023-12-18 12:05:46.861223 gigachain-0.1.9/langchain/agents/agent_toolkits/spark_sql/base.py
--rw-r--r--   0        0        0      127 2023-12-18 12:05:46.862436 gigachain-0.1.9/langchain/agents/agent_toolkits/spark_sql/prompt.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:46.863534 gigachain-0.1.9/langchain/agents/agent_toolkits/spark_sql/toolkit.py
--rw-r--r--   0        0        0       17 2023-08-21 13:51:28.549117 gigachain-0.1.9/langchain/agents/agent_toolkits/sql/__init__.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:46.864520 gigachain-0.1.9/langchain/agents/agent_toolkits/sql/base.py
--rw-r--r--   0        0        0      184 2023-12-18 12:05:46.865869 gigachain-0.1.9/langchain/agents/agent_toolkits/sql/prompt.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:46.866709 gigachain-0.1.9/langchain/agents/agent_toolkits/sql/toolkit.py
--rw-r--r--   0        0        0       21 2023-12-18 12:05:46.867144 gigachain-0.1.9/langchain/agents/agent_toolkits/steam/__init__.py
--rw-r--r--   0        0        0      102 2023-12-18 12:05:46.867506 gigachain-0.1.9/langchain/agents/agent_toolkits/steam/toolkit.py
--rw-r--r--   0        0        0       56 2023-08-21 13:51:28.549949 gigachain-0.1.9/langchain/agents/agent_toolkits/vectorstore/__init__.py
--rw-r--r--   0        0        0     4211 2023-12-18 12:05:46.868458 gigachain-0.1.9/langchain/agents/agent_toolkits/vectorstore/base.py
--rw-r--r--   0        0        0     1557 2023-08-31 07:54:47.805977 gigachain-0.1.9/langchain/agents/agent_toolkits/vectorstore/prompt.py
--rw-r--r--   0        0        0     3001 2024-01-18 15:16:40.604061 gigachain-0.1.9/langchain/agents/agent_toolkits/vectorstore/toolkit.py
--rw-r--r--   0        0        0     1095 2023-12-18 12:05:46.870552 gigachain-0.1.9/langchain/agents/agent_toolkits/xorbits/__init__.py
--rw-r--r--   0        0        0       22 2023-08-21 13:51:28.551302 gigachain-0.1.9/langchain/agents/agent_toolkits/zapier/__init__.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:46.871982 gigachain-0.1.9/langchain/agents/agent_toolkits/zapier/toolkit.py
--rw-r--r--   0        0        0     1948 2024-01-30 12:21:20.018308 gigachain-0.1.9/langchain/agents/agent_types.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.551838 gigachain-0.1.9/langchain/agents/chat/__init__.py
--rw-r--r--   0        0        0     5084 2024-02-22 08:54:03.075995 gigachain-0.1.9/langchain/agents/chat/base.py
--rw-r--r--   0        0        0     1977 2024-02-22 08:54:03.079601 gigachain-0.1.9/langchain/agents/chat/output_parser.py
--rw-r--r--   0        0        0     1776 2023-10-19 12:57:52.688319 gigachain-0.1.9/langchain/agents/chat/prompt.py
--rw-r--r--   0        0        0       75 2023-08-21 13:51:28.552791 gigachain-0.1.9/langchain/agents/conversational/__init__.py
--rw-r--r--   0        0        0     4957 2024-02-22 08:54:03.081376 gigachain-0.1.9/langchain/agents/conversational/base.py
--rw-r--r--   0        0        0     1463 2024-02-22 08:54:03.084332 gigachain-0.1.9/langchain/agents/conversational/output_parser.py
--rw-r--r--   0        0        0     1312 2023-10-19 12:57:52.695256 gigachain-0.1.9/langchain/agents/conversational/prompt.py
--rw-r--r--   0        0        0       75 2023-08-21 13:51:28.553657 gigachain-0.1.9/langchain/agents/conversational_chat/__init__.py
--rw-r--r--   0        0        0     5264 2024-02-22 08:54:03.087665 gigachain-0.1.9/langchain/agents/conversational_chat/base.py
--rw-r--r--   0        0        0     2398 2024-02-22 08:54:03.088654 gigachain-0.1.9/langchain/agents/conversational_chat/output_parser.py
--rw-r--r--   0        0        0     2934 2023-10-19 12:57:52.702190 gigachain-0.1.9/langchain/agents/conversational_chat/prompt.py
--rw-r--r--   0        0        0      847 2023-11-10 13:07:49.983002 gigachain-0.1.9/langchain/agents/format_scratchpad/__init__.py
--rw-r--r--   0        0        0     2209 2024-02-22 08:54:03.092203 gigachain-0.1.9/langchain/agents/format_scratchpad/gigachat_functions.py
--rw-r--r--   0        0        0     1885 2024-02-22 08:54:03.093583 gigachain-0.1.9/langchain/agents/format_scratchpad/gigachat_tools.py
--rw-r--r--   0        0        0      528 2023-12-18 12:05:46.881864 gigachain-0.1.9/langchain/agents/format_scratchpad/log.py
--rw-r--r--   0        0        0      721 2023-12-18 12:05:46.882588 gigachain-0.1.9/langchain/agents/format_scratchpad/log_to_messages.py
--rw-r--r--   0        0        0     2203 2023-12-18 12:05:46.883234 gigachain-0.1.9/langchain/agents/format_scratchpad/openai_functions.py
--rw-r--r--   0        0        0     1885 2024-01-10 09:04:40.320052 gigachain-0.1.9/langchain/agents/format_scratchpad/openai_tools.py
--rw-r--r--   0        0        0      578 2023-12-18 12:05:46.884524 gigachain-0.1.9/langchain/agents/format_scratchpad/xml.py
--rw-r--r--   0        0        0        0 2024-02-22 08:54:03.093863 gigachain-0.1.9/langchain/agents/gigachat_functions_agent/__init__.py
--rw-r--r--   0        0        0     2567 2024-02-22 08:54:03.094866 gigachain-0.1.9/langchain/agents/gigachat_functions_agent/agent_token_buffer_memory.py
--rw-r--r--   0        0        0     4183 2024-02-22 08:54:03.097385 gigachain-0.1.9/langchain/agents/gigachat_functions_agent/base.py
--rw-r--r--   0        0        0        0 2024-02-22 08:54:03.097626 gigachain-0.1.9/langchain/agents/gigachat_tools/__init__.py
--rw-r--r--   0        0        0     3243 2024-02-22 08:54:03.099768 gigachain-0.1.9/langchain/agents/gigachat_tools/base.py
--rw-r--r--   0        0        0     3244 2024-02-22 08:54:03.100651 gigachain-0.1.9/langchain/agents/initialize.py
--rw-r--r--   0        0        0        0 2024-01-18 15:16:40.615878 gigachain-0.1.9/langchain/agents/json_chat/__init__.py
--rw-r--r--   0        0        0     6832 2024-02-22 08:54:03.101790 gigachain-0.1.9/langchain/agents/json_chat/base.py
--rw-r--r--   0        0        0      551 2024-01-18 15:16:40.617394 gigachain-0.1.9/langchain/agents/json_chat/prompt.py
--rw-r--r--   0        0        0    23975 2024-03-01 11:50:11.615565 gigachain-0.1.9/langchain/agents/load_tools.py
--rw-r--r--   0        0        0     4629 2024-02-22 08:54:03.106160 gigachain-0.1.9/langchain/agents/loading.py
--rw-r--r--   0        0        0       86 2023-08-21 13:51:28.555248 gigachain-0.1.9/langchain/agents/mrkl/__init__.py
--rw-r--r--   0        0        0     6046 2024-02-22 08:54:03.107273 gigachain-0.1.9/langchain/agents/mrkl/base.py
--rw-r--r--   0        0        0     3407 2024-02-22 08:54:03.108171 gigachain-0.1.9/langchain/agents/mrkl/output_parser.py
--rw-r--r--   0        0        0     1602 2023-12-18 12:05:46.889787 gigachain-0.1.9/langchain/agents/mrkl/prompt.py
--rw-r--r--   0        0        0      114 2023-12-18 12:05:46.890436 gigachain-0.1.9/langchain/agents/openai_assistant/__init__.py
--rw-r--r--   0        0        0    25732 2024-02-22 08:54:03.113714 gigachain-0.1.9/langchain/agents/openai_assistant/base.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.556082 gigachain-0.1.9/langchain/agents/openai_functions_agent/__init__.py
--rw-r--r--   0        0        0     2567 2023-12-18 12:05:46.893881 gigachain-0.1.9/langchain/agents/openai_functions_agent/agent_token_buffer_memory.py
--rw-r--r--   0        0        0    11522 2024-02-22 08:54:03.115573 gigachain-0.1.9/langchain/agents/openai_functions_agent/base.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.556705 gigachain-0.1.9/langchain/agents/openai_functions_multi_agent/__init__.py
--rw-r--r--   0        0        0    11944 2024-02-22 08:54:03.117313 gigachain-0.1.9/langchain/agents/openai_functions_multi_agent/base.py
--rw-r--r--   0        0        0        0 2024-01-18 15:16:40.628412 gigachain-0.1.9/langchain/agents/openai_tools/__init__.py
--rw-r--r--   0        0        0     3388 2024-02-22 08:54:03.118744 gigachain-0.1.9/langchain/agents/openai_tools/base.py
--rw-r--r--   0        0        0     1419 2024-02-22 08:54:03.121605 gigachain-0.1.9/langchain/agents/output_parsers/__init__.py
--rw-r--r--   0        0        0     3210 2024-02-22 08:54:03.124433 gigachain-0.1.9/langchain/agents/output_parsers/gigachat_functions.py
--rw-r--r--   0        0        0     1846 2024-02-22 08:54:03.125684 gigachain-0.1.9/langchain/agents/output_parsers/json.py
--rw-r--r--   0        0        0     3467 2024-01-18 15:16:40.630141 gigachain-0.1.9/langchain/agents/output_parsers/openai_functions.py
--rw-r--r--   0        0        0     3492 2024-01-18 15:16:40.631038 gigachain-0.1.9/langchain/agents/output_parsers/openai_tools.py
--rw-r--r--   0        0        0     2455 2024-02-22 08:54:03.126947 gigachain-0.1.9/langchain/agents/output_parsers/react_json_single_input.py
--rw-r--r--   0        0        0     3218 2023-12-18 12:05:46.905924 gigachain-0.1.9/langchain/agents/output_parsers/react_single_input.py
--rw-r--r--   0        0        0     1545 2023-12-18 12:05:46.906825 gigachain-0.1.9/langchain/agents/output_parsers/self_ask.py
--rw-r--r--   0        0        0     1658 2023-12-18 12:05:46.907986 gigachain-0.1.9/langchain/agents/output_parsers/xml.py
--rw-r--r--   0        0        0       76 2023-08-21 13:51:28.557154 gigachain-0.1.9/langchain/agents/react/__init__.py
--rw-r--r--   0        0        0     3903 2024-02-22 08:54:03.128763 gigachain-0.1.9/langchain/agents/react/agent.py
--rw-r--r--   0        0        0     5714 2024-02-22 08:54:03.130890 gigachain-0.1.9/langchain/agents/react/base.py
--rw-r--r--   0        0        0     1231 2023-12-18 12:05:46.909814 gigachain-0.1.9/langchain/agents/react/output_parser.py
--rw-r--r--   0        0        0     3005 2023-12-18 12:05:46.910755 gigachain-0.1.9/langchain/agents/react/textworld_prompt.py
--rw-r--r--   0        0        0    10562 2023-12-18 12:05:46.911736 gigachain-0.1.9/langchain/agents/react/wiki_prompt.py
--rw-r--r--   0        0        0     1175 2023-12-18 12:05:46.912970 gigachain-0.1.9/langchain/agents/schema.py
--rw-r--r--   0        0        0      106 2023-08-21 13:51:28.559443 gigachain-0.1.9/langchain/agents/self_ask_with_search/__init__.py
--rw-r--r--   0        0        0     8175 2024-02-22 08:54:03.134843 gigachain-0.1.9/langchain/agents/self_ask_with_search/base.py
--rw-r--r--   0        0        0      138 2023-09-25 07:40:35.498979 gigachain-0.1.9/langchain/agents/self_ask_with_search/output_parser.py
--rw-r--r--   0        0        0     3502 2023-12-18 12:05:46.916766 gigachain-0.1.9/langchain/agents/self_ask_with_search/prompt.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.560593 gigachain-0.1.9/langchain/agents/structured_chat/__init__.py
--rw-r--r--   0        0        0     9948 2024-02-22 08:54:03.135995 gigachain-0.1.9/langchain/agents/structured_chat/base.py
--rw-r--r--   0        0        0     3799 2024-02-22 08:54:03.137224 gigachain-0.1.9/langchain/agents/structured_chat/output_parser.py
--rw-r--r--   0        0        0     1663 2023-09-07 06:38:18.010991 gigachain-0.1.9/langchain/agents/structured_chat/prompt.py
--rw-r--r--   0        0        0     1409 2024-02-22 08:54:03.138801 gigachain-0.1.9/langchain/agents/tools.py
--rw-r--r--   0        0        0     1475 2024-01-29 08:25:46.514870 gigachain-0.1.9/langchain/agents/types.py
--rw-r--r--   0        0        0      384 2023-12-18 12:05:46.920460 gigachain-0.1.9/langchain/agents/utils.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.562209 gigachain-0.1.9/langchain/agents/xml/__init__.py
--rw-r--r--   0        0        0     7258 2024-02-22 08:54:03.140006 gigachain-0.1.9/langchain/agents/xml/base.py
--rw-r--r--   0        0        0      767 2024-01-18 15:16:40.638769 gigachain-0.1.9/langchain/agents/xml/prompt.py
--rw-r--r--   0        0        0      217 2023-12-18 12:05:46.922138 gigachain-0.1.9/langchain/base_language.py
--rw-r--r--   0        0        0      701 2024-01-10 09:04:40.325005 gigachain-0.1.9/langchain/cache.py
--rw-r--r--   0        0        0     2509 2024-02-22 08:54:03.143127 gigachain-0.1.9/langchain/callbacks/__init__.py
--rw-r--r--   0        0        0      211 2023-12-18 12:05:46.925154 gigachain-0.1.9/langchain/callbacks/aim_callback.py
--rw-r--r--   0        0        0      120 2023-12-18 12:05:46.925829 gigachain-0.1.9/langchain/callbacks/argilla_callback.py
--rw-r--r--   0        0        0      114 2023-12-18 12:05:46.926936 gigachain-0.1.9/langchain/callbacks/arize_callback.py
--rw-r--r--   0        0        0      133 2024-01-10 09:04:40.325707 gigachain-0.1.9/langchain/callbacks/arthur_callback.py
--rw-r--r--   0        0        0      653 2024-02-22 08:54:03.144267 gigachain-0.1.9/langchain/callbacks/base.py
--rw-r--r--   0        0        0      129 2024-01-10 09:04:40.326482 gigachain-0.1.9/langchain/callbacks/clearml_callback.py
--rw-r--r--   0        0        0      133 2024-01-10 09:04:40.327283 gigachain-0.1.9/langchain/callbacks/comet_ml_callback.py
--rw-r--r--   0        0        0      124 2023-12-18 12:05:46.931986 gigachain-0.1.9/langchain/callbacks/confident_callback.py
--rw-r--r--   0        0        0      129 2024-01-10 09:04:40.328061 gigachain-0.1.9/langchain/callbacks/context_callback.py
--rw-r--r--   0        0        0     2589 2024-02-22 08:54:03.145615 gigachain-0.1.9/langchain/callbacks/file.py
--rw-r--r--   0        0        0      123 2024-01-10 09:04:40.328815 gigachain-0.1.9/langchain/callbacks/flyte_callback.py
--rw-r--r--   0        0        0      275 2024-01-10 09:04:40.329559 gigachain-0.1.9/langchain/callbacks/human.py
--rw-r--r--   0        0        0      133 2024-01-10 09:04:40.330500 gigachain-0.1.9/langchain/callbacks/infino_callback.py
--rw-r--r--   0        0        0      241 2023-12-18 12:05:46.936755 gigachain-0.1.9/langchain/callbacks/labelstudio_callback.py
--rw-r--r--   0        0        0      142 2024-01-10 09:04:40.331568 gigachain-0.1.9/langchain/callbacks/llmonitor_callback.py
--rw-r--r--   0        0        0     1777 2023-12-18 12:05:46.938871 gigachain-0.1.9/langchain/callbacks/manager.py
--rw-r--r--   0        0        0      305 2024-01-10 09:04:40.332484 gigachain-0.1.9/langchain/callbacks/mlflow_callback.py
--rw-r--r--   0        0        0      113 2024-01-10 09:04:40.333267 gigachain-0.1.9/langchain/callbacks/openai_info.py
--rw-r--r--   0        0        0      141 2024-01-10 09:04:40.333971 gigachain-0.1.9/langchain/callbacks/promptlayer_callback.py
--rw-r--r--   0        0        0      135 2024-01-10 09:04:40.334649 gigachain-0.1.9/langchain/callbacks/sagemaker_callback.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:46.944007 gigachain-0.1.9/langchain/callbacks/stdout.py
--rw-r--r--   0        0        0     2399 2024-02-22 08:54:03.146818 gigachain-0.1.9/langchain/callbacks/streaming_aiter.py
--rw-r--r--   0        0        0     3371 2023-12-18 12:05:46.945805 gigachain-0.1.9/langchain/callbacks/streaming_aiter_final_only.py
--rw-r--r--   0        0        0      173 2024-02-22 08:54:03.147647 gigachain-0.1.9/langchain/callbacks/streaming_stdout.py
--rw-r--r--   0        0        0     3357 2024-02-22 08:54:03.148511 gigachain-0.1.9/langchain/callbacks/streaming_stdout_final_only.py
--rw-r--r--   0        0        0     3190 2023-10-03 07:51:15.793630 gigachain-0.1.9/langchain/callbacks/streamlit/__init__.py
--rw-r--r--   0        0        0      185 2023-12-18 12:05:46.947518 gigachain-0.1.9/langchain/callbacks/streamlit/mutable_expander.py
--rw-r--r--   0        0        0      490 2024-01-10 09:04:40.335344 gigachain-0.1.9/langchain/callbacks/streamlit/streamlit_callback_handler.py
--rw-r--r--   0        0        0      589 2023-12-18 12:05:46.949215 gigachain-0.1.9/langchain/callbacks/tracers/__init__.py
--rw-r--r--   0        0        0      154 2023-12-18 12:05:46.950003 gigachain-0.1.9/langchain/callbacks/tracers/base.py
--rw-r--r--   0        0        0      154 2024-01-10 09:04:40.336248 gigachain-0.1.9/langchain/callbacks/tracers/comet.py
--rw-r--r--   0        0        0      233 2023-12-18 12:05:46.951869 gigachain-0.1.9/langchain/callbacks/tracers/evaluation.py
--rw-r--r--   0        0        0      218 2023-12-18 12:05:46.952818 gigachain-0.1.9/langchain/callbacks/tracers/langchain.py
--rw-r--r--   0        0        0       99 2023-12-18 12:05:46.953574 gigachain-0.1.9/langchain/callbacks/tracers/langchain_v1.py
--rw-r--r--   0        0        0      226 2023-12-18 12:05:46.954653 gigachain-0.1.9/langchain/callbacks/tracers/log_stream.py
--rw-r--r--   0        0        0     1384 2023-12-18 12:05:46.955043 gigachain-0.1.9/langchain/callbacks/tracers/logging.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:46.955825 gigachain-0.1.9/langchain/callbacks/tracers/root_listeners.py
--rw-r--r--   0        0        0      120 2023-12-18 12:05:46.956667 gigachain-0.1.9/langchain/callbacks/tracers/run_collector.py
--rw-r--r--   0        0        0      470 2023-12-18 12:05:46.957919 gigachain-0.1.9/langchain/callbacks/tracers/schemas.py
--rw-r--r--   0        0        0      168 2023-12-18 12:05:46.958747 gigachain-0.1.9/langchain/callbacks/tracers/stdout.py
--rw-r--r--   0        0        0      229 2024-01-10 09:04:40.336940 gigachain-0.1.9/langchain/callbacks/tracers/wandb.py
--rw-r--r--   0        0        0      132 2024-01-10 09:04:40.337840 gigachain-0.1.9/langchain/callbacks/trubrics_callback.py
--rw-r--r--   0        0        0      403 2023-12-18 12:05:46.961334 gigachain-0.1.9/langchain/callbacks/utils.py
--rw-r--r--   0        0        0      130 2024-01-10 09:04:40.338883 gigachain-0.1.9/langchain/callbacks/wandb_callback.py
--rw-r--r--   0        0        0      129 2024-01-10 09:04:40.339806 gigachain-0.1.9/langchain/callbacks/whylabs_callback.py
--rw-r--r--   0        0        0     5951 2024-02-22 08:54:03.149844 gigachain-0.1.9/langchain/chains/__init__.py
--rw-r--r--   0        0        0       84 2023-08-21 13:51:28.576965 gigachain-0.1.9/langchain/chains/api/__init__.py
--rw-r--r--   0        0        0     8919 2024-02-22 08:54:03.151385 gigachain-0.1.9/langchain/chains/api/base.py
--rw-r--r--   0        0        0     2452 2024-01-10 09:04:40.341669 gigachain-0.1.9/langchain/chains/api/news_docs.py
--rw-r--r--   0        0        0     3399 2023-08-21 13:51:28.578041 gigachain-0.1.9/langchain/chains/api/open_meteo_docs.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.578278 gigachain-0.1.9/langchain/chains/api/openapi/__init__.py
--rw-r--r--   0        0        0     8786 2024-02-22 08:54:03.152480 gigachain-0.1.9/langchain/chains/api/openapi/chain.py
--rw-r--r--   0        0        0     1791 2023-08-21 13:51:28.579000 gigachain-0.1.9/langchain/chains/api/openapi/prompts.py
--rw-r--r--   0        0        0     2025 2023-12-18 12:05:46.968380 gigachain-0.1.9/langchain/chains/api/openapi/requests_chain.py
--rw-r--r--   0        0        0     1847 2023-12-18 12:05:46.969509 gigachain-0.1.9/langchain/chains/api/openapi/response_chain.py
--rw-r--r--   0        0        0     1920 2023-08-21 13:51:28.580702 gigachain-0.1.9/langchain/chains/api/podcast_docs.py
--rw-r--r--   0        0        0     1326 2023-12-18 12:05:46.970482 gigachain-0.1.9/langchain/chains/api/prompt.py
--rw-r--r--   0        0        0     1537 2023-08-21 13:51:28.581731 gigachain-0.1.9/langchain/chains/api/tmdb_docs.py
--rw-r--r--   0        0        0    28487 2024-03-01 11:50:11.617337 gigachain-0.1.9/langchain/chains/base.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.582802 gigachain-0.1.9/langchain/chains/chat_vector_db/__init__.py
--rw-r--r--   0        0        0     1037 2023-12-18 12:05:46.972569 gigachain-0.1.9/langchain/chains/chat_vector_db/prompts.py
--rw-r--r--   0        0        0      367 2024-01-10 09:04:40.342648 gigachain-0.1.9/langchain/chains/combine_documents/__init__.py
--rw-r--r--   0        0        0     8094 2024-03-01 11:50:11.618347 gigachain-0.1.9/langchain/chains/combine_documents/base.py
--rw-r--r--   0        0        0     1743 2023-11-15 10:30:09.330835 gigachain-0.1.9/langchain/chains/combine_documents/conditional.py
--rw-r--r--   0        0        0    11781 2024-03-01 11:50:11.619466 gigachain-0.1.9/langchain/chains/combine_documents/map_reduce.py
--rw-r--r--   0        0        0     8991 2024-03-01 11:50:11.620114 gigachain-0.1.9/langchain/chains/combine_documents/map_rerank.py
--rw-r--r--   0        0        0    13894 2024-02-22 08:54:03.165440 gigachain-0.1.9/langchain/chains/combine_documents/reduce.py
--rw-r--r--   0        0        0     9113 2024-02-22 08:54:03.166781 gigachain-0.1.9/langchain/chains/combine_documents/refine.py
--rw-r--r--   0        0        0    11030 2024-02-22 08:54:03.169663 gigachain-0.1.9/langchain/chains/combine_documents/stuff.py
--rw-r--r--   0        0        0      107 2023-08-21 13:51:28.587546 gigachain-0.1.9/langchain/chains/constitutional_ai/__init__.py
--rw-r--r--   0        0        0     6341 2024-02-22 08:54:03.170812 gigachain-0.1.9/langchain/chains/constitutional_ai/base.py
--rw-r--r--   0        0        0      283 2023-12-18 12:05:46.981590 gigachain-0.1.9/langchain/chains/constitutional_ai/models.py
--rw-r--r--   0        0        0    21738 2023-08-21 13:51:28.588681 gigachain-0.1.9/langchain/chains/constitutional_ai/principles.py
--rw-r--r--   0        0        0    14534 2023-12-18 12:05:46.982679 gigachain-0.1.9/langchain/chains/constitutional_ai/prompts.py
--rw-r--r--   0        0        0       71 2023-08-21 13:51:28.589976 gigachain-0.1.9/langchain/chains/conversation/__init__.py
--rw-r--r--   0        0        0     2366 2024-01-18 15:16:40.657291 gigachain-0.1.9/langchain/chains/conversation/base.py
--rw-r--r--   0        0        0      856 2023-08-21 13:51:28.590517 gigachain-0.1.9/langchain/chains/conversation/memory.py
--rw-r--r--   0        0        0     1063 2023-12-18 12:05:46.984228 gigachain-0.1.9/langchain/chains/conversation/prompt.py
--rw-r--r--   0        0        0       49 2023-08-21 13:51:28.591153 gigachain-0.1.9/langchain/chains/conversational_retrieval/__init__.py
--rw-r--r--   0        0        0    18065 2024-02-22 08:54:03.173623 gigachain-0.1.9/langchain/chains/conversational_retrieval/base.py
--rw-r--r--   0        0        0     1037 2023-12-18 12:05:46.988192 gigachain-0.1.9/langchain/chains/conversational_retrieval/prompts.py
--rw-r--r--   0        0        0      126 2023-08-21 13:51:28.592942 gigachain-0.1.9/langchain/chains/elasticsearch_database/__init__.py
--rw-r--r--   0        0        0     8287 2024-02-22 08:54:03.175145 gigachain-0.1.9/langchain/chains/elasticsearch_database/base.py
--rw-r--r--   0        0        0     2480 2023-12-18 12:05:46.989727 gigachain-0.1.9/langchain/chains/elasticsearch_database/prompts.py
--rw-r--r--   0        0        0      669 2023-10-30 16:05:53.857849 gigachain-0.1.9/langchain/chains/encoder.py
--rw-r--r--   0        0        0      465 2023-12-18 12:05:46.990078 gigachain-0.1.9/langchain/chains/ernie_functions/__init__.py
--rw-r--r--   0        0        0    23205 2024-03-01 11:50:11.621045 gigachain-0.1.9/langchain/chains/ernie_functions/base.py
--rw-r--r--   0        0        0      741 2023-12-18 12:05:46.991949 gigachain-0.1.9/langchain/chains/example_generator.py
--rw-r--r--   0        0        0       51 2023-08-21 13:51:28.594704 gigachain-0.1.9/langchain/chains/flare/__init__.py
--rw-r--r--   0        0        0     9033 2024-02-22 08:54:03.177642 gigachain-0.1.9/langchain/chains/flare/base.py
--rw-r--r--   0        0        0     1949 2023-12-18 12:05:46.993539 gigachain-0.1.9/langchain/chains/flare/prompts.py
--rw-r--r--   0        0        0       49 2023-08-21 13:51:28.596462 gigachain-0.1.9/langchain/chains/graph_qa/__init__.py
--rw-r--r--   0        0        0     8397 2024-02-22 08:54:03.178971 gigachain-0.1.9/langchain/chains/graph_qa/arangodb.py
--rw-r--r--   0        0        0     3671 2024-01-18 15:16:40.667708 gigachain-0.1.9/langchain/chains/graph_qa/base.py
--rw-r--r--   0        0        0    10452 2024-02-22 08:54:03.179960 gigachain-0.1.9/langchain/chains/graph_qa/cypher.py
--rw-r--r--   0        0        0     9625 2023-12-18 12:05:46.997918 gigachain-0.1.9/langchain/chains/graph_qa/cypher_utils.py
--rw-r--r--   0        0        0     5272 2024-02-22 08:54:03.180901 gigachain-0.1.9/langchain/chains/graph_qa/falkordb.py
--rw-r--r--   0        0        0     3717 2024-02-22 08:54:03.182056 gigachain-0.1.9/langchain/chains/graph_qa/hugegraph.py
--rw-r--r--   0        0        0     3698 2024-02-22 08:54:03.182898 gigachain-0.1.9/langchain/chains/graph_qa/kuzu.py
--rw-r--r--   0        0        0     3692 2024-02-22 08:54:03.183710 gigachain-0.1.9/langchain/chains/graph_qa/nebulagraph.py
--rw-r--r--   0        0        0     6890 2024-02-22 08:54:03.184676 gigachain-0.1.9/langchain/chains/graph_qa/neptune_cypher.py
--rw-r--r--   0        0        0     6610 2024-02-22 08:54:03.185246 gigachain-0.1.9/langchain/chains/graph_qa/neptune_sparql.py
--rw-r--r--   0        0        0     7226 2024-02-22 08:54:03.185912 gigachain-0.1.9/langchain/chains/graph_qa/ontotext_graphdb.py
--rw-r--r--   0        0        0    25955 2024-02-22 08:54:03.189550 gigachain-0.1.9/langchain/chains/graph_qa/prompts.py
--rw-r--r--   0        0        0     5838 2024-03-01 11:50:11.621545 gigachain-0.1.9/langchain/chains/graph_qa/sparql.py
--rw-r--r--   0        0        0     2662 2024-01-10 09:04:40.353033 gigachain-0.1.9/langchain/chains/history_aware_retriever.py
--rw-r--r--   0        0        0       75 2023-08-21 13:51:28.600763 gigachain-0.1.9/langchain/chains/hyde/__init__.py
--rw-r--r--   0        0        0     3341 2024-02-22 08:54:03.191623 gigachain-0.1.9/langchain/chains/hyde/base.py
--rw-r--r--   0        0        0     2482 2023-12-18 12:05:47.005583 gigachain-0.1.9/langchain/chains/hyde/prompts.py
--rw-r--r--   0        0        0    15030 2024-02-22 08:54:03.195047 gigachain-0.1.9/langchain/chains/llm.py
--rw-r--r--   0        0        0      450 2024-02-22 08:54:03.198689 gigachain-0.1.9/langchain/chains/llm_bash/__init__.py
--rw-r--r--   0        0        0      139 2023-08-21 13:51:28.604012 gigachain-0.1.9/langchain/chains/llm_checker/__init__.py
--rw-r--r--   0        0        0     6164 2024-02-22 08:54:03.200128 gigachain-0.1.9/langchain/chains/llm_checker/base.py
--rw-r--r--   0        0        0     1341 2023-12-18 12:05:47.009556 gigachain-0.1.9/langchain/chains/llm_checker/prompt.py
--rw-r--r--   0        0        0      143 2023-08-21 13:51:28.605454 gigachain-0.1.9/langchain/chains/llm_math/__init__.py
--rw-r--r--   0        0        0     6723 2024-02-22 08:54:03.201078 gigachain-0.1.9/langchain/chains/llm_math/base.py
--rw-r--r--   0        0        0     1158 2023-12-18 12:05:47.012133 gigachain-0.1.9/langchain/chains/llm_math/prompt.py
--rw-r--r--   0        0        0     3193 2024-02-22 08:54:03.201902 gigachain-0.1.9/langchain/chains/llm_requests.py
--rw-r--r--   0        0        0      352 2023-08-21 13:51:28.607135 gigachain-0.1.9/langchain/chains/llm_summarization_checker/__init__.py
--rw-r--r--   0        0        0     6582 2024-02-22 08:54:03.202882 gigachain-0.1.9/langchain/chains/llm_summarization_checker/base.py
--rw-r--r--   0        0        0     1143 2023-08-22 11:25:59.886227 gigachain-0.1.9/langchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt
--rw-r--r--   0        0        0      696 2023-08-22 11:25:59.887142 gigachain-0.1.9/langchain/chains/llm_summarization_checker/prompts/check_facts.txt
--rw-r--r--   0        0        0      234 2023-08-22 11:25:59.887992 gigachain-0.1.9/langchain/chains/llm_summarization_checker/prompts/create_facts.txt
--rw-r--r--   0        0        0      834 2023-08-22 11:25:59.888905 gigachain-0.1.9/langchain/chains/llm_summarization_checker/prompts/revise_summary.txt
--rw-r--r--   0        0        0      467 2024-02-22 08:54:03.205485 gigachain-0.1.9/langchain/chains/llm_symbolic_math/__init__.py
--rw-r--r--   0        0        0    25297 2024-02-22 08:54:03.209215 gigachain-0.1.9/langchain/chains/loading.py
--rw-r--r--   0        0        0     3732 2024-02-22 08:54:03.210816 gigachain-0.1.9/langchain/chains/mapreduce.py
--rw-r--r--   0        0        0     3086 2024-02-22 08:54:03.212255 gigachain-0.1.9/langchain/chains/moderation.py
--rw-r--r--   0        0        0       96 2023-08-21 13:51:28.612079 gigachain-0.1.9/langchain/chains/natbot/__init__.py
--rw-r--r--   0        0        0     4695 2024-02-22 08:54:03.213323 gigachain-0.1.9/langchain/chains/natbot/base.py
--rw-r--r--   0        0        0    16050 2024-02-22 08:54:03.214508 gigachain-0.1.9/langchain/chains/natbot/crawler.py
--rw-r--r--   0        0        0     6769 2023-12-18 12:05:47.020892 gigachain-0.1.9/langchain/chains/natbot/prompt.py
--rw-r--r--   0        0        0     1357 2024-02-22 08:54:03.215313 gigachain-0.1.9/langchain/chains/openai_functions/__init__.py
--rw-r--r--   0        0        0    10080 2024-03-01 11:50:11.622695 gigachain-0.1.9/langchain/chains/openai_functions/base.py
--rw-r--r--   0        0        0     3522 2024-03-01 11:50:11.624093 gigachain-0.1.9/langchain/chains/openai_functions/citation_fuzzy_match.py
--rw-r--r--   0        0        0     4298 2024-03-01 11:50:11.625958 gigachain-0.1.9/langchain/chains/openai_functions/extraction.py
--rw-r--r--   0        0        0    11311 2024-03-01 11:50:11.627637 gigachain-0.1.9/langchain/chains/openai_functions/openapi.py
--rw-r--r--   0        0        0     3923 2024-03-01 11:50:11.628248 gigachain-0.1.9/langchain/chains/openai_functions/qa_with_structure.py
--rw-r--r--   0        0        0     2665 2024-03-01 11:50:11.628741 gigachain-0.1.9/langchain/chains/openai_functions/tagging.py
--rw-r--r--   0        0        0     1257 2023-08-21 13:51:28.616551 gigachain-0.1.9/langchain/chains/openai_functions/utils.py
--rw-r--r--   0        0        0      134 2023-11-10 13:07:50.024454 gigachain-0.1.9/langchain/chains/openai_tools/__init__.py
--rw-r--r--   0        0        0     1665 2024-02-22 08:54:03.220719 gigachain-0.1.9/langchain/chains/openai_tools/extraction.py
--rw-r--r--   0        0        0     2015 2023-12-18 12:05:47.029972 gigachain-0.1.9/langchain/chains/prompt_selector.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.617097 gigachain-0.1.9/langchain/chains/qa_generation/__init__.py
--rw-r--r--   0        0        0     2464 2024-02-22 08:54:03.221867 gigachain-0.1.9/langchain/chains/qa_generation/base.py
--rw-r--r--   0        0        0     2657 2023-12-18 12:05:47.032423 gigachain-0.1.9/langchain/chains/qa_generation/prompt.py
--rw-r--r--   0        0        0      173 2023-08-21 13:51:28.619059 gigachain-0.1.9/langchain/chains/qa_with_sources/__init__.py
--rw-r--r--   0        0        0     7976 2024-02-22 08:54:03.223422 gigachain-0.1.9/langchain/chains/qa_with_sources/base.py
--rw-r--r--   0        0        0     6793 2023-12-18 12:05:47.034152 gigachain-0.1.9/langchain/chains/qa_with_sources/loading.py
--rw-r--r--   0        0        0     4144 2023-12-18 12:05:47.035020 gigachain-0.1.9/langchain/chains/qa_with_sources/map_reduce_prompt.py
--rw-r--r--   0        0        0     1764 2023-12-18 12:05:47.035786 gigachain-0.1.9/langchain/chains/qa_with_sources/refine_prompts.py
--rw-r--r--   0        0        0     2459 2024-02-22 08:54:03.224282 gigachain-0.1.9/langchain/chains/qa_with_sources/retrieval.py
--rw-r--r--   0        0        0     3471 2023-12-18 12:05:47.037437 gigachain-0.1.9/langchain/chains/qa_with_sources/stuff_prompt.py
--rw-r--r--   0        0        0     2770 2024-02-22 08:54:03.225130 gigachain-0.1.9/langchain/chains/qa_with_sources/vector_db.py
--rw-r--r--   0        0        0      131 2024-02-22 08:54:03.225931 gigachain-0.1.9/langchain/chains/query_constructor/__init__.py
--rw-r--r--   0        0        0    13721 2024-02-22 08:54:03.230318 gigachain-0.1.9/langchain/chains/query_constructor/base.py
--rw-r--r--   0        0        0     3191 2023-12-18 12:05:47.039898 gigachain-0.1.9/langchain/chains/query_constructor/ir.py
--rw-r--r--   0        0        0     5707 2023-12-18 12:05:47.040791 gigachain-0.1.9/langchain/chains/query_constructor/parser.py
--rw-r--r--   0        0        0    10146 2023-12-18 12:05:47.041579 gigachain-0.1.9/langchain/chains/query_constructor/prompt.py
--rw-r--r--   0        0        0      321 2023-12-18 12:05:47.042242 gigachain-0.1.9/langchain/chains/query_constructor/schema.py
--rw-r--r--   0        0        0     8503 2024-02-22 08:54:03.231561 gigachain-0.1.9/langchain/chains/question_answering/__init__.py
--rw-r--r--   0        0        0     5425 2023-12-18 12:05:47.043620 gigachain-0.1.9/langchain/chains/question_answering/map_reduce_prompt.py
--rw-r--r--   0        0        0     2477 2023-12-18 12:05:47.044547 gigachain-0.1.9/langchain/chains/question_answering/map_rerank_prompt.py
--rw-r--r--   0        0        0     3133 2023-12-18 12:05:47.045293 gigachain-0.1.9/langchain/chains/question_answering/refine_prompts.py
--rw-r--r--   0        0        0     1404 2023-12-18 12:05:47.046327 gigachain-0.1.9/langchain/chains/question_answering/stuff_prompt.py
--rw-r--r--   0        0        0     2742 2024-01-18 15:16:40.690412 gigachain-0.1.9/langchain/chains/retrieval.py
--rw-r--r--   0        0        0       62 2023-08-21 13:51:28.631121 gigachain-0.1.9/langchain/chains/retrieval_qa/__init__.py
--rw-r--r--   0        0        0     9952 2024-02-22 08:54:03.232560 gigachain-0.1.9/langchain/chains/retrieval_qa/base.py
--rw-r--r--   0        0        0      527 2023-12-18 12:05:47.048474 gigachain-0.1.9/langchain/chains/retrieval_qa/prompt.py
--rw-r--r--   0        0        0      407 2023-08-21 13:51:28.632647 gigachain-0.1.9/langchain/chains/router/__init__.py
--rw-r--r--   0        0        0     4571 2024-02-22 08:54:03.234029 gigachain-0.1.9/langchain/chains/router/base.py
--rw-r--r--   0        0        0     1982 2024-02-22 08:54:03.234826 gigachain-0.1.9/langchain/chains/router/embedding_router.py
--rw-r--r--   0        0        0     4283 2024-02-22 08:54:03.235785 gigachain-0.1.9/langchain/chains/router/llm_router.py
--rw-r--r--   0        0        0     2245 2023-12-18 12:05:47.052334 gigachain-0.1.9/langchain/chains/router/multi_prompt.py
--rw-r--r--   0        0        0     1849 2023-09-04 05:57:22.503454 gigachain-0.1.9/langchain/chains/router/multi_prompt_prompt.py
--rw-r--r--   0        0        0     1904 2023-08-21 14:03:46.158141 gigachain-0.1.9/langchain/chains/router/multi_retrieval_prompt.py
--rw-r--r--   0        0        0     3659 2024-01-18 15:16:40.692341 gigachain-0.1.9/langchain/chains/router/multi_retrieval_qa.py
--rw-r--r--   0        0        0     7510 2024-02-22 08:54:03.236797 gigachain-0.1.9/langchain/chains/sequential.py
--rw-r--r--   0        0        0       47 2023-08-21 13:51:28.636997 gigachain-0.1.9/langchain/chains/sql_database/__init__.py
--rw-r--r--   0        0        0    30619 2024-02-22 08:54:03.240301 gigachain-0.1.9/langchain/chains/sql_database/prompt.py
--rw-r--r--   0        0        0     5293 2024-02-22 08:54:03.241443 gigachain-0.1.9/langchain/chains/sql_database/query.py
--rw-r--r--   0        0        0      204 2024-02-22 08:54:03.242140 gigachain-0.1.9/langchain/chains/structured_output/__init__.py
--rw-r--r--   0        0        0    22268 2024-03-01 11:50:11.629251 gigachain-0.1.9/langchain/chains/structured_output/base.py
--rw-r--r--   0        0        0     6711 2024-02-22 08:54:03.246577 gigachain-0.1.9/langchain/chains/summarize/__init__.py
--rw-r--r--   0        0        0      271 2023-12-18 12:05:47.059118 gigachain-0.1.9/langchain/chains/summarize/map_reduce_prompt.py
--rw-r--r--   0        0        0     1138 2023-12-18 12:05:47.060439 gigachain-0.1.9/langchain/chains/summarize/refine_prompts.py
--rw-r--r--   0        0        0      271 2023-12-18 12:05:47.061163 gigachain-0.1.9/langchain/chains/summarize/stuff_prompt.py
--rw-r--r--   0        0        0     2369 2024-02-22 08:54:03.247840 gigachain-0.1.9/langchain/chains/transform.py
--rw-r--r--   0        0        0      452 2023-09-12 10:52:10.662329 gigachain-0.1.9/langchain/chat_loaders/__init__.py
--rw-r--r--   0        0        0       95 2023-12-18 12:05:47.064850 gigachain-0.1.9/langchain/chat_loaders/base.py
--rw-r--r--   0        0        0      240 2023-12-18 12:05:47.066006 gigachain-0.1.9/langchain/chat_loaders/facebook_messenger.py
--rw-r--r--   0        0        0       99 2024-01-10 09:04:40.356789 gigachain-0.1.9/langchain/chat_loaders/gmail.py
--rw-r--r--   0        0        0      107 2023-12-18 12:05:47.067658 gigachain-0.1.9/langchain/chat_loaders/imessage.py
--rw-r--r--   0        0        0      187 2023-12-18 12:05:47.068610 gigachain-0.1.9/langchain/chat_loaders/langsmith.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.069730 gigachain-0.1.9/langchain/chat_loaders/slack.py
--rw-r--r--   0        0        0      107 2023-12-18 12:05:47.070887 gigachain-0.1.9/langchain/chat_loaders/telegram.py
--rw-r--r--   0        0        0      290 2023-12-18 12:05:47.071655 gigachain-0.1.9/langchain/chat_loaders/utils.py
--rw-r--r--   0        0        0      107 2023-12-18 12:05:47.072872 gigachain-0.1.9/langchain/chat_loaders/whatsapp.py
--rw-r--r--   0        0        0     1995 2024-01-18 15:16:40.697309 gigachain-0.1.9/langchain/chat_models/__init__.py
--rw-r--r--   0        0        0      199 2024-01-10 09:04:40.357806 gigachain-0.1.9/langchain/chat_models/anthropic.py
--rw-r--r--   0        0        0      103 2024-01-10 09:04:40.358738 gigachain-0.1.9/langchain/chat_models/anyscale.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:47.078945 gigachain-0.1.9/langchain/chat_models/azure_openai.py
--rw-r--r--   0        0        0      189 2023-12-18 12:05:47.080365 gigachain-0.1.9/langchain/chat_models/azureml_endpoint.py
--rw-r--r--   0        0        0      110 2024-01-10 09:04:40.359766 gigachain-0.1.9/langchain/chat_models/baichuan.py
--rw-r--r--   0        0        0      131 2024-01-10 09:04:40.360897 gigachain-0.1.9/langchain/chat_models/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0      268 2024-01-10 09:04:40.361805 gigachain-0.1.9/langchain/chat_models/base.py
--rw-r--r--   0        0        0      131 2023-12-18 12:05:47.084089 gigachain-0.1.9/langchain/chat_models/bedrock.py
--rw-r--r--   0        0        0       97 2024-01-10 09:04:40.362621 gigachain-0.1.9/langchain/chat_models/cohere.py
--rw-r--r--   0        0        0      100 2023-12-18 12:05:47.085569 gigachain-0.1.9/langchain/chat_models/databricks.py
--rw-r--r--   0        0        0       91 2024-01-10 09:04:40.363366 gigachain-0.1.9/langchain/chat_models/ernie.py
--rw-r--r--   0        0        0      103 2024-01-10 09:04:40.364542 gigachain-0.1.9/langchain/chat_models/everlyai.py
--rw-r--r--   0        0        0      169 2023-12-18 12:05:47.088330 gigachain-0.1.9/langchain/chat_models/fake.py
--rw-r--r--   0        0        0      113 2024-01-10 09:04:40.365619 gigachain-0.1.9/langchain/chat_models/fireworks.py
--rw-r--r--   0        0        0       95 2024-01-10 09:04:40.366318 gigachain-0.1.9/langchain/chat_models/gigachat.py
--rw-r--r--   0        0        0      158 2024-01-10 09:04:40.367091 gigachain-0.1.9/langchain/chat_models/google_palm.py
--rw-r--r--   0        0        0      114 2024-01-10 09:04:40.367972 gigachain-0.1.9/langchain/chat_models/human.py
--rw-r--r--   0        0        0      107 2024-01-10 09:04:40.368737 gigachain-0.1.9/langchain/chat_models/hunyuan.py
--rw-r--r--   0        0        0      159 2024-01-10 09:04:40.369542 gigachain-0.1.9/langchain/chat_models/javelin_ai_gateway.py
--rw-r--r--   0        0        0      102 2024-01-10 09:04:40.370300 gigachain-0.1.9/langchain/chat_models/jinachat.py
--rw-r--r--   0        0        0       94 2024-01-10 09:04:40.371073 gigachain-0.1.9/langchain/chat_models/konko.py
--rw-r--r--   0        0        0      137 2024-01-10 09:04:40.371862 gigachain-0.1.9/langchain/chat_models/litellm.py
--rw-r--r--   0        0        0      139 2024-01-10 09:04:40.372837 gigachain-0.1.9/langchain/chat_models/meta.py
--rw-r--r--   0        0        0      100 2024-01-10 09:04:40.373952 gigachain-0.1.9/langchain/chat_models/minimax.py
--rw-r--r--   0        0        0       88 2023-12-18 12:05:47.098332 gigachain-0.1.9/langchain/chat_models/mlflow.py
--rw-r--r--   0        0        0      156 2024-01-10 09:04:40.375069 gigachain-0.1.9/langchain/chat_models/mlflow_ai_gateway.py
--rw-r--r--   0        0        0       97 2024-01-10 09:04:40.375700 gigachain-0.1.9/langchain/chat_models/ollama.py
--rw-r--r--   0        0        0      104 2024-01-10 09:04:40.377001 gigachain-0.1.9/langchain/chat_models/openai.py
--rw-r--r--   0        0        0      114 2023-12-18 12:05:47.102210 gigachain-0.1.9/langchain/chat_models/pai_eas_endpoint.py
--rw-r--r--   0        0        0      122 2023-12-18 12:05:47.103242 gigachain-0.1.9/langchain/chat_models/promptlayer_openai.py
--rw-r--r--   0        0        0      104 2024-01-10 09:04:40.377793 gigachain-0.1.9/langchain/chat_models/tongyi.py
--rw-r--r--   0        0        0      110 2024-01-10 09:04:40.378622 gigachain-0.1.9/langchain/chat_models/vertexai.py
--rw-r--r--   0        0        0      178 2024-01-10 09:04:40.379547 gigachain-0.1.9/langchain/chat_models/volcengine_maas.py
--rw-r--r--   0        0        0      103 2024-01-10 09:04:40.380328 gigachain-0.1.9/langchain/chat_models/yandex.py
--rw-r--r--   0        0        0     1184 2024-02-22 08:54:03.251031 gigachain-0.1.9/langchain/docstore/__init__.py
--rw-r--r--   0        0        0       91 2023-12-18 12:05:47.107159 gigachain-0.1.9/langchain/docstore/arbitrary_fn.py
--rw-r--r--   0        0        0      109 2023-12-18 12:05:47.107958 gigachain-0.1.9/langchain/docstore/base.py
--rw-r--r--   0        0        0       70 2023-12-18 12:05:47.108669 gigachain-0.1.9/langchain/docstore/document.py
--rw-r--r--   0        0        0      100 2023-12-18 12:05:47.109501 gigachain-0.1.9/langchain/docstore/in_memory.py
--rw-r--r--   0        0        0       86 2023-12-18 12:05:47.110273 gigachain-0.1.9/langchain/docstore/wikipedia.py
--rw-r--r--   0        0        0     5722 2024-02-22 08:54:03.254344 gigachain-0.1.9/langchain/document_loaders/__init__.py
--rw-r--r--   0        0        0       97 2023-12-18 12:05:47.112427 gigachain-0.1.9/langchain/document_loaders/acreom.py
--rw-r--r--   0        0        0      554 2023-12-18 12:05:47.113265 gigachain-0.1.9/langchain/document_loaders/airbyte.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.114177 gigachain-0.1.9/langchain/document_loaders/airbyte_json.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:47.115207 gigachain-0.1.9/langchain/document_loaders/airtable.py
--rw-r--r--   0        0        0      116 2023-12-18 12:05:47.116053 gigachain-0.1.9/langchain/document_loaders/apify_dataset.py
--rw-r--r--   0        0        0      113 2024-01-10 09:04:40.381440 gigachain-0.1.9/langchain/document_loaders/arcgis_loader.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.117596 gigachain-0.1.9/langchain/document_loaders/arxiv.py
--rw-r--r--   0        0        0      190 2023-12-18 12:05:47.118350 gigachain-0.1.9/langchain/document_loaders/assemblyai.py
--rw-r--r--   0        0        0      116 2024-01-10 09:04:40.382547 gigachain-0.1.9/langchain/document_loaders/async_html.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:47.120014 gigachain-0.1.9/langchain/document_loaders/azlyrics.py
--rw-r--r--   0        0        0      114 2023-12-18 12:05:47.120412 gigachain-0.1.9/langchain/document_loaders/azure_ai_data.py
--rw-r--r--   0        0        0      166 2023-12-18 12:05:47.121235 gigachain-0.1.9/langchain/document_loaders/azure_blob_storage_container.py
--rw-r--r--   0        0        0      151 2023-12-18 12:05:47.122051 gigachain-0.1.9/langchain/document_loaders/azure_blob_storage_file.py
--rw-r--r--   0        0        0      146 2023-12-18 12:05:47.122866 gigachain-0.1.9/langchain/document_loaders/baiducloud_bos_directory.py
--rw-r--r--   0        0        0      122 2023-12-18 12:05:47.123637 gigachain-0.1.9/langchain/document_loaders/baiducloud_bos_file.py
--rw-r--r--   0        0        0      125 2023-12-18 12:05:47.124374 gigachain-0.1.9/langchain/document_loaders/base.py
--rw-r--r--   0        0        0      120 2024-01-10 09:04:40.383758 gigachain-0.1.9/langchain/document_loaders/base_o365.py
--rw-r--r--   0        0        0       97 2023-12-18 12:05:47.125960 gigachain-0.1.9/langchain/document_loaders/bibtex.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:47.126880 gigachain-0.1.9/langchain/document_loaders/bigquery.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:47.127706 gigachain-0.1.9/langchain/document_loaders/bilibili.py
--rw-r--r--   0        0        0      109 2023-12-18 12:05:47.128455 gigachain-0.1.9/langchain/document_loaders/blackboard.py
--rw-r--r--   0        0        0      374 2024-01-18 15:16:40.702123 gigachain-0.1.9/langchain/document_loaders/blob_loaders/__init__.py
--rw-r--r--   0        0        0      140 2024-01-10 09:04:40.384621 gigachain-0.1.9/langchain/document_loaders/blob_loaders/file_system.py
--rw-r--r--   0        0        0      159 2023-12-18 12:05:47.130737 gigachain-0.1.9/langchain/document_loaders/blob_loaders/schema.py
--rw-r--r--   0        0        0      138 2023-12-18 12:05:47.131488 gigachain-0.1.9/langchain/document_loaders/blob_loaders/youtube_audio.py
--rw-r--r--   0        0        0      172 2023-12-18 12:05:47.132145 gigachain-0.1.9/langchain/document_loaders/blockchain.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.132987 gigachain-0.1.9/langchain/document_loaders/brave_search.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:47.133606 gigachain-0.1.9/langchain/document_loaders/browserless.py
--rw-r--r--   0        0        0      138 2023-12-18 12:05:47.134633 gigachain-0.1.9/langchain/document_loaders/chatgpt.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.135559 gigachain-0.1.9/langchain/document_loaders/chromium.py
--rw-r--r--   0        0        0      146 2023-12-18 12:05:47.137221 gigachain-0.1.9/langchain/document_loaders/college_confidential.py
--rw-r--r--   0        0        0      118 2024-01-10 09:04:40.385398 gigachain-0.1.9/langchain/document_loaders/concurrent.py
--rw-r--r--   0        0        0      154 2023-12-18 12:05:47.139495 gigachain-0.1.9/langchain/document_loaders/confluence.py
--rw-r--r--   0        0        0       97 2023-12-18 12:05:47.141295 gigachain-0.1.9/langchain/document_loaders/conllu.py
--rw-r--r--   0        0        0      106 2023-12-18 12:05:47.141905 gigachain-0.1.9/langchain/document_loaders/couchbase.py
--rw-r--r--   0        0        0      156 2023-12-18 12:05:47.142595 gigachain-0.1.9/langchain/document_loaders/csv_loader.py
--rw-r--r--   0        0        0      116 2023-12-18 12:05:47.143458 gigachain-0.1.9/langchain/document_loaders/cube_semantic.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.144613 gigachain-0.1.9/langchain/document_loaders/datadog_logs.py
--rw-r--r--   0        0        0      163 2023-12-18 12:05:47.145949 gigachain-0.1.9/langchain/document_loaders/dataframe.py
--rw-r--r--   0        0        0      100 2023-12-18 12:05:47.147296 gigachain-0.1.9/langchain/document_loaders/diffbot.py
--rw-r--r--   0        0        0      115 2024-01-10 09:04:40.386259 gigachain-0.1.9/langchain/document_loaders/directory.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:47.149307 gigachain-0.1.9/langchain/document_loaders/discord.py
--rw-r--r--   0        0        0      119 2024-01-10 09:04:40.387645 gigachain-0.1.9/langchain/document_loaders/docugami.py
--rw-r--r--   0        0        0      109 2023-12-18 12:05:47.150906 gigachain-0.1.9/langchain/document_loaders/docusaurus.py
--rw-r--r--   0        0        0      100 2023-12-18 12:05:47.151662 gigachain-0.1.9/langchain/document_loaders/dropbox.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:47.152424 gigachain-0.1.9/langchain/document_loaders/duckdb_loader.py
--rw-r--r--   0        0        0      177 2023-12-18 12:05:47.153750 gigachain-0.1.9/langchain/document_loaders/email.py
--rw-r--r--   0        0        0      115 2023-12-18 12:05:47.154940 gigachain-0.1.9/langchain/document_loaders/epub.py
--rw-r--r--   0        0        0      106 2023-12-18 12:05:47.156146 gigachain-0.1.9/langchain/document_loaders/etherscan.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:47.156948 gigachain-0.1.9/langchain/document_loaders/evernote.py
--rw-r--r--   0        0        0      118 2023-12-18 12:05:47.158021 gigachain-0.1.9/langchain/document_loaders/excel.py
--rw-r--r--   0        0        0      167 2023-12-18 12:05:47.158818 gigachain-0.1.9/langchain/document_loaders/facebook_chat.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.160349 gigachain-0.1.9/langchain/document_loaders/fauna.py
--rw-r--r--   0        0        0      102 2023-12-18 12:05:47.161384 gigachain-0.1.9/langchain/document_loaders/figma.py
--rw-r--r--   0        0        0      116 2023-12-18 12:05:47.163101 gigachain-0.1.9/langchain/document_loaders/gcs_directory.py
--rw-r--r--   0        0        0      101 2023-12-18 12:05:47.164293 gigachain-0.1.9/langchain/document_loaders/gcs_file.py
--rw-r--r--   0        0        0      109 2024-01-10 09:04:40.388322 gigachain-0.1.9/langchain/document_loaders/generic.py
--rw-r--r--   0        0        0      115 2023-12-18 12:05:47.166270 gigachain-0.1.9/langchain/document_loaders/geodataframe.py
--rw-r--r--   0        0        0       88 2023-12-18 12:05:47.167324 gigachain-0.1.9/langchain/document_loaders/git.py
--rw-r--r--   0        0        0      100 2023-12-18 12:05:47.168806 gigachain-0.1.9/langchain/document_loaders/gitbook.py
--rw-r--r--   0        0        0      160 2023-12-18 12:05:47.169956 gigachain-0.1.9/langchain/document_loaders/github.py
--rw-r--r--   0        0        0      145 2023-12-18 12:05:47.171116 gigachain-0.1.9/langchain/document_loaders/google_speech_to_text.py
--rw-r--r--   0        0        0      112 2024-01-10 09:04:40.389172 gigachain-0.1.9/langchain/document_loaders/googledrive.py
--rw-r--r--   0        0        0      106 2023-12-18 12:05:47.173144 gigachain-0.1.9/langchain/document_loaders/gutenberg.py
--rw-r--r--   0        0        0      159 2023-12-18 12:05:47.174366 gigachain-0.1.9/langchain/document_loaders/helpers.py
--rw-r--r--   0        0        0       85 2023-12-18 12:05:47.175285 gigachain-0.1.9/langchain/document_loaders/hn.py
--rw-r--r--   0        0        0      115 2023-12-18 12:05:47.176378 gigachain-0.1.9/langchain/document_loaders/html.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.177108 gigachain-0.1.9/langchain/document_loaders/html_bs.py
--rw-r--r--   0        0        0      144 2023-12-18 12:05:47.178240 gigachain-0.1.9/langchain/document_loaders/hugging_face_dataset.py
--rw-r--r--   0        0        0       97 2024-01-10 09:04:40.389976 gigachain-0.1.9/langchain/document_loaders/ifixit.py
--rw-r--r--   0        0        0      118 2023-12-18 12:05:47.180404 gigachain-0.1.9/langchain/document_loaders/image.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.181253 gigachain-0.1.9/langchain/document_loaders/image_captions.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.182514 gigachain-0.1.9/langchain/document_loaders/imsdb.py
--rw-r--r--   0        0        0       91 2024-01-10 09:04:40.390811 gigachain-0.1.9/langchain/document_loaders/iugu.py
--rw-r--r--   0        0        0       97 2024-01-10 09:04:40.391872 gigachain-0.1.9/langchain/document_loaders/joplin.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.184945 gigachain-0.1.9/langchain/document_loaders/json_loader.py
--rw-r--r--   0        0        0      198 2023-12-18 12:05:47.185665 gigachain-0.1.9/langchain/document_loaders/lakefs.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:47.186694 gigachain-0.1.9/langchain/document_loaders/larksuite.py
--rw-r--r--   0        0        0      127 2023-12-18 12:05:47.188009 gigachain-0.1.9/langchain/document_loaders/markdown.py
--rw-r--r--   0        0        0      122 2024-01-10 09:04:40.392640 gigachain-0.1.9/langchain/document_loaders/mastodon.py
--rw-r--r--   0        0        0      110 2023-12-18 12:05:47.190950 gigachain-0.1.9/langchain/document_loaders/max_compute.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:47.191580 gigachain-0.1.9/langchain/document_loaders/mediawikidump.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:47.192413 gigachain-0.1.9/langchain/document_loaders/merge.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.193132 gigachain-0.1.9/langchain/document_loaders/mhtml.py
--rw-r--r--   0        0        0      131 2024-01-10 09:04:40.393450 gigachain-0.1.9/langchain/document_loaders/modern_treasury.py
--rw-r--r--   0        0        0      100 2023-12-18 12:05:47.195107 gigachain-0.1.9/langchain/document_loaders/mongodb.py
--rw-r--r--   0        0        0       97 2023-12-18 12:05:47.196443 gigachain-0.1.9/langchain/document_loaders/news.py
--rw-r--r--   0        0        0      196 2023-12-18 12:05:47.198825 gigachain-0.1.9/langchain/document_loaders/notebook.py
--rw-r--r--   0        0        0      115 2023-12-18 12:05:47.199713 gigachain-0.1.9/langchain/document_loaders/notion.py
--rw-r--r--   0        0        0      112 2024-01-10 09:04:40.394263 gigachain-0.1.9/langchain/document_loaders/notiondb.py
--rw-r--r--   0        0        0       97 2023-12-18 12:05:47.201509 gigachain-0.1.9/langchain/document_loaders/nuclia.py
--rw-r--r--   0        0        0      116 2023-12-18 12:05:47.202637 gigachain-0.1.9/langchain/document_loaders/obs_directory.py
--rw-r--r--   0        0        0      101 2023-12-18 12:05:47.203432 gigachain-0.1.9/langchain/document_loaders/obs_file.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:47.204584 gigachain-0.1.9/langchain/document_loaders/obsidian.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:47.205631 gigachain-0.1.9/langchain/document_loaders/odt.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:47.206554 gigachain-0.1.9/langchain/document_loaders/onedrive.py
--rw-r--r--   0        0        0      125 2024-01-10 09:04:40.395058 gigachain-0.1.9/langchain/document_loaders/onedrive_file.py
--rw-r--r--   0        0        0      109 2024-01-10 09:04:40.395856 gigachain-0.1.9/langchain/document_loaders/onenote.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.209150 gigachain-0.1.9/langchain/document_loaders/open_city_data.py
--rw-r--r--   0        0        0      125 2023-12-18 12:05:47.209977 gigachain-0.1.9/langchain/document_loaders/org_mode.py
--rw-r--r--   0        0        0      789 2024-01-18 15:16:40.703524 gigachain-0.1.9/langchain/document_loaders/parsers/__init__.py
--rw-r--r--   0        0        0      225 2023-12-18 12:05:47.210876 gigachain-0.1.9/langchain/document_loaders/parsers/audio.py
--rw-r--r--   0        0        0      159 2023-12-18 12:05:47.211715 gigachain-0.1.9/langchain/document_loaders/parsers/docai.py
--rw-r--r--   0        0        0      120 2023-12-18 12:05:47.212945 gigachain-0.1.9/langchain/document_loaders/parsers/generic.py
--rw-r--r--   0        0        0      176 2024-01-10 09:04:40.397095 gigachain-0.1.9/langchain/document_loaders/parsers/grobid.py
--rw-r--r--   0        0        0      109 2024-01-18 15:16:40.704455 gigachain-0.1.9/langchain/document_loaders/parsers/html/__init__.py
--rw-r--r--   0        0        0      109 2023-12-18 12:05:47.214977 gigachain-0.1.9/langchain/document_loaders/parsers/html/bs4.py
--rw-r--r--   0        0        0      136 2024-01-18 15:16:40.705628 gigachain-0.1.9/langchain/document_loaders/parsers/language/__init__.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.216206 gigachain-0.1.9/langchain/document_loaders/parsers/language/cobol.py
--rw-r--r--   0        0        0      133 2023-12-18 12:05:47.217158 gigachain-0.1.9/langchain/document_loaders/parsers/language/code_segmenter.py
--rw-r--r--   0        0        0      141 2023-12-18 12:05:47.217871 gigachain-0.1.9/langchain/document_loaders/parsers/language/javascript.py
--rw-r--r--   0        0        0      136 2023-12-18 12:05:47.218842 gigachain-0.1.9/langchain/document_loaders/parsers/language/language_parser.py
--rw-r--r--   0        0        0      120 2023-12-18 12:05:47.219645 gigachain-0.1.9/langchain/document_loaders/parsers/language/python.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:47.220840 gigachain-0.1.9/langchain/document_loaders/parsers/msword.py
--rw-r--r--   0        0        0      494 2024-01-10 09:04:40.398416 gigachain-0.1.9/langchain/document_loaders/parsers/pdf.py
--rw-r--r--   0        0        0      112 2024-01-10 09:04:40.399315 gigachain-0.1.9/langchain/document_loaders/parsers/registry.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.223502 gigachain-0.1.9/langchain/document_loaders/parsers/txt.py
--rw-r--r--   0        0        0      706 2023-12-18 12:05:47.224305 gigachain-0.1.9/langchain/document_loaders/pdf.py
--rw-r--r--   0        0        0      125 2023-12-18 12:05:47.225423 gigachain-0.1.9/langchain/document_loaders/polars_dataframe.py
--rw-r--r--   0        0        0      133 2023-12-18 12:05:47.226416 gigachain-0.1.9/langchain/document_loaders/powerpoint.py
--rw-r--r--   0        0        0      100 2023-12-18 12:05:47.227234 gigachain-0.1.9/langchain/document_loaders/psychic.py
--rw-r--r--   0        0        0       97 2023-12-18 12:05:47.228478 gigachain-0.1.9/langchain/document_loaders/pubmed.py
--rw-r--r--   0        0        0      137 2023-12-18 12:05:47.229728 gigachain-0.1.9/langchain/document_loaders/pyspark_dataframe.py
--rw-r--r--   0        0        0       97 2023-12-18 12:05:47.230746 gigachain-0.1.9/langchain/document_loaders/python.py
--rw-r--r--   0        0        0       91 2024-01-10 09:04:40.400297 gigachain-0.1.9/langchain/document_loaders/quip.py
--rw-r--r--   0        0        0      128 2024-01-10 09:04:40.401198 gigachain-0.1.9/langchain/document_loaders/readthedocs.py
--rw-r--r--   0        0        0      132 2024-01-10 09:04:40.402205 gigachain-0.1.9/langchain/document_loaders/recursive_url_loader.py
--rw-r--r--   0        0        0      116 2024-01-10 09:04:40.403129 gigachain-0.1.9/langchain/document_loaders/reddit.py
--rw-r--r--   0        0        0       91 2023-12-18 12:05:47.234795 gigachain-0.1.9/langchain/document_loaders/roam.py
--rw-r--r--   0        0        0      111 2024-01-10 09:04:40.403904 gigachain-0.1.9/langchain/document_loaders/rocksetdb.py
--rw-r--r--   0        0        0       97 2023-12-18 12:05:47.236908 gigachain-0.1.9/langchain/document_loaders/rspace.py
--rw-r--r--   0        0        0       96 2023-12-18 12:05:47.237697 gigachain-0.1.9/langchain/document_loaders/rss.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:47.238291 gigachain-0.1.9/langchain/document_loaders/rst.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:47.239100 gigachain-0.1.9/langchain/document_loaders/rtf.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.239781 gigachain-0.1.9/langchain/document_loaders/s3_directory.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.240496 gigachain-0.1.9/langchain/document_loaders/s3_file.py
--rw-r--r--   0        0        0      109 2023-12-18 12:05:47.241193 gigachain-0.1.9/langchain/document_loaders/sharepoint.py
--rw-r--r--   0        0        0      116 2024-01-10 09:04:40.404728 gigachain-0.1.9/langchain/document_loaders/sitemap.py
--rw-r--r--   0        0        0      122 2023-12-18 12:05:47.243092 gigachain-0.1.9/langchain/document_loaders/slack_directory.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.243833 gigachain-0.1.9/langchain/document_loaders/snowflake_loader.py
--rw-r--r--   0        0        0      112 2024-01-10 09:04:40.405568 gigachain-0.1.9/langchain/document_loaders/spreedly.py
--rw-r--r--   0        0        0       88 2023-12-18 12:05:47.245722 gigachain-0.1.9/langchain/document_loaders/srt.py
--rw-r--r--   0        0        0       97 2024-01-10 09:04:40.406422 gigachain-0.1.9/langchain/document_loaders/stripe.py
--rw-r--r--   0        0        0      275 2023-12-18 12:05:47.248314 gigachain-0.1.9/langchain/document_loaders/telegram.py
--rw-r--r--   0        0        0      147 2023-12-18 12:05:47.249456 gigachain-0.1.9/langchain/document_loaders/tencent_cos_directory.py
--rw-r--r--   0        0        0      123 2023-12-18 12:05:47.250244 gigachain-0.1.9/langchain/document_loaders/tencent_cos_file.py
--rw-r--r--   0        0        0      141 2023-12-18 12:05:47.250861 gigachain-0.1.9/langchain/document_loaders/tensorflow_datasets.py
--rw-r--r--   0        0        0       91 2023-12-18 12:05:47.251412 gigachain-0.1.9/langchain/document_loaders/text.py
--rw-r--r--   0        0        0      109 2023-12-18 12:05:47.252277 gigachain-0.1.9/langchain/document_loaders/tomarkdown.py
--rw-r--r--   0        0        0       91 2023-12-18 12:05:47.253561 gigachain-0.1.9/langchain/document_loaders/toml.py
--rw-r--r--   0        0        0       97 2023-12-18 12:05:47.254464 gigachain-0.1.9/langchain/document_loaders/trello.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:47.255363 gigachain-0.1.9/langchain/document_loaders/tsv.py
--rw-r--r--   0        0        0      119 2024-01-10 09:04:40.407370 gigachain-0.1.9/langchain/document_loaders/twitter.py
--rw-r--r--   0        0        0      601 2023-12-18 12:05:47.259283 gigachain-0.1.9/langchain/document_loaders/unstructured.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:47.260397 gigachain-0.1.9/langchain/document_loaders/url.py
--rw-r--r--   0        0        0      236 2023-12-18 12:05:47.261334 gigachain-0.1.9/langchain/document_loaders/url_playwright.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.262991 gigachain-0.1.9/langchain/document_loaders/url_selenium.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:47.263820 gigachain-0.1.9/langchain/document_loaders/weather.py
--rw-r--r--   0        0        0      110 2024-01-10 09:04:40.408467 gigachain-0.1.9/langchain/document_loaders/web_base.py
--rw-r--r--   0        0        0      167 2023-12-18 12:05:47.265747 gigachain-0.1.9/langchain/document_loaders/whatsapp_chat.py
--rw-r--r--   0        0        0      106 2023-12-18 12:05:47.266913 gigachain-0.1.9/langchain/document_loaders/wikipedia.py
--rw-r--r--   0        0        0      187 2023-12-18 12:05:47.268711 gigachain-0.1.9/langchain/document_loaders/word_document.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:47.269613 gigachain-0.1.9/langchain/document_loaders/xml.py
--rw-r--r--   0        0        0      100 2023-12-18 12:05:47.270340 gigachain-0.1.9/langchain/document_loaders/xorbits.py
--rw-r--r--   0        0        0      218 2024-01-10 09:04:40.409212 gigachain-0.1.9/langchain/document_loaders/youtube.py
--rw-r--r--   0        0        0     1616 2024-02-22 08:54:03.257298 gigachain-0.1.9/langchain/document_transformers/__init__.py
--rw-r--r--   0        0        0      155 2024-01-10 09:04:40.410215 gigachain-0.1.9/langchain/document_transformers/beautiful_soup_transformer.py
--rw-r--r--   0        0        0      149 2023-12-18 12:05:47.274031 gigachain-0.1.9/langchain/document_transformers/doctran_text_extract.py
--rw-r--r--   0        0        0      136 2023-12-18 12:05:47.274901 gigachain-0.1.9/langchain/document_transformers/doctran_text_qa.py
--rw-r--r--   0        0        0      145 2023-12-18 12:05:47.275765 gigachain-0.1.9/langchain/document_transformers/doctran_text_translate.py
--rw-r--r--   0        0        0      487 2024-01-10 09:04:40.411019 gigachain-0.1.9/langchain/document_transformers/embeddings_redundant_filter.py
--rw-r--r--   0        0        0      149 2023-12-18 12:05:47.277716 gigachain-0.1.9/langchain/document_transformers/google_translate.py
--rw-r--r--   0        0        0      121 2023-12-18 12:05:47.278875 gigachain-0.1.9/langchain/document_transformers/html2text.py
--rw-r--r--   0        0        0     2042 2023-10-30 16:05:53.900619 gigachain-0.1.9/langchain/document_transformers/loading.py
--rw-r--r--   0        0        0      137 2024-01-10 09:04:40.411886 gigachain-0.1.9/langchain/document_transformers/long_context_reorder.py
--rw-r--r--   0        0        0      144 2023-12-18 12:05:47.280608 gigachain-0.1.9/langchain/document_transformers/nuclia_text_transform.py
--rw-r--r--   0        0        0      191 2023-12-18 12:05:47.281371 gigachain-0.1.9/langchain/document_transformers/openai_functions.py
--rw-r--r--   0        0        0     2103 2023-10-30 16:05:53.902104 gigachain-0.1.9/langchain/document_transformers/serializers.py
--rw-r--r--   0        0        0     6033 2023-10-06 14:43:01.456268 gigachain-0.1.9/langchain/document_transformers/xsl/html_chunks_with_headers.xslt
--rw-r--r--   0        0        0     3598 2024-02-22 08:54:03.259977 gigachain-0.1.9/langchain/embeddings/__init__.py
--rw-r--r--   0        0        0      248 2023-12-18 12:05:47.283533 gigachain-0.1.9/langchain/embeddings/aleph_alpha.py
--rw-r--r--   0        0        0       90 2023-12-18 12:05:47.284257 gigachain-0.1.9/langchain/embeddings/awa.py
--rw-r--r--   0        0        0      115 2023-12-18 12:05:47.285011 gigachain-0.1.9/langchain/embeddings/azure_openai.py
--rw-r--r--   0        0        0      142 2023-12-18 12:05:47.285672 gigachain-0.1.9/langchain/embeddings/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.286522 gigachain-0.1.9/langchain/embeddings/base.py
--rw-r--r--   0        0        0      102 2023-12-18 12:05:47.287374 gigachain-0.1.9/langchain/embeddings/bedrock.py
--rw-r--r--   0        0        0      111 2024-01-10 09:04:40.412764 gigachain-0.1.9/langchain/embeddings/bookend.py
--rw-r--r--   0        0        0     8260 2024-02-22 08:54:03.263810 gigachain-0.1.9/langchain/embeddings/cache.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:47.292653 gigachain-0.1.9/langchain/embeddings/clarifai.py
--rw-r--r--   0        0        0      148 2024-01-10 09:04:40.413596 gigachain-0.1.9/langchain/embeddings/cloudflare_workersai.py
--rw-r--r--   0        0        0       99 2023-12-18 12:05:47.293939 gigachain-0.1.9/langchain/embeddings/cohere.py
--rw-r--r--   0        0        0      117 2024-01-10 09:04:40.414696 gigachain-0.1.9/langchain/embeddings/dashscope.py
--rw-r--r--   0        0        0      111 2024-01-10 09:04:40.415721 gigachain-0.1.9/langchain/embeddings/databricks.py
--rw-r--r--   0        0        0      117 2024-01-10 09:04:40.416625 gigachain-0.1.9/langchain/embeddings/deepinfra.py
--rw-r--r--   0        0        0       99 2023-12-18 12:05:47.297444 gigachain-0.1.9/langchain/embeddings/edenai.py
--rw-r--r--   0        0        0      120 2023-12-18 12:05:47.298257 gigachain-0.1.9/langchain/embeddings/elasticsearch.py
--rw-r--r--   0        0        0      115 2024-01-10 09:04:40.417442 gigachain-0.1.9/langchain/embeddings/embaas.py
--rw-r--r--   0        0        0       96 2023-12-18 12:05:47.299986 gigachain-0.1.9/langchain/embeddings/ernie.py
--rw-r--r--   0        0        0      164 2023-12-18 12:05:47.300774 gigachain-0.1.9/langchain/embeddings/fake.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:47.301576 gigachain-0.1.9/langchain/embeddings/fastembed.py
--rw-r--r--   0        0        0      121 2024-01-10 09:04:40.418811 gigachain-0.1.9/langchain/embeddings/google_palm.py
--rw-r--r--   0        0        0      102 2023-12-18 12:05:47.303315 gigachain-0.1.9/langchain/embeddings/gpt4all.py
--rw-r--r--   0        0        0      108 2024-01-10 09:04:40.419865 gigachain-0.1.9/langchain/embeddings/gradient_ai.py
--rw-r--r--   0        0        0      344 2024-01-10 09:04:40.420673 gigachain-0.1.9/langchain/embeddings/huggingface.py
--rw-r--r--   0        0        0      133 2024-01-10 09:04:40.421652 gigachain-0.1.9/langchain/embeddings/huggingface_hub.py
--rw-r--r--   0        0        0      200 2023-12-18 12:05:47.305872 gigachain-0.1.9/langchain/embeddings/infinity.py
--rw-r--r--   0        0        0      140 2024-01-10 09:04:40.422554 gigachain-0.1.9/langchain/embeddings/javelin_ai_gateway.py
--rw-r--r--   0        0        0       93 2023-12-18 12:05:47.307827 gigachain-0.1.9/langchain/embeddings/jina.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.308610 gigachain-0.1.9/langchain/embeddings/johnsnowlabs.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:47.309681 gigachain-0.1.9/langchain/embeddings/llamacpp.py
--rw-r--r--   0        0        0      106 2023-12-18 12:05:47.310693 gigachain-0.1.9/langchain/embeddings/llm_rails.py
--rw-r--r--   0        0        0      118 2024-01-10 09:04:40.423295 gigachain-0.1.9/langchain/embeddings/localai.py
--rw-r--r--   0        0        0      111 2024-01-10 09:04:40.424032 gigachain-0.1.9/langchain/embeddings/minimax.py
--rw-r--r--   0        0        0       99 2024-01-10 09:04:40.425886 gigachain-0.1.9/langchain/embeddings/mlflow.py
--rw-r--r--   0        0        0      134 2024-01-10 09:04:40.427005 gigachain-0.1.9/langchain/embeddings/mlflow_gateway.py
--rw-r--r--   0        0        0      115 2023-12-18 12:05:47.314820 gigachain-0.1.9/langchain/embeddings/modelscope_hub.py
--rw-r--r--   0        0        0      125 2023-12-18 12:05:47.315663 gigachain-0.1.9/langchain/embeddings/mosaicml.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:47.316642 gigachain-0.1.9/langchain/embeddings/nlpcloud.py
--rw-r--r--   0        0        0      119 2024-01-10 09:04:40.427920 gigachain-0.1.9/langchain/embeddings/octoai_embeddings.py
--rw-r--r--   0        0        0       99 2023-12-18 12:05:47.318757 gigachain-0.1.9/langchain/embeddings/ollama.py
--rw-r--r--   0        0        0      115 2024-01-10 09:04:40.429049 gigachain-0.1.9/langchain/embeddings/openai.py
--rw-r--r--   0        0        0      200 2023-12-18 12:05:47.321173 gigachain-0.1.9/langchain/embeddings/sagemaker_endpoint.py
--rw-r--r--   0        0        0      121 2024-01-10 09:04:40.429895 gigachain-0.1.9/langchain/embeddings/self_hosted.py
--rw-r--r--   0        0        0      255 2024-01-10 09:04:40.430809 gigachain-0.1.9/langchain/embeddings/self_hosted_hugging_face.py
--rw-r--r--   0        0        0      148 2023-12-18 12:05:47.324200 gigachain-0.1.9/langchain/embeddings/sentence_transformer.py
--rw-r--r--   0        0        0      107 2023-12-18 12:05:47.325329 gigachain-0.1.9/langchain/embeddings/spacy_embeddings.py
--rw-r--r--   0        0        0      130 2024-01-10 09:04:40.432025 gigachain-0.1.9/langchain/embeddings/tensorflow_hub.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:47.327137 gigachain-0.1.9/langchain/embeddings/vertexai.py
--rw-r--r--   0        0        0      117 2024-01-10 09:04:40.433066 gigachain-0.1.9/langchain/embeddings/voyageai.py
--rw-r--r--   0        0        0      111 2023-12-18 12:05:47.328934 gigachain-0.1.9/langchain/embeddings/xinference.py
--rw-r--r--   0        0        0      476 2023-08-21 13:51:28.799282 gigachain-0.1.9/langchain/env.py
--rw-r--r--   0        0        0     5803 2023-10-30 16:05:53.905619 gigachain-0.1.9/langchain/evaluation/__init__.py
--rw-r--r--   0        0        0      165 2023-08-21 13:51:28.800913 gigachain-0.1.9/langchain/evaluation/agents/__init__.py
--rw-r--r--   0        0        0    13884 2024-02-22 08:54:03.265154 gigachain-0.1.9/langchain/evaluation/agents/trajectory_eval_chain.py
--rw-r--r--   0        0        0     9688 2023-12-18 12:05:47.331055 gigachain-0.1.9/langchain/evaluation/agents/trajectory_eval_prompt.py
--rw-r--r--   0        0        0     1400 2024-01-18 15:16:40.713791 gigachain-0.1.9/langchain/evaluation/comparison/__init__.py
--rw-r--r--   0        0        0    16056 2024-01-18 15:16:40.715217 gigachain-0.1.9/langchain/evaluation/comparison/eval_chain.py
--rw-r--r--   0        0        0     2358 2023-12-18 12:05:47.333888 gigachain-0.1.9/langchain/evaluation/comparison/prompt.py
--rw-r--r--   0        0        0     1647 2024-01-18 15:16:40.716003 gigachain-0.1.9/langchain/evaluation/criteria/__init__.py
--rw-r--r--   0        0        0    21358 2024-01-18 15:16:40.717295 gigachain-0.1.9/langchain/evaluation/criteria/eval_chain.py
--rw-r--r--   0        0        0     2723 2023-12-18 12:05:47.336070 gigachain-0.1.9/langchain/evaluation/criteria/prompt.py
--rw-r--r--   0        0        0      323 2023-08-21 13:51:28.806871 gigachain-0.1.9/langchain/evaluation/embedding_distance/__init__.py
--rw-r--r--   0        0        0    15503 2024-01-18 15:16:40.719400 gigachain-0.1.9/langchain/evaluation/embedding_distance/base.py
--rw-r--r--   0        0        0        0 2023-10-03 07:51:15.890624 gigachain-0.1.9/langchain/evaluation/exact_match/__init__.py
--rw-r--r--   0        0        0     2751 2023-10-03 07:51:15.891318 gigachain-0.1.9/langchain/evaluation/exact_match/base.py
--rw-r--r--   0        0        0     6693 2024-01-18 15:16:40.720469 gigachain-0.1.9/langchain/evaluation/loading.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.807950 gigachain-0.1.9/langchain/evaluation/parsing/__init__.py
--rw-r--r--   0        0        0     5246 2024-01-18 15:16:40.721461 gigachain-0.1.9/langchain/evaluation/parsing/base.py
--rw-r--r--   0        0        0     3679 2023-10-30 16:05:53.907474 gigachain-0.1.9/langchain/evaluation/parsing/json_distance.py
--rw-r--r--   0        0        0     3197 2023-10-30 16:05:53.907950 gigachain-0.1.9/langchain/evaluation/parsing/json_schema.py
--rw-r--r--   0        0        0      344 2023-08-21 13:51:28.808592 gigachain-0.1.9/langchain/evaluation/qa/__init__.py
--rw-r--r--   0        0        0    10886 2023-12-18 12:05:47.339833 gigachain-0.1.9/langchain/evaluation/qa/eval_chain.py
--rw-r--r--   0        0        0     6525 2023-12-18 12:05:47.340520 gigachain-0.1.9/langchain/evaluation/qa/eval_prompt.py
--rw-r--r--   0        0        0     1052 2023-12-18 12:05:47.341163 gigachain-0.1.9/langchain/evaluation/qa/generate_chain.py
--rw-r--r--   0        0        0      917 2023-12-18 12:05:47.341977 gigachain-0.1.9/langchain/evaluation/qa/generate_prompt.py
--rw-r--r--   0        0        0        0 2023-10-03 07:51:15.892405 gigachain-0.1.9/langchain/evaluation/regex_match/__init__.py
--rw-r--r--   0        0        0     2407 2023-10-03 07:51:15.893632 gigachain-0.1.9/langchain/evaluation/regex_match/base.py
--rw-r--r--   0        0        0    18197 2024-01-18 15:16:40.722881 gigachain-0.1.9/langchain/evaluation/schema.py
--rw-r--r--   0        0        0     1112 2024-01-18 15:16:40.723972 gigachain-0.1.9/langchain/evaluation/scoring/__init__.py
--rw-r--r--   0        0        0    15656 2024-01-18 15:16:40.725217 gigachain-0.1.9/langchain/evaluation/scoring/eval_chain.py
--rw-r--r--   0        0        0     2129 2023-12-18 12:05:47.344553 gigachain-0.1.9/langchain/evaluation/scoring/prompt.py
--rw-r--r--   0        0        0      285 2023-08-21 13:51:28.811472 gigachain-0.1.9/langchain/evaluation/string_distance/__init__.py
--rw-r--r--   0        0        0    14014 2023-12-18 12:05:47.346023 gigachain-0.1.9/langchain/evaluation/string_distance/base.py
--rw-r--r--   0        0        0      141 2023-08-21 13:51:28.812128 gigachain-0.1.9/langchain/example_generator.py
--rw-r--r--   0        0        0      167 2023-12-18 12:05:47.347238 gigachain-0.1.9/langchain/formatting.py
--rw-r--r--   0        0        0     7435 2023-12-18 12:05:47.348391 gigachain-0.1.9/langchain/globals/__init__.py
--rw-r--r--   0        0        0     1104 2024-02-22 08:54:03.267822 gigachain-0.1.9/langchain/graphs/__init__.py
--rw-r--r--   0        0        0      148 2024-01-10 09:04:40.437971 gigachain-0.1.9/langchain/graphs/arangodb_graph.py
--rw-r--r--   0        0        0      113 2024-01-10 09:04:40.438954 gigachain-0.1.9/langchain/graphs/falkordb_graph.py
--rw-r--r--   0        0        0      141 2023-12-18 12:05:47.350721 gigachain-0.1.9/langchain/graphs/graph_document.py
--rw-r--r--   0        0        0       88 2023-12-18 12:05:47.351490 gigachain-0.1.9/langchain/graphs/graph_store.py
--rw-r--r--   0        0        0       84 2023-12-18 12:05:47.352513 gigachain-0.1.9/langchain/graphs/hugegraph.py
--rw-r--r--   0        0        0       85 2023-12-18 12:05:47.353474 gigachain-0.1.9/langchain/graphs/kuzu_graph.py
--rw-r--r--   0        0        0      106 2024-01-10 09:04:40.439872 gigachain-0.1.9/langchain/graphs/memgraph_graph.py
--rw-r--r--   0        0        0       91 2024-01-10 09:04:40.440630 gigachain-0.1.9/langchain/graphs/nebula_graph.py
--rw-r--r--   0        0        0       97 2024-01-10 09:04:40.441708 gigachain-0.1.9/langchain/graphs/neo4j_graph.py
--rw-r--r--   0        0        0       94 2024-01-10 09:04:40.442566 gigachain-0.1.9/langchain/graphs/neptune_graph.py
--rw-r--r--   0        0        0      299 2023-12-18 12:05:47.358092 gigachain-0.1.9/langchain/graphs/networkx_graph.py
--rw-r--r--   0        0        0       98 2024-01-10 09:04:40.443339 gigachain-0.1.9/langchain/graphs/rdf_graph.py
--rw-r--r--   0        0        0     2874 2023-12-18 12:05:47.360240 gigachain-0.1.9/langchain/hub.py
--rw-r--r--   0        0        0      902 2024-03-01 11:50:11.630290 gigachain-0.1.9/langchain/indexes/__init__.py
--rw-r--r--   0        0        0    22479 2024-02-22 08:54:03.268766 gigachain-0.1.9/langchain/indexes/_api.py
--rw-r--r--   0        0        0    20556 2024-02-22 08:54:03.269921 gigachain-0.1.9/langchain/indexes/_sql_record_manager.py
--rw-r--r--   0        0        0     5221 2023-10-19 12:57:52.916879 gigachain-0.1.9/langchain/indexes/base.py
--rw-r--r--   0        0        0     1752 2024-01-18 15:16:40.727874 gigachain-0.1.9/langchain/indexes/graph.py
--rw-r--r--   0        0        0       49 2023-08-21 13:51:28.816990 gigachain-0.1.9/langchain/indexes/prompts/__init__.py
--rw-r--r--   0        0        0     3241 2023-12-18 12:05:47.364265 gigachain-0.1.9/langchain/indexes/prompts/entity_extraction.py
--rw-r--r--   0        0        0     1797 2023-12-18 12:05:47.365149 gigachain-0.1.9/langchain/indexes/prompts/entity_summarization.py
--rw-r--r--   0        0        0     2276 2024-01-18 15:16:40.730868 gigachain-0.1.9/langchain/indexes/prompts/knowledge_triplet_extraction.py
--rw-r--r--   0        0        0     3423 2024-01-18 15:16:40.731835 gigachain-0.1.9/langchain/indexes/vectorstore.py
--rw-r--r--   0        0        0      282 2023-12-18 12:05:47.367912 gigachain-0.1.9/langchain/input.py
--rw-r--r--   0        0        0    17126 2024-02-22 08:54:03.273345 gigachain-0.1.9/langchain/llms/__init__.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:47.373059 gigachain-0.1.9/langchain/llms/ai21.py
--rw-r--r--   0        0        0       86 2023-12-18 12:05:47.375795 gigachain-0.1.9/langchain/llms/aleph_alpha.py
--rw-r--r--   0        0        0      114 2024-01-10 09:04:40.445264 gigachain-0.1.9/langchain/llms/amazon_api_gateway.py
--rw-r--r--   0        0        0       82 2024-01-10 09:04:40.446089 gigachain-0.1.9/langchain/llms/anthropic.py
--rw-r--r--   0        0        0       88 2024-01-10 09:04:40.446963 gigachain-0.1.9/langchain/llms/anyscale.py
--rw-r--r--   0        0        0       70 2023-12-18 12:05:47.380664 gigachain-0.1.9/langchain/llms/arcee.py
--rw-r--r--   0        0        0       82 2024-01-10 09:04:40.448322 gigachain-0.1.9/langchain/llms/aviary.py
--rw-r--r--   0        0        0      507 2023-12-18 12:05:47.382858 gigachain-0.1.9/langchain/llms/azureml_endpoint.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.383805 gigachain-0.1.9/langchain/llms/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0       76 2023-12-18 12:05:47.384682 gigachain-0.1.9/langchain/llms/bananadev.py
--rw-r--r--   0        0        0      228 2024-01-10 09:04:40.449816 gigachain-0.1.9/langchain/llms/base.py
--rw-r--r--   0        0        0       76 2023-12-18 12:05:47.386653 gigachain-0.1.9/langchain/llms/baseten.py
--rw-r--r--   0        0        0       67 2024-01-10 09:04:40.450756 gigachain-0.1.9/langchain/llms/beam.py
--rw-r--r--   0        0        0      128 2024-01-10 09:04:40.451692 gigachain-0.1.9/langchain/llms/bedrock.py
--rw-r--r--   0        0        0       92 2023-12-18 12:05:47.389069 gigachain-0.1.9/langchain/llms/bittensor.py
--rw-r--r--   0        0        0       88 2023-12-18 12:05:47.389772 gigachain-0.1.9/langchain/llms/cerebriumai.py
--rw-r--r--   0        0        0       76 2023-12-18 12:05:47.390471 gigachain-0.1.9/langchain/llms/chatglm.py
--rw-r--r--   0        0        0       79 2024-01-10 09:04:40.452477 gigachain-0.1.9/langchain/llms/clarifai.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.391687 gigachain-0.1.9/langchain/llms/cloudflare_workersai.py
--rw-r--r--   0        0        0       89 2024-01-10 09:04:40.453363 gigachain-0.1.9/langchain/llms/cohere.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.393292 gigachain-0.1.9/langchain/llms/ctransformers.py
--rw-r--r--   0        0        0       88 2023-12-18 12:05:47.394040 gigachain-0.1.9/langchain/llms/ctranslate2.py
--rw-r--r--   0        0        0      101 2024-01-10 09:04:40.454645 gigachain-0.1.9/langchain/llms/databricks.py
--rw-r--r--   0        0        0       98 2024-01-10 09:04:40.455573 gigachain-0.1.9/langchain/llms/deepinfra.py
--rw-r--r--   0        0        0       85 2023-12-18 12:05:47.397072 gigachain-0.1.9/langchain/llms/deepsparse.py
--rw-r--r--   0        0        0       73 2023-12-18 12:05:47.397873 gigachain-0.1.9/langchain/llms/edenai.py
--rw-r--r--   0        0        0      127 2023-12-18 12:05:47.399013 gigachain-0.1.9/langchain/llms/fake.py
--rw-r--r--   0        0        0       98 2024-01-10 09:04:40.456495 gigachain-0.1.9/langchain/llms/fireworks.py
--rw-r--r--   0        0        0       88 2023-12-18 12:05:47.400669 gigachain-0.1.9/langchain/llms/forefrontai.py
--rw-r--r--   0        0        0       79 2024-01-10 09:04:40.457511 gigachain-0.1.9/langchain/llms/gigachat.py
--rw-r--r--   0        0        0       86 2024-01-10 09:04:40.459648 gigachain-0.1.9/langchain/llms/google_palm.py
--rw-r--r--   0        0        0       76 2023-12-18 12:05:47.403054 gigachain-0.1.9/langchain/llms/gooseai.py
--rw-r--r--   0        0        0       76 2023-12-18 12:05:47.403988 gigachain-0.1.9/langchain/llms/gpt4all.py
--rw-r--r--   0        0        0      116 2023-12-18 12:05:47.404853 gigachain-0.1.9/langchain/llms/gradient_ai.py
--rw-r--r--   0        0        0      664 2023-08-29 13:18:02.701979 gigachain-0.1.9/langchain/llms/grammars/json.gbnf
--rw-r--r--   0        0        0      167 2023-08-29 13:18:02.702167 gigachain-0.1.9/langchain/llms/grammars/list.gbnf
--rw-r--r--   0        0        0      122 2024-01-10 09:04:40.460567 gigachain-0.1.9/langchain/llms/huggingface_endpoint.py
--rw-r--r--   0        0        0      107 2024-01-10 09:04:40.461738 gigachain-0.1.9/langchain/llms/huggingface_hub.py
--rw-r--r--   0        0        0      129 2024-01-10 09:04:40.462973 gigachain-0.1.9/langchain/llms/huggingface_pipeline.py
--rw-r--r--   0        0        0      148 2023-12-18 12:05:47.408597 gigachain-0.1.9/langchain/llms/huggingface_text_gen_inference.py
--rw-r--r--   0        0        0       95 2024-01-10 09:04:40.464144 gigachain-0.1.9/langchain/llms/human.py
--rw-r--r--   0        0        0      123 2024-01-10 09:04:40.465399 gigachain-0.1.9/langchain/llms/javelin_ai_gateway.py
--rw-r--r--   0        0        0       87 2024-01-10 09:04:40.466206 gigachain-0.1.9/langchain/llms/koboldai.py
--rw-r--r--   0        0        0       79 2023-12-18 12:05:47.413304 gigachain-0.1.9/langchain/llms/llamacpp.py
--rw-r--r--   0        0        0      124 2023-12-18 12:05:47.414682 gigachain-0.1.9/langchain/llms/loading.py
--rw-r--r--   0        0        0       93 2023-12-18 12:05:47.415424 gigachain-0.1.9/langchain/llms/manifest.py
--rw-r--r--   0        0        0       85 2024-01-10 09:04:40.467239 gigachain-0.1.9/langchain/llms/minimax.py
--rw-r--r--   0        0        0       73 2024-01-10 09:04:40.468921 gigachain-0.1.9/langchain/llms/mlflow.py
--rw-r--r--   0        0        0      102 2024-01-10 09:04:40.469899 gigachain-0.1.9/langchain/llms/mlflow_ai_gateway.py
--rw-r--r--   0        0        0       70 2023-12-18 12:05:47.418198 gigachain-0.1.9/langchain/llms/modal.py
--rw-r--r--   0        0        0       95 2024-01-10 09:04:40.470830 gigachain-0.1.9/langchain/llms/mosaicml.py
--rw-r--r--   0        0        0       79 2023-12-18 12:05:47.419808 gigachain-0.1.9/langchain/llms/nlpcloud.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.420848 gigachain-0.1.9/langchain/llms/octoai_endpoint.py
--rw-r--r--   0        0        0       82 2024-01-10 09:04:40.471699 gigachain-0.1.9/langchain/llms/ollama.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.422749 gigachain-0.1.9/langchain/llms/opaqueprompts.py
--rw-r--r--   0        0        0      193 2024-01-10 09:04:40.472465 gigachain-0.1.9/langchain/llms/openai.py
--rw-r--r--   0        0        0       76 2024-01-10 09:04:40.473297 gigachain-0.1.9/langchain/llms/openllm.py
--rw-r--r--   0        0        0       73 2023-12-18 12:05:47.425514 gigachain-0.1.9/langchain/llms/openlm.py
--rw-r--r--   0        0        0       99 2023-12-18 12:05:47.426494 gigachain-0.1.9/langchain/llms/pai_eas_endpoint.py
--rw-r--r--   0        0        0       73 2023-12-18 12:05:47.427233 gigachain-0.1.9/langchain/llms/petals.py
--rw-r--r--   0        0        0       85 2023-12-18 12:05:47.427965 gigachain-0.1.9/langchain/llms/pipelineai.py
--rw-r--r--   0        0        0       82 2023-12-18 12:05:47.428665 gigachain-0.1.9/langchain/llms/predibase.py
--rw-r--r--   0        0        0      100 2023-12-18 12:05:47.429339 gigachain-0.1.9/langchain/llms/predictionguard.py
--rw-r--r--   0        0        0      168 2023-12-18 12:05:47.430258 gigachain-0.1.9/langchain/llms/promptlayer_openai.py
--rw-r--r--   0        0        0       82 2023-12-18 12:05:47.431189 gigachain-0.1.9/langchain/llms/replicate.py
--rw-r--r--   0        0        0       67 2023-12-18 12:05:47.431973 gigachain-0.1.9/langchain/llms/rwkv.py
--rw-r--r--   0        0        0      160 2024-01-10 09:04:40.479050 gigachain-0.1.9/langchain/llms/sagemaker_endpoint.py
--rw-r--r--   0        0        0      111 2024-01-10 09:04:40.479967 gigachain-0.1.9/langchain/llms/self_hosted.py
--rw-r--r--   0        0        0      143 2024-01-10 09:04:40.480961 gigachain-0.1.9/langchain/llms/self_hosted_hugging_face.py
--rw-r--r--   0        0        0       91 2023-12-18 12:05:47.435028 gigachain-0.1.9/langchain/llms/stochasticai.py
--rw-r--r--   0        0        0       97 2024-01-10 09:04:40.481881 gigachain-0.1.9/langchain/llms/symblai_nebula.py
--rw-r--r--   0        0        0       76 2023-12-18 12:05:47.436528 gigachain-0.1.9/langchain/llms/textgen.py
--rw-r--r--   0        0        0       92 2023-12-18 12:05:47.437384 gigachain-0.1.9/langchain/llms/titan_takeoff.py
--rw-r--r--   0        0        0      102 2023-12-18 12:05:47.438099 gigachain-0.1.9/langchain/llms/titan_takeoff_pro.py
--rw-r--r--   0        0        0       79 2023-12-18 12:05:47.438940 gigachain-0.1.9/langchain/llms/together.py
--rw-r--r--   0        0        0       89 2024-01-10 09:04:40.482832 gigachain-0.1.9/langchain/llms/tongyi.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.440079 gigachain-0.1.9/langchain/llms/utils.py
--rw-r--r--   0        0        0      147 2024-01-10 09:04:40.483851 gigachain-0.1.9/langchain/llms/vertexai.py
--rw-r--r--   0        0        0       93 2023-12-18 12:05:47.441569 gigachain-0.1.9/langchain/llms/vllm.py
--rw-r--r--   0        0        0      159 2023-12-18 12:05:47.441823 gigachain-0.1.9/langchain/llms/volcengine_maas.py
--rw-r--r--   0        0        0       85 2023-12-18 12:05:47.442050 gigachain-0.1.9/langchain/llms/watsonxllm.py
--rw-r--r--   0        0        0       73 2023-12-18 12:05:47.442855 gigachain-0.1.9/langchain/llms/writer.py
--rw-r--r--   0        0        0       85 2023-12-18 12:05:47.443467 gigachain-0.1.9/langchain/llms/xinference.py
--rw-r--r--   0        0        0       79 2024-01-10 09:04:40.484703 gigachain-0.1.9/langchain/llms/yandex.py
--rw-r--r--   0        0        0      206 2023-12-18 12:05:47.445806 gigachain-0.1.9/langchain/load/__init__.py
--rw-r--r--   0        0        0      100 2023-12-18 12:05:47.446683 gigachain-0.1.9/langchain/load/dump.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.447484 gigachain-0.1.9/langchain/load/load.py
--rw-r--r--   0        0        0      412 2023-12-18 12:05:47.448066 gigachain-0.1.9/langchain/load/serializable.py
--rw-r--r--   0        0        0     3256 2024-01-18 15:16:40.735874 gigachain-0.1.9/langchain/memory/__init__.py
--rw-r--r--   0        0        0     4861 2024-02-22 08:54:03.274556 gigachain-0.1.9/langchain/memory/buffer.py
--rw-r--r--   0        0        0     1616 2024-03-01 11:50:11.631255 gigachain-0.1.9/langchain/memory/buffer_window.py
--rw-r--r--   0        0        0     2245 2024-02-22 08:54:03.275441 gigachain-0.1.9/langchain/memory/chat_memory.py
--rw-r--r--   0        0        0     1560 2024-02-22 08:54:03.277945 gigachain-0.1.9/langchain/memory/chat_message_histories/__init__.py
--rw-r--r--   0        0        0      139 2024-01-10 09:04:40.485550 gigachain-0.1.9/langchain/memory/chat_message_histories/astradb.py
--rw-r--r--   0        0        0      145 2024-01-10 09:04:40.486385 gigachain-0.1.9/langchain/memory/chat_message_histories/cassandra.py
--rw-r--r--   0        0        0      143 2023-12-18 12:05:47.453355 gigachain-0.1.9/langchain/memory/chat_message_histories/cosmos_db.py
--rw-r--r--   0        0        0      142 2023-12-18 12:05:47.454333 gigachain-0.1.9/langchain/memory/chat_message_histories/dynamodb.py
--rw-r--r--   0        0        0      157 2023-12-18 12:05:47.455260 gigachain-0.1.9/langchain/memory/chat_message_histories/elasticsearch.py
--rw-r--r--   0        0        0      121 2023-12-18 12:05:47.456262 gigachain-0.1.9/langchain/memory/chat_message_histories/file.py
--rw-r--r--   0        0        0      145 2024-01-10 09:04:40.487202 gigachain-0.1.9/langchain/memory/chat_message_histories/firestore.py
--rw-r--r--   0        0        0      118 2023-12-18 12:05:47.458129 gigachain-0.1.9/langchain/memory/chat_message_histories/in_memory.py
--rw-r--r--   0        0        0      139 2024-01-10 09:04:40.488531 gigachain-0.1.9/langchain/memory/chat_message_histories/momento.py
--rw-r--r--   0        0        0      139 2024-01-10 09:04:40.489333 gigachain-0.1.9/langchain/memory/chat_message_histories/mongodb.py
--rw-r--r--   0        0        0      124 2023-12-18 12:05:47.461292 gigachain-0.1.9/langchain/memory/chat_message_histories/neo4j.py
--rw-r--r--   0        0        0      142 2024-01-10 09:04:40.490216 gigachain-0.1.9/langchain/memory/chat_message_histories/postgres.py
--rw-r--r--   0        0        0      124 2023-12-18 12:05:47.469349 gigachain-0.1.9/langchain/memory/chat_message_histories/redis.py
--rw-r--r--   0        0        0      141 2023-12-18 12:05:47.470277 gigachain-0.1.9/langchain/memory/chat_message_histories/rocksetdb.py
--rw-r--r--   0        0        0      157 2023-12-18 12:05:47.474949 gigachain-0.1.9/langchain/memory/chat_message_histories/singlestoredb.py
--rw-r--r--   0        0        0      248 2024-01-10 09:04:40.492289 gigachain-0.1.9/langchain/memory/chat_message_histories/sql.py
--rw-r--r--   0        0        0      145 2023-12-18 12:05:47.476873 gigachain-0.1.9/langchain/memory/chat_message_histories/streamlit.py
--rw-r--r--   0        0        0      155 2023-12-18 12:05:47.477734 gigachain-0.1.9/langchain/memory/chat_message_histories/upstash_redis.py
--rw-r--r--   0        0        0      121 2023-12-18 12:05:47.478747 gigachain-0.1.9/langchain/memory/chat_message_histories/xata.py
--rw-r--r--   0        0        0      118 2023-12-18 12:05:47.479566 gigachain-0.1.9/langchain/memory/chat_message_histories/zep.py
--rw-r--r--   0        0        0     2912 2023-12-18 12:05:47.480430 gigachain-0.1.9/langchain/memory/combined.py
--rw-r--r--   0        0        0    15677 2024-02-22 08:54:03.279615 gigachain-0.1.9/langchain/memory/entity.py
--rw-r--r--   0        0        0     5075 2024-01-18 15:16:40.739203 gigachain-0.1.9/langchain/memory/kg.py
--rw-r--r--   0        0        0     3106 2023-12-18 12:05:47.483008 gigachain-0.1.9/langchain/memory/motorhead_memory.py
--rw-r--r--   0        0        0    13128 2023-12-18 12:05:47.483791 gigachain-0.1.9/langchain/memory/prompt.py
--rw-r--r--   0        0        0      794 2023-12-18 12:05:47.484537 gigachain-0.1.9/langchain/memory/readonly.py
--rw-r--r--   0        0        0      761 2023-12-18 12:05:47.485293 gigachain-0.1.9/langchain/memory/simple.py
--rw-r--r--   0        0        0     3389 2023-12-18 12:05:47.485998 gigachain-0.1.9/langchain/memory/summary.py
--rw-r--r--   0        0        0     2949 2023-12-18 12:05:47.486936 gigachain-0.1.9/langchain/memory/summary_buffer.py
--rw-r--r--   0        0        0     2144 2023-12-18 12:05:47.487927 gigachain-0.1.9/langchain/memory/token_buffer.py
--rw-r--r--   0        0        0      617 2023-08-29 13:18:02.706587 gigachain-0.1.9/langchain/memory/utils.py
--rw-r--r--   0        0        0     3002 2023-12-18 12:05:47.489028 gigachain-0.1.9/langchain/memory/vectorstore.py
--rw-r--r--   0        0        0     5090 2024-01-18 15:16:40.740045 gigachain-0.1.9/langchain/memory/zep_memory.py
--rw-r--r--   0        0        0     3278 2024-02-22 08:54:03.280782 gigachain-0.1.9/langchain/model_laboratory.py
--rw-r--r--   0        0        0     2216 2023-12-18 12:05:47.491014 gigachain-0.1.9/langchain/output_parsers/__init__.py
--rw-r--r--   0        0        0     1433 2024-03-01 11:50:11.632242 gigachain-0.1.9/langchain/output_parsers/boolean.py
--rw-r--r--   0        0        0     1799 2023-12-18 12:05:47.492673 gigachain-0.1.9/langchain/output_parsers/combining.py
--rw-r--r--   0        0        0     1924 2024-02-22 08:54:03.283314 gigachain-0.1.9/langchain/output_parsers/datetime.py
--rw-r--r--   0        0        0     1205 2023-12-18 12:05:47.494416 gigachain-0.1.9/langchain/output_parsers/enum.py
--rw-r--r--   0        0        0      424 2024-02-22 08:54:03.284260 gigachain-0.1.9/langchain/output_parsers/ernie_functions.py
--rw-r--r--   0        0        0     3153 2023-12-18 12:05:47.496827 gigachain-0.1.9/langchain/output_parsers/fix.py
--rw-r--r--   0        0        0     3958 2024-01-18 15:16:40.741558 gigachain-0.1.9/langchain/output_parsers/format_instructions.py
--rw-r--r--   0        0        0      298 2024-01-10 09:04:40.495028 gigachain-0.1.9/langchain/output_parsers/json.py
--rw-r--r--   0        0        0      310 2023-12-18 12:05:47.500021 gigachain-0.1.9/langchain/output_parsers/list.py
--rw-r--r--   0        0        0      702 2023-08-21 13:51:28.860635 gigachain-0.1.9/langchain/output_parsers/loading.py
--rw-r--r--   0        0        0      364 2024-03-01 11:50:11.633028 gigachain-0.1.9/langchain/output_parsers/openai_functions.py
--rw-r--r--   0        0        0      229 2024-03-01 11:50:11.633712 gigachain-0.1.9/langchain/output_parsers/openai_tools.py
--rw-r--r--   0        0        0     6548 2024-02-22 08:54:03.288456 gigachain-0.1.9/langchain/output_parsers/pandas_dataframe.py
--rw-r--r--   0        0        0      699 2023-12-18 12:05:47.503286 gigachain-0.1.9/langchain/output_parsers/prompts.py
--rw-r--r--   0        0        0       99 2024-03-01 11:50:11.634691 gigachain-0.1.9/langchain/output_parsers/pydantic.py
--rw-r--r--   0        0        0      129 2024-02-22 08:54:03.292714 gigachain-0.1.9/langchain/output_parsers/rail_parser.py
--rw-r--r--   0        0        0     1214 2023-12-18 12:05:47.506059 gigachain-0.1.9/langchain/output_parsers/regex.py
--rw-r--r--   0        0        0     1709 2023-12-18 12:05:47.506885 gigachain-0.1.9/langchain/output_parsers/regex_dict.py
--rw-r--r--   0        0        0     7792 2024-01-18 15:16:40.746608 gigachain-0.1.9/langchain/output_parsers/retry.py
--rw-r--r--   0        0        0     3134 2024-02-22 08:54:03.293969 gigachain-0.1.9/langchain/output_parsers/structured.py
--rw-r--r--   0        0        0       93 2024-01-10 09:04:40.496050 gigachain-0.1.9/langchain/output_parsers/xml.py
--rw-r--r--   0        0        0     2181 2024-02-22 08:54:03.295025 gigachain-0.1.9/langchain/output_parsers/yaml.py
--rw-r--r--   0        0        0     2560 2023-12-18 12:05:47.510676 gigachain-0.1.9/langchain/prompts/__init__.py
--rw-r--r--   0        0        0      565 2023-12-18 12:05:47.511466 gigachain-0.1.9/langchain/prompts/base.py
--rw-r--r--   0        0        0     1045 2023-12-18 12:05:47.512665 gigachain-0.1.9/langchain/prompts/chat.py
--rw-r--r--   0        0        0      568 2023-12-18 12:05:47.513679 gigachain-0.1.9/langchain/prompts/example_selector/__init__.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:47.514537 gigachain-0.1.9/langchain/prompts/example_selector/base.py
--rw-r--r--   0        0        0      136 2023-12-18 12:05:47.515578 gigachain-0.1.9/langchain/prompts/example_selector/length_based.py
--rw-r--r--   0        0        0      203 2024-02-22 08:54:03.296005 gigachain-0.1.9/langchain/prompts/example_selector/ngram_overlap.py
--rw-r--r--   0        0        0      288 2023-12-18 12:05:47.517451 gigachain-0.1.9/langchain/prompts/example_selector/semantic_similarity.py
--rw-r--r--   0        0        0      265 2023-12-18 12:05:47.518312 gigachain-0.1.9/langchain/prompts/few_shot.py
--rw-r--r--   0        0        0      128 2023-12-18 12:05:47.519153 gigachain-0.1.9/langchain/prompts/few_shot_with_templates.py
--rw-r--r--   0        0        0      530 2023-12-18 12:05:47.519896 gigachain-0.1.9/langchain/prompts/loading.py
--rw-r--r--   0        0        0      133 2023-12-18 12:05:47.520643 gigachain-0.1.9/langchain/prompts/pipeline.py
--rw-r--r--   0        0        0      153 2023-12-18 12:05:47.521708 gigachain-0.1.9/langchain/prompts/prompt.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.868214 gigachain-0.1.9/langchain/py.typed
--rw-r--r--   0        0        0      897 2023-08-21 13:51:28.868582 gigachain-0.1.9/langchain/pydantic_v1/__init__.py
--rw-r--r--   0        0        0      134 2023-08-21 13:51:28.868846 gigachain-0.1.9/langchain/pydantic_v1/dataclasses.py
--rw-r--r--   0        0        0      120 2023-08-21 13:51:28.869090 gigachain-0.1.9/langchain/pydantic_v1/main.py
--rw-r--r--   0        0        0      121 2024-01-18 15:16:40.748012 gigachain-0.1.9/langchain/python.py
--rw-r--r--   0        0        0      222 2024-01-18 15:16:40.748946 gigachain-0.1.9/langchain/requests.py
--rw-r--r--   0        0        0     3488 2024-02-22 08:54:03.298877 gigachain-0.1.9/langchain/retrievers/__init__.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.523253 gigachain-0.1.9/langchain/retrievers/arcee.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.524007 gigachain-0.1.9/langchain/retrievers/arxiv.py
--rw-r--r--   0        0        0      150 2024-01-10 09:04:40.496942 gigachain-0.1.9/langchain/retrievers/azure_cognitive_search.py
--rw-r--r--   0        0        0      221 2023-12-18 12:05:47.525596 gigachain-0.1.9/langchain/retrievers/bedrock.py
--rw-r--r--   0        0        0      162 2023-12-18 12:05:47.526294 gigachain-0.1.9/langchain/retrievers/bm25.py
--rw-r--r--   0        0        0      106 2023-12-18 12:05:47.527002 gigachain-0.1.9/langchain/retrievers/chaindesk.py
--rw-r--r--   0        0        0      138 2023-12-18 12:05:47.527627 gigachain-0.1.9/langchain/retrievers/chatgpt_plugin_retriever.py
--rw-r--r--   0        0        0      126 2024-01-10 09:04:40.497936 gigachain-0.1.9/langchain/retrievers/cohere_rag_retriever.py
--rw-r--r--   0        0        0     2298 2024-02-22 08:54:03.299860 gigachain-0.1.9/langchain/retrievers/contextual_compression.py
--rw-r--r--   0        0        0      106 2023-12-18 12:05:47.530630 gigachain-0.1.9/langchain/retrievers/databerry.py
--rw-r--r--   0        0        0      129 2023-12-18 12:05:47.531715 gigachain-0.1.9/langchain/retrievers/docarray.py
--rw-r--r--   0        0        0      701 2024-02-22 08:54:03.300629 gigachain-0.1.9/langchain/retrievers/document_compressors/__init__.py
--rw-r--r--   0        0        0     2938 2024-03-01 11:50:11.635714 gigachain-0.1.9/langchain/retrievers/document_compressors/base.py
--rw-r--r--   0        0        0     3955 2024-02-22 08:54:03.301513 gigachain-0.1.9/langchain/retrievers/document_compressors/chain_extract.py
--rw-r--r--   0        0        0      621 2023-08-21 13:51:28.874260 gigachain-0.1.9/langchain/retrievers/document_compressors/chain_extract_prompt.py
--rw-r--r--   0        0        0     2757 2023-12-18 12:05:47.535586 gigachain-0.1.9/langchain/retrievers/document_compressors/chain_filter.py
--rw-r--r--   0        0        0      336 2023-09-04 15:41:37.267607 gigachain-0.1.9/langchain/retrievers/document_compressors/chain_filter_prompt.py
--rw-r--r--   0        0        0     4213 2024-02-22 08:54:03.302441 gigachain-0.1.9/langchain/retrievers/document_compressors/cohere_rerank.py
--rw-r--r--   0        0        0     3031 2024-01-18 15:16:40.752303 gigachain-0.1.9/langchain/retrievers/document_compressors/embeddings_filter.py
--rw-r--r--   0        0        0     2415 2024-02-22 08:54:03.302873 gigachain-0.1.9/langchain/retrievers/document_compressors/flashrank_rerank.py
--rw-r--r--   0        0        0      141 2023-12-18 12:05:47.538561 gigachain-0.1.9/langchain/retrievers/elastic_search_bm25.py
--rw-r--r--   0        0        0      109 2023-12-18 12:05:47.539048 gigachain-0.1.9/langchain/retrievers/embedchain.py
--rw-r--r--   0        0        0     9668 2024-02-22 08:54:03.304010 gigachain-0.1.9/langchain/retrievers/ensemble.py
--rw-r--r--   0        0        0      171 2023-12-18 12:05:47.540495 gigachain-0.1.9/langchain/retrievers/google_cloud_documentai_warehouse.py
--rw-r--r--   0        0        0      334 2024-01-10 09:04:40.499089 gigachain-0.1.9/langchain/retrievers/google_vertex_ai_search.py
--rw-r--r--   0        0        0       92 2023-12-18 12:05:47.542055 gigachain-0.1.9/langchain/retrievers/kay.py
--rw-r--r--   0        0        0      803 2023-12-18 12:05:47.542775 gigachain-0.1.9/langchain/retrievers/kendra.py
--rw-r--r--   0        0        0       88 2024-01-10 09:04:40.499990 gigachain-0.1.9/langchain/retrievers/knn.py
--rw-r--r--   0        0        0      177 2023-12-18 12:05:47.544144 gigachain-0.1.9/langchain/retrievers/llama_index.py
--rw-r--r--   0        0        0     3489 2024-02-22 08:54:03.304848 gigachain-0.1.9/langchain/retrievers/merger_retriever.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.546337 gigachain-0.1.9/langchain/retrievers/metal.py
--rw-r--r--   0        0        0      133 2023-12-18 12:05:47.547245 gigachain-0.1.9/langchain/retrievers/milvus.py
--rw-r--r--   0        0        0     7120 2024-02-22 08:54:03.308226 gigachain-0.1.9/langchain/retrievers/multi_query.py
--rw-r--r--   0        0        0     3920 2024-02-22 08:54:03.309148 gigachain-0.1.9/langchain/retrievers/multi_vector.py
--rw-r--r--   0        0        0      100 2023-12-18 12:05:47.549986 gigachain-0.1.9/langchain/retrievers/outline.py
--rw-r--r--   0        0        0     5196 2024-02-22 08:54:03.310174 gigachain-0.1.9/langchain/retrievers/parent_document_retriever.py
--rw-r--r--   0        0        0      150 2024-01-10 09:04:40.501259 gigachain-0.1.9/langchain/retrievers/pinecone_hybrid_search.py
--rw-r--r--   0        0        0       97 2023-12-18 12:05:47.552477 gigachain-0.1.9/langchain/retrievers/pubmed.py
--rw-r--r--   0        0        0       94 2023-08-21 13:51:28.881470 gigachain-0.1.9/langchain/retrievers/pupmed.py
--rw-r--r--   0        0        0     2930 2024-02-22 08:54:03.313542 gigachain-0.1.9/langchain/retrievers/re_phraser.py
--rw-r--r--   0        0        0      125 2023-12-18 12:05:47.554463 gigachain-0.1.9/langchain/retrievers/remote_retriever.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.882217 gigachain-0.1.9/langchain/retrievers/self_query/__init__.py
--rw-r--r--   0        0        0     2194 2024-02-22 08:54:03.314677 gigachain-0.1.9/langchain/retrievers/self_query/astradb.py
--rw-r--r--   0        0        0    10068 2024-03-01 11:50:11.636759 gigachain-0.1.9/langchain/retrievers/self_query/base.py
--rw-r--r--   0        0        0     1474 2023-09-12 10:52:10.683073 gigachain-0.1.9/langchain/retrievers/self_query/chroma.py
--rw-r--r--   0        0        0     1918 2024-01-18 15:16:40.762739 gigachain-0.1.9/langchain/retrievers/self_query/dashvector.py
--rw-r--r--   0        0        0     2592 2023-09-04 05:57:22.522888 gigachain-0.1.9/langchain/retrievers/self_query/deeplake.py
--rw-r--r--   0        0        0     3273 2024-02-22 08:54:03.317536 gigachain-0.1.9/langchain/retrievers/self_query/elasticsearch.py
--rw-r--r--   0        0        0     3352 2024-02-22 08:54:03.318497 gigachain-0.1.9/langchain/retrievers/self_query/milvus.py
--rw-r--r--   0        0        0     2303 2023-12-18 12:05:47.558690 gigachain-0.1.9/langchain/retrievers/self_query/mongodb_atlas.py
--rw-r--r--   0        0        0     3636 2024-02-22 08:54:03.319483 gigachain-0.1.9/langchain/retrievers/self_query/myscale.py
--rw-r--r--   0        0        0     3271 2024-02-22 08:54:03.320355 gigachain-0.1.9/langchain/retrievers/self_query/opensearch.py
--rw-r--r--   0        0        0     1529 2024-02-22 08:54:03.320824 gigachain-0.1.9/langchain/retrievers/self_query/pgvector.py
--rw-r--r--   0        0        0     1687 2023-10-06 14:43:01.539605 gigachain-0.1.9/langchain/retrievers/self_query/pinecone.py
--rw-r--r--   0        0        0     3168 2024-02-22 08:54:03.321769 gigachain-0.1.9/langchain/retrievers/self_query/qdrant.py
--rw-r--r--   0        0        0     3376 2024-01-18 15:16:40.763805 gigachain-0.1.9/langchain/retrievers/self_query/redis.py
--rw-r--r--   0        0        0     2974 2023-09-12 10:52:10.683619 gigachain-0.1.9/langchain/retrievers/self_query/supabase.py
--rw-r--r--   0        0        0     2633 2023-09-25 07:40:35.527447 gigachain-0.1.9/langchain/retrievers/self_query/timescalevector.py
--rw-r--r--   0        0        0     2164 2023-10-19 12:57:53.001031 gigachain-0.1.9/langchain/retrievers/self_query/vectara.py
--rw-r--r--   0        0        0     2619 2023-11-15 10:30:09.358178 gigachain-0.1.9/langchain/retrievers/self_query/weaviate.py
--rw-r--r--   0        0        0       88 2024-01-10 09:04:40.503132 gigachain-0.1.9/langchain/retrievers/svm.py
--rw-r--r--   0        0        0      167 2023-12-18 12:05:47.560135 gigachain-0.1.9/langchain/retrievers/tavily_search_api.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.560807 gigachain-0.1.9/langchain/retrievers/tfidf.py
--rw-r--r--   0        0        0     6279 2024-02-22 08:54:03.324848 gigachain-0.1.9/langchain/retrievers/time_weighted_retriever.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:47.564083 gigachain-0.1.9/langchain/retrievers/vespa_retriever.py
--rw-r--r--   0        0        0      150 2023-12-18 12:05:47.566297 gigachain-0.1.9/langchain/retrievers/weaviate_hybrid_search.py
--rw-r--r--   0        0        0     9014 2024-03-01 11:50:11.638549 gigachain-0.1.9/langchain/retrievers/web_research.py
--rw-r--r--   0        0        0      106 2023-12-18 12:05:47.567950 gigachain-0.1.9/langchain/retrievers/wikipedia.py
--rw-r--r--   0        0        0       88 2023-12-18 12:05:47.569099 gigachain-0.1.9/langchain/retrievers/you.py
--rw-r--r--   0        0        0      142 2023-12-18 12:05:47.569898 gigachain-0.1.9/langchain/retrievers/zep.py
--rw-r--r--   0        0        0      133 2023-12-18 12:05:47.570757 gigachain-0.1.9/langchain/retrievers/zilliz.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.887732 gigachain-0.1.9/langchain/runnables/__init__.py
--rw-r--r--   0        0        0      809 2023-12-18 12:05:47.571530 gigachain-0.1.9/langchain/runnables/hub.py
--rw-r--r--   0        0        0     1525 2024-03-01 11:50:11.639231 gigachain-0.1.9/langchain/runnables/openai_functions.py
--rw-r--r--   0        0        0     2065 2023-12-18 12:05:47.575459 gigachain-0.1.9/langchain/schema/__init__.py
--rw-r--r--   0        0        0      149 2023-12-18 12:05:47.576297 gigachain-0.1.9/langchain/schema/agent.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:47.576979 gigachain-0.1.9/langchain/schema/cache.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:47.577169 gigachain-0.1.9/langchain/schema/callbacks/__init__.py
--rw-r--r--   0        0        0      511 2023-12-18 12:05:47.577786 gigachain-0.1.9/langchain/schema/callbacks/base.py
--rw-r--r--   0        0        0     1511 2023-12-18 12:05:47.578611 gigachain-0.1.9/langchain/schema/callbacks/manager.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:47.579043 gigachain-0.1.9/langchain/schema/callbacks/stdout.py
--rw-r--r--   0        0        0      131 2023-12-18 12:05:47.579408 gigachain-0.1.9/langchain/schema/callbacks/streaming_stdout.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:47.579637 gigachain-0.1.9/langchain/schema/callbacks/tracers/__init__.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.580043 gigachain-0.1.9/langchain/schema/callbacks/tracers/base.py
--rw-r--r--   0        0        0      176 2023-12-18 12:05:47.580505 gigachain-0.1.9/langchain/schema/callbacks/tracers/evaluation.py
--rw-r--r--   0        0        0      219 2023-12-18 12:05:47.580868 gigachain-0.1.9/langchain/schema/callbacks/tracers/langchain.py
--rw-r--r--   0        0        0      127 2023-12-18 12:05:47.581282 gigachain-0.1.9/langchain/schema/callbacks/tracers/langchain_v1.py
--rw-r--r--   0        0        0      226 2023-12-18 12:05:47.581685 gigachain-0.1.9/langchain/schema/callbacks/tracers/log_stream.py
--rw-r--r--   0        0        0      105 2023-12-18 12:05:47.582039 gigachain-0.1.9/langchain/schema/callbacks/tracers/root_listeners.py
--rw-r--r--   0        0        0      120 2023-12-18 12:05:47.582518 gigachain-0.1.9/langchain/schema/callbacks/tracers/run_collector.py
--rw-r--r--   0        0        0      470 2023-12-18 12:05:47.582779 gigachain-0.1.9/langchain/schema/callbacks/tracers/schemas.py
--rw-r--r--   0        0        0      257 2023-12-18 12:05:47.583106 gigachain-0.1.9/langchain/schema/callbacks/tracers/stdout.py
--rw-r--r--   0        0        0       80 2023-12-18 12:05:47.583799 gigachain-0.1.9/langchain/schema/chat.py
--rw-r--r--   0        0        0      101 2023-12-18 12:05:47.584843 gigachain-0.1.9/langchain/schema/chat_history.py
--rw-r--r--   0        0        0      122 2023-12-18 12:05:47.585605 gigachain-0.1.9/langchain/schema/document.py
--rw-r--r--   0        0        0       75 2023-12-18 12:05:47.586431 gigachain-0.1.9/langchain/schema/embeddings.py
--rw-r--r--   0        0        0       91 2023-12-18 12:05:47.587468 gigachain-0.1.9/langchain/schema/exceptions.py
--rw-r--r--   0        0        0      367 2023-12-18 12:05:47.588176 gigachain-0.1.9/langchain/schema/language_model.py
--rw-r--r--   0        0        0       71 2023-12-18 12:05:47.588957 gigachain-0.1.9/langchain/schema/memory.py
--rw-r--r--   0        0        0     1048 2023-12-18 12:05:47.589743 gigachain-0.1.9/langchain/schema/messages.py
--rw-r--r--   0        0        0      320 2023-12-18 12:05:47.590462 gigachain-0.1.9/langchain/schema/output.py
--rw-r--r--   0        0        0      651 2023-12-18 12:05:47.591291 gigachain-0.1.9/langchain/schema/output_parser.py
--rw-r--r--   0        0        0       80 2023-12-18 12:05:47.592095 gigachain-0.1.9/langchain/schema/prompt.py
--rw-r--r--   0        0        0      124 2023-12-18 12:05:47.592918 gigachain-0.1.9/langchain/schema/prompt_template.py
--rw-r--r--   0        0        0       81 2023-12-18 12:05:47.593622 gigachain-0.1.9/langchain/schema/retriever.py
--rw-r--r--   0        0        0     1796 2023-12-18 12:05:47.594714 gigachain-0.1.9/langchain/schema/runnable/__init__.py
--rw-r--r--   0        0        0      781 2023-12-18 12:05:47.595763 gigachain-0.1.9/langchain/schema/runnable/base.py
--rw-r--r--   0        0        0       89 2023-12-18 12:05:47.596655 gigachain-0.1.9/langchain/schema/runnable/branch.py
--rw-r--r--   0        0        0      665 2023-12-18 12:05:47.597563 gigachain-0.1.9/langchain/schema/runnable/config.py
--rw-r--r--   0        0        0      333 2023-12-18 12:05:47.598462 gigachain-0.1.9/langchain/schema/runnable/configurable.py
--rw-r--r--   0        0        0      106 2023-12-18 12:05:47.599358 gigachain-0.1.9/langchain/schema/runnable/fallbacks.py
--rw-r--r--   0        0        0      260 2023-12-18 12:05:47.600021 gigachain-0.1.9/langchain/schema/runnable/history.py
--rw-r--r--   0        0        0      205 2023-12-18 12:05:47.600672 gigachain-0.1.9/langchain/schema/runnable/passthrough.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.601412 gigachain-0.1.9/langchain/schema/runnable/retry.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.602442 gigachain-0.1.9/langchain/schema/runnable/router.py
--rw-r--r--   0        0        0     1118 2023-12-18 12:05:47.603240 gigachain-0.1.9/langchain/schema/runnable/utils.py
--rw-r--r--   0        0        0       85 2023-12-18 12:05:47.604392 gigachain-0.1.9/langchain/schema/storage.py
--rw-r--r--   0        0        0      137 2023-12-18 12:05:47.605680 gigachain-0.1.9/langchain/schema/vectorstore.py
--rw-r--r--   0        0        0      130 2024-01-18 15:16:40.768493 gigachain-0.1.9/langchain/serpapi.py
--rw-r--r--   0        0        0     3544 2024-01-18 15:16:40.769415 gigachain-0.1.9/langchain/smith/__init__.py
--rw-r--r--   0        0        0     2199 2024-01-18 15:16:40.770441 gigachain-0.1.9/langchain/smith/evaluation/__init__.py
--rw-r--r--   0        0        0    12480 2024-01-10 09:04:40.504756 gigachain-0.1.9/langchain/smith/evaluation/config.py
--rw-r--r--   0        0        0     9936 2023-12-18 12:05:47.609341 gigachain-0.1.9/langchain/smith/evaluation/name_generation.py
--rw-r--r--   0        0        0     3310 2024-03-01 11:50:11.639824 gigachain-0.1.9/langchain/smith/evaluation/progress.py
--rw-r--r--   0        0        0    50978 2024-02-22 08:54:03.330642 gigachain-0.1.9/langchain/smith/evaluation/runner_utils.py
--rw-r--r--   0        0        0    17107 2023-12-18 12:05:47.613221 gigachain-0.1.9/langchain/smith/evaluation/string_run_evaluator.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.895985 gigachain-0.1.9/langchain/smith/evaluation/utils.py
--rw-r--r--   0        0        0      139 2024-01-18 15:16:40.773265 gigachain-0.1.9/langchain/sql_database.py
--rw-r--r--   0        0        0     1571 2024-02-22 08:54:03.333134 gigachain-0.1.9/langchain/storage/__init__.py
--rw-r--r--   0        0        0     2517 2023-12-18 12:05:47.615861 gigachain-0.1.9/langchain/storage/_lc_store.py
--rw-r--r--   0        0        0     2970 2023-12-18 12:05:47.616837 gigachain-0.1.9/langchain/storage/encoder_backed.py
--rw-r--r--   0        0        0      106 2023-12-18 12:05:47.617809 gigachain-0.1.9/langchain/storage/exceptions.py
--rw-r--r--   0        0        0     4307 2024-02-22 08:54:03.334261 gigachain-0.1.9/langchain/storage/file_system.py
--rw-r--r--   0        0        0     4448 2024-02-22 08:54:03.335210 gigachain-0.1.9/langchain/storage/in_memory.py
--rw-r--r--   0        0        0       83 2023-12-18 12:05:47.621280 gigachain-0.1.9/langchain/storage/redis.py
--rw-r--r--   0        0        0      166 2024-01-10 09:04:40.510757 gigachain-0.1.9/langchain/storage/upstash_redis.py
--rw-r--r--   0        0        0    55865 2024-02-22 08:54:03.336949 gigachain-0.1.9/langchain/text_splitter.py
--rw-r--r--   0        0        0     5663 2024-01-18 15:16:40.776804 gigachain-0.1.9/langchain/tools/__init__.py
--rw-r--r--   0        0        0      166 2023-12-18 12:05:47.625523 gigachain-0.1.9/langchain/tools/ainetwork/app.py
--rw-r--r--   0        0        0      124 2023-12-18 12:05:47.626232 gigachain-0.1.9/langchain/tools/ainetwork/base.py
--rw-r--r--   0        0        0      119 2023-12-18 12:05:47.626998 gigachain-0.1.9/langchain/tools/ainetwork/owner.py
--rw-r--r--   0        0        0      116 2023-12-18 12:05:47.627720 gigachain-0.1.9/langchain/tools/ainetwork/rule.py
--rw-r--r--   0        0        0      130 2023-12-18 12:05:47.628416 gigachain-0.1.9/langchain/tools/ainetwork/transfer.py
--rw-r--r--   0        0        0      121 2023-12-18 12:05:47.630133 gigachain-0.1.9/langchain/tools/ainetwork/value.py
--rw-r--r--   0        0        0      257 2024-01-18 15:16:40.778408 gigachain-0.1.9/langchain/tools/amadeus/__init__.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.630970 gigachain-0.1.9/langchain/tools/amadeus/base.py
--rw-r--r--   0        0        0      180 2023-12-18 12:05:47.632104 gigachain-0.1.9/langchain/tools/amadeus/closest_airport.py
--rw-r--r--   0        0        0      170 2023-12-18 12:05:47.632931 gigachain-0.1.9/langchain/tools/amadeus/flight_search.py
--rw-r--r--   0        0        0       25 2023-08-21 13:51:28.901095 gigachain-0.1.9/langchain/tools/arxiv/__init__.py
--rw-r--r--   0        0        0      118 2023-12-18 12:05:47.634560 gigachain-0.1.9/langchain/tools/arxiv/tool.py
--rw-r--r--   0        0        0      802 2024-01-18 15:16:40.780425 gigachain-0.1.9/langchain/tools/azure_cognitive_services/__init__.py
--rw-r--r--   0        0        0      159 2023-12-18 12:05:47.636784 gigachain-0.1.9/langchain/tools/azure_cognitive_services/form_recognizer.py
--rw-r--r--   0        0        0      156 2023-12-18 12:05:47.638067 gigachain-0.1.9/langchain/tools/azure_cognitive_services/image_analysis.py
--rw-r--r--   0        0        0      149 2023-12-18 12:05:47.638948 gigachain-0.1.9/langchain/tools/azure_cognitive_services/speech2text.py
--rw-r--r--   0        0        0      149 2023-12-18 12:05:47.639702 gigachain-0.1.9/langchain/tools/azure_cognitive_services/text2speech.py
--rw-r--r--   0        0        0      175 2023-12-18 12:05:47.640091 gigachain-0.1.9/langchain/tools/azure_cognitive_services/text_analytics_health.py
--rw-r--r--   0        0        0      332 2024-01-10 09:04:40.515503 gigachain-0.1.9/langchain/tools/base.py
--rw-r--r--   0        0        0        0 2023-10-19 12:57:53.049903 gigachain-0.1.9/langchain/tools/bearly/__init__.py
--rw-r--r--   0        0        0      229 2024-01-10 09:04:40.518070 gigachain-0.1.9/langchain/tools/bearly/tool.py
--rw-r--r--   0        0        0      170 2024-01-18 15:16:40.781740 gigachain-0.1.9/langchain/tools/bing_search/__init__.py
--rw-r--r--   0        0        0      138 2023-12-18 12:05:47.643848 gigachain-0.1.9/langchain/tools/bing_search/tool.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.906784 gigachain-0.1.9/langchain/tools/brave_search/__init__.py
--rw-r--r--   0        0        0       95 2023-12-18 12:05:47.644621 gigachain-0.1.9/langchain/tools/brave_search/tool.py
--rw-r--r--   0        0        0        0 2023-10-06 14:43:01.562867 gigachain-0.1.9/langchain/tools/clickup/__init__.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.646160 gigachain-0.1.9/langchain/tools/clickup/tool.py
--rw-r--r--   0        0        0      157 2024-02-22 08:54:03.337885 gigachain-0.1.9/langchain/tools/convert_to_openai.py
--rw-r--r--   0        0        0      268 2024-01-18 15:16:40.785078 gigachain-0.1.9/langchain/tools/dataforseo_api_search/__init__.py
--rw-r--r--   0        0        0      197 2023-12-18 12:05:47.647471 gigachain-0.1.9/langchain/tools/dataforseo_api_search/tool.py
--rw-r--r--   0        0        0      147 2024-01-18 15:16:40.786394 gigachain-0.1.9/langchain/tools/ddg_search/__init__.py
--rw-r--r--   0        0        0      269 2023-12-18 12:05:47.648366 gigachain-0.1.9/langchain/tools/ddg_search/tool.py
--rw-r--r--   0        0        0        0 2023-10-30 16:05:53.968119 gigachain-0.1.9/langchain/tools/e2b_data_analysis/__init__.py
--rw-r--r--   0        0        0      240 2024-01-10 09:04:40.519149 gigachain-0.1.9/langchain/tools/e2b_data_analysis/tool.py
--rw-r--r--   0        0        0     1024 2024-01-18 15:16:40.788076 gigachain-0.1.9/langchain/tools/edenai/__init__.py
--rw-r--r--   0        0        0      127 2023-12-18 12:05:47.651357 gigachain-0.1.9/langchain/tools/edenai/audio_speech_to_text.py
--rw-r--r--   0        0        0      127 2023-12-18 12:05:47.652284 gigachain-0.1.9/langchain/tools/edenai/audio_text_to_speech.py
--rw-r--r--   0        0        0       99 2023-12-18 12:05:47.653108 gigachain-0.1.9/langchain/tools/edenai/edenai_base_tool.py
--rw-r--r--   0        0        0      139 2023-12-18 12:05:47.654289 gigachain-0.1.9/langchain/tools/edenai/image_explicitcontent.py
--rw-r--r--   0        0        0      143 2023-12-18 12:05:47.667832 gigachain-0.1.9/langchain/tools/edenai/image_objectdetection.py
--rw-r--r--   0        0        0      119 2023-12-18 12:05:47.673367 gigachain-0.1.9/langchain/tools/edenai/ocr_identityparser.py
--rw-r--r--   0        0        0      128 2023-12-18 12:05:47.678230 gigachain-0.1.9/langchain/tools/edenai/ocr_invoiceparser.py
--rw-r--r--   0        0        0      126 2023-12-18 12:05:47.680238 gigachain-0.1.9/langchain/tools/edenai/text_moderation.py
--rw-r--r--   0        0        0      164 2024-01-18 15:16:40.789002 gigachain-0.1.9/langchain/tools/eleven_labs/__init__.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:47.681114 gigachain-0.1.9/langchain/tools/eleven_labs/models.py
--rw-r--r--   0        0        0      138 2024-01-10 09:04:40.520141 gigachain-0.1.9/langchain/tools/eleven_labs/text2speech.py
--rw-r--r--   0        0        0      723 2024-01-18 15:16:40.790286 gigachain-0.1.9/langchain/tools/file_management/__init__.py
--rw-r--r--   0        0        0      132 2023-12-18 12:05:47.683048 gigachain-0.1.9/langchain/tools/file_management/copy.py
--rw-r--r--   0        0        0      155 2023-12-18 12:05:47.684055 gigachain-0.1.9/langchain/tools/file_management/delete.py
--rw-r--r--   0        0        0      160 2023-12-18 12:05:47.684795 gigachain-0.1.9/langchain/tools/file_management/file_search.py
--rw-r--r--   0        0        0      175 2023-12-18 12:05:47.685876 gigachain-0.1.9/langchain/tools/file_management/list_dir.py
--rw-r--r--   0        0        0      132 2023-12-18 12:05:47.687226 gigachain-0.1.9/langchain/tools/file_management/move.py
--rw-r--r--   0        0        0      132 2023-12-18 12:05:47.688294 gigachain-0.1.9/langchain/tools/file_management/read.py
--rw-r--r--   0        0        0      150 2023-12-18 12:05:47.690230 gigachain-0.1.9/langchain/tools/file_management/write.py
--rw-r--r--   0        0        0       20 2023-08-21 13:51:28.913036 gigachain-0.1.9/langchain/tools/github/__init__.py
--rw-r--r--   0        0        0       91 2023-12-18 12:05:47.692510 gigachain-0.1.9/langchain/tools/github/tool.py
--rw-r--r--   0        0        0       20 2023-09-19 14:33:02.316769 gigachain-0.1.9/langchain/tools/gitlab/__init__.py
--rw-r--r--   0        0        0       91 2023-12-18 12:05:47.694012 gigachain-0.1.9/langchain/tools/gitlab/tool.py
--rw-r--r--   0        0        0      500 2024-01-18 15:16:40.791834 gigachain-0.1.9/langchain/tools/gmail/__init__.py
--rw-r--r--   0        0        0       92 2023-12-18 12:05:47.695102 gigachain-0.1.9/langchain/tools/gmail/base.py
--rw-r--r--   0        0        0      159 2023-12-18 12:05:47.696034 gigachain-0.1.9/langchain/tools/gmail/create_draft.py
--rw-r--r--   0        0        0      154 2023-12-18 12:05:47.696879 gigachain-0.1.9/langchain/tools/gmail/get_message.py
--rw-r--r--   0        0        0      136 2023-12-18 12:05:47.697691 gigachain-0.1.9/langchain/tools/gmail/get_thread.py
--rw-r--r--   0        0        0      167 2023-12-18 12:05:47.698533 gigachain-0.1.9/langchain/tools/gmail/search.py
--rw-r--r--   0        0        0      159 2023-12-18 12:05:47.699261 gigachain-0.1.9/langchain/tools/gmail/send_message.py
--rw-r--r--   0        0        0      136 2024-01-18 15:16:40.794195 gigachain-0.1.9/langchain/tools/golden_query/__init__.py
--rw-r--r--   0        0        0      101 2023-12-18 12:05:47.701139 gigachain-0.1.9/langchain/tools/golden_query/tool.py
--rw-r--r--   0        0        0      171 2024-01-18 15:16:40.795771 gigachain-0.1.9/langchain/tools/google_cloud/__init__.py
--rw-r--r--   0        0        0      151 2024-01-10 09:04:40.524958 gigachain-0.1.9/langchain/tools/google_cloud/texttospeech.py
--rw-r--r--   0        0        0      152 2024-01-18 15:16:40.798988 gigachain-0.1.9/langchain/tools/google_finance/__init__.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.703299 gigachain-0.1.9/langchain/tools/google_finance/tool.py
--rw-r--r--   0        0        0      140 2024-01-18 15:16:40.802247 gigachain-0.1.9/langchain/tools/google_jobs/__init__.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:47.703936 gigachain-0.1.9/langchain/tools/google_jobs/tool.py
--rw-r--r--   0        0        0      140 2024-01-18 15:16:40.804061 gigachain-0.1.9/langchain/tools/google_lens/__init__.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:47.704750 gigachain-0.1.9/langchain/tools/google_lens/tool.py
--rw-r--r--   0        0        0      140 2024-01-18 15:16:40.808715 gigachain-0.1.9/langchain/tools/google_places/__init__.py
--rw-r--r--   0        0        0      161 2023-12-18 12:05:47.706017 gigachain-0.1.9/langchain/tools/google_places/tool.py
--rw-r--r--   0        0        0      152 2024-01-18 15:16:40.810765 gigachain-0.1.9/langchain/tools/google_scholar/__init__.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.707012 gigachain-0.1.9/langchain/tools/google_scholar/tool.py
--rw-r--r--   0        0        0      195 2024-01-18 15:16:40.814439 gigachain-0.1.9/langchain/tools/google_search/__init__.py
--rw-r--r--   0        0        0      161 2023-12-18 12:05:47.708241 gigachain-0.1.9/langchain/tools/google_search/tool.py
--rw-r--r--   0        0        0      243 2024-01-18 15:16:40.816966 gigachain-0.1.9/langchain/tools/google_serper/__init__.py
--rw-r--r--   0        0        0      161 2023-12-18 12:05:47.709262 gigachain-0.1.9/langchain/tools/google_serper/tool.py
--rw-r--r--   0        0        0      148 2024-01-18 15:16:40.824180 gigachain-0.1.9/langchain/tools/google_trends/__init__.py
--rw-r--r--   0        0        0      114 2023-12-18 12:05:47.709982 gigachain-0.1.9/langchain/tools/google_trends/tool.py
--rw-r--r--   0        0        0       47 2023-08-21 13:51:28.921484 gigachain-0.1.9/langchain/tools/graphql/__init__.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.710894 gigachain-0.1.9/langchain/tools/graphql/tool.py
--rw-r--r--   0        0        0      132 2024-01-18 15:16:40.829390 gigachain-0.1.9/langchain/tools/human/__init__.py
--rw-r--r--   0        0        0       92 2024-01-10 09:04:40.530860 gigachain-0.1.9/langchain/tools/human/tool.py
--rw-r--r--   0        0        0       85 2023-12-18 12:05:47.713440 gigachain-0.1.9/langchain/tools/ifttt.py
--rw-r--r--   0        0        0       43 2023-08-21 13:51:28.923495 gigachain-0.1.9/langchain/tools/interaction/__init__.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:47.714893 gigachain-0.1.9/langchain/tools/interaction/tool.py
--rw-r--r--   0        0        0       17 2023-08-21 13:51:28.924161 gigachain-0.1.9/langchain/tools/jira/__init__.py
--rw-r--r--   0        0        0       85 2023-12-18 12:05:47.717607 gigachain-0.1.9/langchain/tools/jira/tool.py
--rw-r--r--   0        0        0       46 2023-08-21 13:51:28.925352 gigachain-0.1.9/langchain/tools/json/__init__.py
--rw-r--r--   0        0        0      174 2024-01-10 09:04:40.535392 gigachain-0.1.9/langchain/tools/json/tool.py
--rw-r--r--   0        0        0      134 2024-01-18 15:16:40.836631 gigachain-0.1.9/langchain/tools/memorize/__init__.py
--rw-r--r--   0        0        0      115 2023-12-18 12:05:47.719498 gigachain-0.1.9/langchain/tools/memorize/tool.py
--rw-r--r--   0        0        0       35 2023-12-18 12:05:47.720059 gigachain-0.1.9/langchain/tools/merriam_webster/__init__.py
--rw-r--r--   0        0        0      120 2023-12-18 12:05:47.720682 gigachain-0.1.9/langchain/tools/merriam_webster/tool.py
--rw-r--r--   0        0        0      154 2024-01-18 15:16:40.840932 gigachain-0.1.9/langchain/tools/metaphor_search/__init__.py
--rw-r--r--   0        0        0      118 2023-12-18 12:05:47.721767 gigachain-0.1.9/langchain/tools/metaphor_search/tool.py
--rw-r--r--   0        0        0      359 2024-01-18 15:16:40.842423 gigachain-0.1.9/langchain/tools/multion/__init__.py
--rw-r--r--   0        0        0      170 2023-12-18 12:05:47.722885 gigachain-0.1.9/langchain/tools/multion/close_session.py
--rw-r--r--   0        0        0      175 2023-12-18 12:05:47.723750 gigachain-0.1.9/langchain/tools/multion/create_session.py
--rw-r--r--   0        0        0      175 2023-12-18 12:05:47.724545 gigachain-0.1.9/langchain/tools/multion/update_session.py
--rw-r--r--   0        0        0        0 2023-12-18 12:05:47.724833 gigachain-0.1.9/langchain/tools/nasa/__init__.py
--rw-r--r--   0        0        0       85 2023-12-18 12:05:47.725566 gigachain-0.1.9/langchain/tools/nasa/tool.py
--rw-r--r--   0        0        0      111 2024-01-18 15:16:40.844691 gigachain-0.1.9/langchain/tools/nuclia/__init__.py
--rw-r--r--   0        0        0      135 2023-12-18 12:05:47.726427 gigachain-0.1.9/langchain/tools/nuclia/tool.py
--rw-r--r--   0        0        0      567 2024-01-18 15:16:40.847490 gigachain-0.1.9/langchain/tools/office365/__init__.py
--rw-r--r--   0        0        0       94 2023-12-18 12:05:47.727311 gigachain-0.1.9/langchain/tools/office365/base.py
--rw-r--r--   0        0        0      197 2023-12-18 12:05:47.728682 gigachain-0.1.9/langchain/tools/office365/create_draft_message.py
--rw-r--r--   0        0        0      164 2023-12-18 12:05:47.730216 gigachain-0.1.9/langchain/tools/office365/events_search.py
--rw-r--r--   0        0        0      166 2023-12-18 12:05:47.731158 gigachain-0.1.9/langchain/tools/office365/messages_search.py
--rw-r--r--   0        0        0      151 2023-12-18 12:05:47.732031 gigachain-0.1.9/langchain/tools/office365/send_event.py
--rw-r--r--   0        0        0      161 2023-12-18 12:05:47.732938 gigachain-0.1.9/langchain/tools/office365/send_message.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.933159 gigachain-0.1.9/langchain/tools/openapi/__init__.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.933535 gigachain-0.1.9/langchain/tools/openapi/utils/__init__.py
--rw-r--r--   0        0        0      542 2024-01-10 09:04:40.537910 gigachain-0.1.9/langchain/tools/openapi/utils/api_models.py
--rw-r--r--   0        0        0      191 2024-01-18 15:16:40.849295 gigachain-0.1.9/langchain/tools/openapi/utils/openapi_utils.py
--rw-r--r--   0        0        0      162 2024-01-18 15:16:40.852577 gigachain-0.1.9/langchain/tools/openweathermap/__init__.py
--rw-r--r--   0        0        0      119 2023-12-18 12:05:47.735667 gigachain-0.1.9/langchain/tools/openweathermap/tool.py
--rw-r--r--   0        0        0      763 2024-01-18 15:16:40.855894 gigachain-0.1.9/langchain/tools/playwright/__init__.py
--rw-r--r--   0        0        0      110 2024-01-10 09:04:40.538998 gigachain-0.1.9/langchain/tools/playwright/base.py
--rw-r--r--   0        0        0      124 2023-12-18 12:05:47.737713 gigachain-0.1.9/langchain/tools/playwright/click.py
--rw-r--r--   0        0        0      115 2023-12-18 12:05:47.738636 gigachain-0.1.9/langchain/tools/playwright/current_page.py
--rw-r--r--   0        0        0      198 2023-12-18 12:05:47.739546 gigachain-0.1.9/langchain/tools/playwright/extract_hyperlinks.py
--rw-r--r--   0        0        0      109 2023-12-18 12:05:47.740370 gigachain-0.1.9/langchain/tools/playwright/extract_text.py
--rw-r--r--   0        0        0      168 2024-01-10 09:04:40.540758 gigachain-0.1.9/langchain/tools/playwright/get_elements.py
--rw-r--r--   0        0        0      152 2023-12-18 12:05:47.741776 gigachain-0.1.9/langchain/tools/playwright/navigate.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:47.742595 gigachain-0.1.9/langchain/tools/playwright/navigate_back.py
--rw-r--r--   0        0        0      214 2024-01-10 09:04:40.541624 gigachain-0.1.9/langchain/tools/plugin.py
--rw-r--r--   0        0        0       52 2023-08-21 13:51:28.940033 gigachain-0.1.9/langchain/tools/powerbi/__init__.py
--rw-r--r--   0        0        0      189 2023-12-18 12:05:47.747546 gigachain-0.1.9/langchain/tools/powerbi/tool.py
--rw-r--r--   0        0        0       26 2023-08-21 13:51:28.941121 gigachain-0.1.9/langchain/tools/pubmed/__init__.py
--rw-r--r--   0        0        0       95 2023-12-18 12:05:47.748986 gigachain-0.1.9/langchain/tools/pubmed/tool.py
--rw-r--r--   0        0        0      512 2023-12-18 12:05:47.750576 gigachain-0.1.9/langchain/tools/python/__init__.py
--rw-r--r--   0        0        0        0 2024-01-10 09:04:40.541802 gigachain-0.1.9/langchain/tools/reddit_search/__init__.py
--rw-r--r--   0        0        0      159 2023-12-18 12:05:47.750982 gigachain-0.1.9/langchain/tools/reddit_search/tool.py
--rw-r--r--   0        0        0     1581 2024-02-22 08:54:03.338610 gigachain-0.1.9/langchain/tools/render.py
--rw-r--r--   0        0        0       52 2023-08-21 13:51:28.942395 gigachain-0.1.9/langchain/tools/requests/__init__.py
--rw-r--r--   0        0        0      349 2024-01-10 09:04:40.543130 gigachain-0.1.9/langchain/tools/requests/tool.py
--rw-r--r--   0        0        0     2494 2024-02-22 08:54:03.339522 gigachain-0.1.9/langchain/tools/retriever.py
--rw-r--r--   0        0        0       31 2023-08-21 13:51:28.943010 gigachain-0.1.9/langchain/tools/scenexplain/__init__.py
--rw-r--r--   0        0        0      140 2023-12-18 12:05:47.754166 gigachain-0.1.9/langchain/tools/scenexplain/tool.py
--rw-r--r--   0        0        0      214 2024-01-18 15:16:40.857082 gigachain-0.1.9/langchain/tools/searchapi/__init__.py
--rw-r--r--   0        0        0      132 2023-12-18 12:05:47.754976 gigachain-0.1.9/langchain/tools/searchapi/tool.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.943553 gigachain-0.1.9/langchain/tools/searx_search/__init__.py
--rw-r--r--   0        0        0      156 2023-12-18 12:05:47.756022 gigachain-0.1.9/langchain/tools/searx_search/tool.py
--rw-r--r--   0        0        0      103 2024-01-18 15:16:40.858323 gigachain-0.1.9/langchain/tools/shell/__init__.py
--rw-r--r--   0        0        0      123 2024-01-10 09:04:40.545873 gigachain-0.1.9/langchain/tools/shell/tool.py
--rw-r--r--   0        0        0      433 2024-01-18 15:16:40.859291 gigachain-0.1.9/langchain/tools/slack/__init__.py
--rw-r--r--   0        0        0       92 2023-12-18 12:05:47.757949 gigachain-0.1.9/langchain/tools/slack/base.py
--rw-r--r--   0        0        0      103 2023-12-18 12:05:47.758288 gigachain-0.1.9/langchain/tools/slack/get_channel.py
--rw-r--r--   0        0        0      164 2023-12-18 12:05:47.758614 gigachain-0.1.9/langchain/tools/slack/get_message.py
--rw-r--r--   0        0        0      179 2023-12-18 12:05:47.758964 gigachain-0.1.9/langchain/tools/slack/schedule_message.py
--rw-r--r--   0        0        0      159 2023-12-18 12:05:47.759577 gigachain-0.1.9/langchain/tools/slack/send_message.py
--rw-r--r--   0        0        0       18 2023-08-21 13:51:28.944873 gigachain-0.1.9/langchain/tools/sleep/__init__.py
--rw-r--r--   0        0        0      110 2023-12-18 12:05:47.760887 gigachain-0.1.9/langchain/tools/sleep/tool.py
--rw-r--r--   0        0        0       44 2023-08-21 13:51:28.945531 gigachain-0.1.9/langchain/tools/spark_sql/__init__.py
--rw-r--r--   0        0        0      304 2023-12-18 12:05:47.762602 gigachain-0.1.9/langchain/tools/spark_sql/tool.py
--rw-r--r--   0        0        0       49 2023-08-21 13:51:28.946602 gigachain-0.1.9/langchain/tools/sql_database/__init__.py
--rw-r--r--   0        0        0      101 2023-12-18 12:05:47.763764 gigachain-0.1.9/langchain/tools/sql_database/prompt.py
--rw-r--r--   0        0        0      337 2023-12-18 12:05:47.764601 gigachain-0.1.9/langchain/tools/sql_database/tool.py
--rw-r--r--   0        0        0       33 2023-12-18 12:05:47.764989 gigachain-0.1.9/langchain/tools/stackexchange/__init__.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:47.765358 gigachain-0.1.9/langchain/tools/stackexchange/tool.py
--rw-r--r--   0        0        0       24 2023-12-18 12:05:47.765850 gigachain-0.1.9/langchain/tools/steam/__init__.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:47.766652 gigachain-0.1.9/langchain/tools/steam/tool.py
--rw-r--r--   0        0        0      186 2024-01-18 15:16:40.861528 gigachain-0.1.9/langchain/tools/steamship_image_generation/__init__.py
--rw-r--r--   0        0        0      180 2024-01-10 09:04:40.549946 gigachain-0.1.9/langchain/tools/steamship_image_generation/tool.py
--rw-r--r--   0        0        0      189 2024-01-18 15:16:40.863373 gigachain-0.1.9/langchain/tools/tavily_search/__init__.py
--rw-r--r--   0        0        0      187 2023-12-18 12:05:47.769298 gigachain-0.1.9/langchain/tools/tavily_search/tool.py
--rw-r--r--   0        0        0       51 2023-08-21 13:51:28.948611 gigachain-0.1.9/langchain/tools/vectorstore/__init__.py
--rw-r--r--   0        0        0      192 2024-01-10 09:04:40.550932 gigachain-0.1.9/langchain/tools/vectorstore/tool.py
--rw-r--r--   0        0        0       29 2023-08-21 13:51:28.949334 gigachain-0.1.9/langchain/tools/wikipedia/__init__.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:47.770933 gigachain-0.1.9/langchain/tools/wikipedia/tool.py
--rw-r--r--   0        0        0      156 2024-01-18 15:16:40.865406 gigachain-0.1.9/langchain/tools/wolfram_alpha/__init__.py
--rw-r--r--   0        0        0      114 2023-12-18 12:05:47.772046 gigachain-0.1.9/langchain/tools/wolfram_alpha/tool.py
--rw-r--r--   0        0        0      114 2023-12-18 12:05:47.772808 gigachain-0.1.9/langchain/tools/yahoo_finance_news.py
--rw-r--r--   0        0        0        0 2023-08-21 13:51:28.950523 gigachain-0.1.9/langchain/tools/youtube/__init__.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:47.773642 gigachain-0.1.9/langchain/tools/youtube/search.py
--rw-r--r--   0        0        0      193 2024-01-18 15:16:40.866803 gigachain-0.1.9/langchain/tools/zapier/__init__.py
--rw-r--r--   0        0        0      162 2023-12-18 12:05:47.775875 gigachain-0.1.9/langchain/tools/zapier/tool.py
--rw-r--r--   0        0        0     2327 2024-02-22 08:54:03.342679 gigachain-0.1.9/langchain/utilities/__init__.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.777546 gigachain-0.1.9/langchain/utilities/alpha_vantage.py
--rw-r--r--   0        0        0      193 2024-01-10 09:04:40.553326 gigachain-0.1.9/langchain/utilities/anthropic.py
--rw-r--r--   0        0        0       89 2023-12-18 12:05:47.779550 gigachain-0.1.9/langchain/utilities/apify.py
--rw-r--r--   0        0        0      361 2023-12-18 12:05:47.780643 gigachain-0.1.9/langchain/utilities/arcee.py
--rw-r--r--   0        0        0       95 2023-12-18 12:05:47.781484 gigachain-0.1.9/langchain/utilities/arxiv.py
--rw-r--r--   0        0        0      274 2023-08-21 13:51:28.954857 gigachain-0.1.9/langchain/utilities/asyncio.py
--rw-r--r--   0        0        0       95 2023-12-18 12:05:47.782588 gigachain-0.1.9/langchain/utilities/awslambda.py
--rw-r--r--   0        0        0      104 2024-01-10 09:04:40.554292 gigachain-0.1.9/langchain/utilities/bibtex.py
--rw-r--r--   0        0        0      111 2023-12-18 12:05:47.784354 gigachain-0.1.9/langchain/utilities/bing_search.py
--rw-r--r--   0        0        0      108 2023-12-18 12:05:47.785090 gigachain-0.1.9/langchain/utilities/brave_search.py
--rw-r--r--   0        0        0      269 2024-01-10 09:04:40.555397 gigachain-0.1.9/langchain/utilities/clickup.py
--rw-r--r--   0        0        0      111 2023-12-18 12:05:47.786400 gigachain-0.1.9/langchain/utilities/dalle_image_generator.py
--rw-r--r--   0        0        0      121 2023-12-18 12:05:47.787554 gigachain-0.1.9/langchain/utilities/dataforseo_api_search.py
--rw-r--r--   0        0        0      129 2023-12-18 12:05:47.788355 gigachain-0.1.9/langchain/utilities/duckduckgo_search.py
--rw-r--r--   0        0        0       98 2024-01-10 09:04:40.556303 gigachain-0.1.9/langchain/utilities/github.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.789907 gigachain-0.1.9/langchain/utilities/gitlab.py
--rw-r--r--   0        0        0      123 2024-01-10 09:04:40.557288 gigachain-0.1.9/langchain/utilities/golden_query.py
--rw-r--r--   0        0        0      120 2023-12-18 12:05:47.790928 gigachain-0.1.9/langchain/utilities/google_finance.py
--rw-r--r--   0        0        0      111 2023-12-18 12:05:47.791487 gigachain-0.1.9/langchain/utilities/google_jobs.py
--rw-r--r--   0        0        0      111 2023-12-18 12:05:47.791854 gigachain-0.1.9/langchain/utilities/google_lens.py
--rw-r--r--   0        0        0      121 2023-12-18 12:05:47.792836 gigachain-0.1.9/langchain/utilities/google_places_api.py
--rw-r--r--   0        0        0      120 2023-12-18 12:05:47.793660 gigachain-0.1.9/langchain/utilities/google_scholar.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.794263 gigachain-0.1.9/langchain/utilities/google_search.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.794850 gigachain-0.1.9/langchain/utilities/google_serper.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.795198 gigachain-0.1.9/langchain/utilities/google_trends.py
--rw-r--r--   0        0        0      101 2023-12-18 12:05:47.796297 gigachain-0.1.9/langchain/utilities/graphql.py
--rw-r--r--   0        0        0       92 2023-12-18 12:05:47.797166 gigachain-0.1.9/langchain/utilities/jira.py
--rw-r--r--   0        0        0      122 2023-12-18 12:05:47.798009 gigachain-0.1.9/langchain/utilities/loading.py
--rw-r--r--   0        0        0      111 2023-12-18 12:05:47.798917 gigachain-0.1.9/langchain/utilities/max_compute.py
--rw-r--r--   0        0        0      139 2024-01-10 09:04:40.558668 gigachain-0.1.9/langchain/utilities/merriam_webster.py
--rw-r--r--   0        0        0      132 2024-01-10 09:04:40.559696 gigachain-0.1.9/langchain/utilities/metaphor_search.py
--rw-r--r--   0        0        0      101 2024-01-10 09:04:40.560501 gigachain-0.1.9/langchain/utilities/nasa.py
--rw-r--r--   0        0        0      115 2023-12-18 12:05:47.801862 gigachain-0.1.9/langchain/utilities/opaqueprompts.py
--rw-r--r--   0        0        0      111 2023-12-18 12:05:47.803267 gigachain-0.1.9/langchain/utilities/openapi.py
--rw-r--r--   0        0        0      122 2023-12-18 12:05:47.804229 gigachain-0.1.9/langchain/utilities/openweathermap.py
--rw-r--r--   0        0        0      110 2024-01-10 09:04:40.562773 gigachain-0.1.9/langchain/utilities/outline.py
--rw-r--r--   0        0        0       81 2023-12-18 12:05:47.805758 gigachain-0.1.9/langchain/utilities/portkey.py
--rw-r--r--   0        0        0      111 2024-01-10 09:04:40.563881 gigachain-0.1.9/langchain/utilities/powerbi.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.807428 gigachain-0.1.9/langchain/utilities/pubmed.py
--rw-r--r--   0        0        0       86 2024-01-10 09:04:40.566650 gigachain-0.1.9/langchain/utilities/python.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.808570 gigachain-0.1.9/langchain/utilities/reddit_search.py
--rw-r--r--   0        0        0      201 2024-01-10 09:04:40.567678 gigachain-0.1.9/langchain/utilities/redis.py
--rw-r--r--   0        0        0      181 2023-12-18 12:05:47.810729 gigachain-0.1.9/langchain/utilities/requests.py
--rw-r--r--   0        0        0      113 2023-12-18 12:05:47.811895 gigachain-0.1.9/langchain/utilities/scenexplain.py
--rw-r--r--   0        0        0      107 2023-12-18 12:05:47.812573 gigachain-0.1.9/langchain/utilities/searchapi.py
--rw-r--r--   0        0        0      151 2024-01-10 09:04:40.568799 gigachain-0.1.9/langchain/utilities/searx_search.py
--rw-r--r--   0        0        0      125 2023-12-18 12:05:47.814336 gigachain-0.1.9/langchain/utilities/serpapi.py
--rw-r--r--   0        0        0       85 2023-12-18 12:05:47.815076 gigachain-0.1.9/langchain/utilities/spark_sql.py
--rw-r--r--   0        0        0      139 2024-01-10 09:04:40.570370 gigachain-0.1.9/langchain/utilities/sql_database.py
--rw-r--r--   0        0        0      119 2023-12-18 12:05:47.816263 gigachain-0.1.9/langchain/utilities/stackexchange.py
--rw-r--r--   0        0        0      101 2023-12-18 12:05:47.816643 gigachain-0.1.9/langchain/utilities/steam.py
--rw-r--r--   0        0        0      126 2024-01-10 09:04:40.571469 gigachain-0.1.9/langchain/utilities/tavily_search.py
--rw-r--r--   0        0        0      115 2023-12-18 12:05:47.818236 gigachain-0.1.9/langchain/utilities/tensorflow_datasets.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.819464 gigachain-0.1.9/langchain/utilities/twilio.py
--rw-r--r--   0        0        0      276 2023-12-18 12:05:47.820326 gigachain-0.1.9/langchain/utilities/vertexai.py
--rw-r--r--   0        0        0      116 2024-01-10 09:04:40.572515 gigachain-0.1.9/langchain/utilities/wikipedia.py
--rw-r--r--   0        0        0      117 2023-12-18 12:05:47.822016 gigachain-0.1.9/langchain/utilities/wolfram_alpha.py
--rw-r--r--   0        0        0       98 2023-12-18 12:05:47.823234 gigachain-0.1.9/langchain/utilities/zapier.py
--rw-r--r--   0        0        0     1221 2023-12-18 12:05:47.824245 gigachain-0.1.9/langchain/utils/__init__.py
--rw-r--r--   0        0        0      102 2023-12-18 12:05:47.825271 gigachain-0.1.9/langchain/utils/aiter.py
--rw-r--r--   0        0        0      124 2023-12-18 12:05:47.826109 gigachain-0.1.9/langchain/utils/env.py
--rw-r--r--   0        0        0      325 2024-01-18 15:16:40.869253 gigachain-0.1.9/langchain/utils/ernie_functions.py
--rw-r--r--   0        0        0       91 2023-12-18 12:05:47.827383 gigachain-0.1.9/langchain/utils/formatting.py
--rw-r--r--   0        0        0      421 2023-12-18 12:05:47.828299 gigachain-0.1.9/langchain/utils/html.py
--rw-r--r--   0        0        0      211 2023-12-18 12:05:47.829085 gigachain-0.1.9/langchain/utils/input.py
--rw-r--r--   0        0        0      139 2024-01-18 15:16:40.869655 gigachain-0.1.9/langchain/utils/interactive_env.py
--rw-r--r--   0        0        0      133 2023-12-18 12:05:47.829865 gigachain-0.1.9/langchain/utils/iter.py
--rw-r--r--   0        0        0      258 2023-12-18 12:05:47.830615 gigachain-0.1.9/langchain/utils/json_schema.py
--rw-r--r--   0        0        0       92 2023-12-18 12:05:47.831372 gigachain-0.1.9/langchain/utils/loading.py
--rw-r--r--   0        0        0      181 2023-12-18 12:05:47.832276 gigachain-0.1.9/langchain/utils/math.py
--rw-r--r--   0        0        0       86 2023-12-18 12:05:47.833389 gigachain-0.1.9/langchain/utils/openai.py
--rw-r--r--   0        0        0      330 2023-12-18 12:05:47.834161 gigachain-0.1.9/langchain/utils/openai_functions.py
--rw-r--r--   0        0        0      111 2023-12-18 12:05:47.835107 gigachain-0.1.9/langchain/utils/pydantic.py
--rw-r--r--   0        0        0      148 2023-12-18 12:05:47.835836 gigachain-0.1.9/langchain/utils/strings.py
--rw-r--r--   0        0        0      446 2023-12-18 12:05:47.836793 gigachain-0.1.9/langchain/utils/utils.py
--rw-r--r--   0        0        0     2768 2024-02-22 08:54:03.345759 gigachain-0.1.9/langchain/vectorstores/__init__.py
--rw-r--r--   0        0        0      220 2024-01-10 09:04:40.575258 gigachain-0.1.9/langchain/vectorstores/alibabacloud_opensearch.py
--rw-r--r--   0        0        0      109 2024-01-10 09:04:40.576760 gigachain-0.1.9/langchain/vectorstores/analyticdb.py
--rw-r--r--   0        0        0       87 2024-01-10 09:04:40.580566 gigachain-0.1.9/langchain/vectorstores/annoy.py
--rw-r--r--   0        0        0      100 2024-01-10 09:04:40.583665 gigachain-0.1.9/langchain/vectorstores/astradb.py
--rw-r--r--   0        0        0       82 2023-12-18 12:05:47.842405 gigachain-0.1.9/langchain/vectorstores/atlas.py
--rw-r--r--   0        0        0       78 2024-01-10 09:04:40.584957 gigachain-0.1.9/langchain/vectorstores/awadb.py
--rw-r--r--   0        0        0      256 2024-01-10 09:04:40.586040 gigachain-0.1.9/langchain/vectorstores/azure_cosmos_db.py
--rw-r--r--   0        0        0      188 2024-01-10 09:04:40.587676 gigachain-0.1.9/langchain/vectorstores/azuresearch.py
--rw-r--r--   0        0        0       89 2024-01-10 09:04:40.589288 gigachain-0.1.9/langchain/vectorstores/bageldb.py
--rw-r--r--   0        0        0      115 2023-12-18 12:05:47.846640 gigachain-0.1.9/langchain/vectorstores/baiducloud_vector_search.py
--rw-r--r--   0        0        0      125 2023-12-18 12:05:47.847689 gigachain-0.1.9/langchain/vectorstores/base.py
--rw-r--r--   0        0        0      104 2023-12-18 12:05:47.848672 gigachain-0.1.9/langchain/vectorstores/cassandra.py
--rw-r--r--   0        0        0       90 2024-01-10 09:04:40.590074 gigachain-0.1.9/langchain/vectorstores/chroma.py
--rw-r--r--   0        0        0       87 2023-12-18 12:05:47.850266 gigachain-0.1.9/langchain/vectorstores/clarifai.py
--rw-r--r--   0        0        0      148 2024-01-10 09:04:40.590843 gigachain-0.1.9/langchain/vectorstores/clickhouse.py
--rw-r--r--   0        0        0       93 2023-12-18 12:05:47.852012 gigachain-0.1.9/langchain/vectorstores/dashvector.py
--rw-r--r--   0        0        0      140 2023-12-18 12:05:47.852481 gigachain-0.1.9/langchain/vectorstores/databricks_vector_search.py
--rw-r--r--   0        0        0       87 2023-12-18 12:05:47.853219 gigachain-0.1.9/langchain/vectorstores/deeplake.py
--rw-r--r--   0        0        0       78 2023-12-18 12:05:47.854024 gigachain-0.1.9/langchain/vectorstores/dingo.py
--rw-r--r--   0        0        0      236 2024-01-18 15:16:40.872866 gigachain-0.1.9/langchain/vectorstores/docarray/__init__.py
--rw-r--r--   0        0        0      111 2024-01-10 09:04:40.591768 gigachain-0.1.9/langchain/vectorstores/docarray/base.py
--rw-r--r--   0        0        0      112 2023-12-18 12:05:47.859528 gigachain-0.1.9/langchain/vectorstores/docarray/hnsw.py
--rw-r--r--   0        0        0      125 2023-12-18 12:05:47.860361 gigachain-0.1.9/langchain/vectorstores/docarray/in_memory.py
--rw-r--r--   0        0        0      184 2024-01-10 09:04:40.593248 gigachain-0.1.9/langchain/vectorstores/elastic_vector_search.py
--rw-r--r--   0        0        0      362 2023-12-18 12:05:47.862557 gigachain-0.1.9/langchain/vectorstores/elasticsearch.py
--rw-r--r--   0        0        0       84 2023-12-18 12:05:47.863374 gigachain-0.1.9/langchain/vectorstores/epsilla.py
--rw-r--r--   0        0        0       87 2024-01-10 09:04:40.594436 gigachain-0.1.9/langchain/vectorstores/faiss.py
--rw-r--r--   0        0        0       78 2024-01-10 09:04:40.595403 gigachain-0.1.9/langchain/vectorstores/hippo.py
--rw-r--r--   0        0        0       96 2024-01-10 09:04:40.596341 gigachain-0.1.9/langchain/vectorstores/hologres.py
--rw-r--r--   0        0        0       84 2023-12-18 12:05:47.867322 gigachain-0.1.9/langchain/vectorstores/lancedb.py
--rw-r--r--   0        0        0      128 2023-12-18 12:05:47.868167 gigachain-0.1.9/langchain/vectorstores/llm_rails.py
--rw-r--r--   0        0        0       78 2023-12-18 12:05:47.869093 gigachain-0.1.9/langchain/vectorstores/marqo.py
--rw-r--r--   0        0        0      106 2023-12-18 12:05:47.870058 gigachain-0.1.9/langchain/vectorstores/matching_engine.py
--rw-r--r--   0        0        0       96 2024-01-10 09:04:40.597226 gigachain-0.1.9/langchain/vectorstores/meilisearch.py
--rw-r--r--   0        0        0       81 2024-01-10 09:04:40.599173 gigachain-0.1.9/langchain/vectorstores/milvus.py
--rw-r--r--   0        0        0      128 2024-01-10 09:04:40.600394 gigachain-0.1.9/langchain/vectorstores/momento_vector_index.py
--rw-r--r--   0        0        0      192 2024-01-10 09:04:40.601389 gigachain-0.1.9/langchain/vectorstores/mongodb_atlas.py
--rw-r--r--   0        0        0      179 2024-01-10 09:04:40.602397 gigachain-0.1.9/langchain/vectorstores/myscale.py
--rw-r--r--   0        0        0      147 2024-01-10 09:04:40.603441 gigachain-0.1.9/langchain/vectorstores/neo4j_vector.py
--rw-r--r--   0        0        0       87 2024-01-10 09:04:40.604618 gigachain-0.1.9/langchain/vectorstores/nucliadb.py
--rw-r--r--   0        0        0      147 2024-01-10 09:04:40.605556 gigachain-0.1.9/langchain/vectorstores/opensearch_vector_search.py
--rw-r--r--   0        0        0      234 2024-01-10 09:04:40.607685 gigachain-0.1.9/langchain/vectorstores/pgembedding.py
--rw-r--r--   0        0        0       93 2024-01-10 09:04:40.608761 gigachain-0.1.9/langchain/vectorstores/pgvecto_rs.py
--rw-r--r--   0        0        0      149 2024-01-10 09:04:40.609389 gigachain-0.1.9/langchain/vectorstores/pgvector.py
--rw-r--r--   0        0        0       87 2023-12-18 12:05:47.880186 gigachain-0.1.9/langchain/vectorstores/pinecone.py
--rw-r--r--   0        0        0      130 2024-01-10 09:04:40.610308 gigachain-0.1.9/langchain/vectorstores/qdrant.py
--rw-r--r--   0        0        0      265 2023-09-12 10:52:10.695398 gigachain-0.1.9/langchain/vectorstores/redis/__init__.py
--rw-r--r--   0        0        0      213 2024-01-10 09:04:40.611387 gigachain-0.1.9/langchain/vectorstores/redis/base.py
--rw-r--r--   0        0        0      416 2023-12-18 12:05:47.884194 gigachain-0.1.9/langchain/vectorstores/redis/filters.py
--rw-r--r--   0        0        0      503 2023-12-18 12:05:47.885024 gigachain-0.1.9/langchain/vectorstores/redis/schema.py
--rw-r--r--   0        0        0       86 2023-12-18 12:05:47.885729 gigachain-0.1.9/langchain/vectorstores/rocksetdb.py
--rw-r--r--   0        0        0       87 2024-01-10 09:04:40.612428 gigachain-0.1.9/langchain/vectorstores/scann.py
--rw-r--r--   0        0        0       81 2023-12-18 12:05:47.887513 gigachain-0.1.9/langchain/vectorstores/semadb.py
--rw-r--r--   0        0        0      165 2024-01-10 09:04:40.613481 gigachain-0.1.9/langchain/vectorstores/singlestoredb.py
--rw-r--r--   0        0        0      364 2024-01-10 09:04:40.614368 gigachain-0.1.9/langchain/vectorstores/sklearn.py
--rw-r--r--   0        0        0       90 2023-12-18 12:05:47.889663 gigachain-0.1.9/langchain/vectorstores/sqlitevss.py
--rw-r--r--   0        0        0      154 2024-01-10 09:04:40.617741 gigachain-0.1.9/langchain/vectorstores/starrocks.py
--rw-r--r--   0        0        0      109 2023-12-18 12:05:47.891235 gigachain-0.1.9/langchain/vectorstores/supabase.py
--rw-r--r--   0        0        0       75 2024-01-10 09:04:40.620407 gigachain-0.1.9/langchain/vectorstores/tair.py
--rw-r--r--   0        0        0      191 2023-12-18 12:05:47.893009 gigachain-0.1.9/langchain/vectorstores/tencentvectordb.py
--rw-r--r--   0        0        0       81 2023-12-18 12:05:47.893937 gigachain-0.1.9/langchain/vectorstores/tigris.py
--rw-r--r--   0        0        0       97 2024-01-10 09:04:40.621429 gigachain-0.1.9/langchain/vectorstores/tiledb.py
--rw-r--r--   0        0        0      124 2024-01-10 09:04:40.622500 gigachain-0.1.9/langchain/vectorstores/timescalevector.py
--rw-r--r--   0        0        0       90 2023-12-18 12:05:47.896743 gigachain-0.1.9/langchain/vectorstores/typesense.py
--rw-r--r--   0        0        0       84 2024-01-10 09:04:40.623762 gigachain-0.1.9/langchain/vectorstores/usearch.py
--rw-r--r--   0        0        0      227 2023-12-18 12:05:47.898744 gigachain-0.1.9/langchain/vectorstores/utils.py
--rw-r--r--   0        0        0       75 2023-12-18 12:05:47.899754 gigachain-0.1.9/langchain/vectorstores/vald.py
--rw-r--r--   0        0        0       81 2024-01-10 09:04:40.624717 gigachain-0.1.9/langchain/vectorstores/vearch.py
--rw-r--r--   0        0        0      122 2023-12-18 12:05:47.901403 gigachain-0.1.9/langchain/vectorstores/vectara.py
--rw-r--r--   0        0        0       88 2023-12-18 12:05:47.902340 gigachain-0.1.9/langchain/vectorstores/vespa.py
--rw-r--r--   0        0        0      103 2024-01-10 09:04:40.625644 gigachain-0.1.9/langchain/vectorstores/weaviate.py
--rw-r--r--   0        0        0       97 2023-12-18 12:05:47.904061 gigachain-0.1.9/langchain/vectorstores/xata.py
--rw-r--r--   0        0        0       96 2023-12-18 12:05:47.904403 gigachain-0.1.9/langchain/vectorstores/yellowbrick.py
--rw-r--r--   0        0        0      132 2023-12-18 12:05:47.905433 gigachain-0.1.9/langchain/vectorstores/zep.py
--rw-r--r--   0        0        0       81 2023-12-18 12:05:47.906395 gigachain-0.1.9/langchain/vectorstores/zilliz.py
--rw-r--r--   0        0        0    11751 2024-03-01 11:50:11.652206 gigachain-0.1.9/pyproject.toml
--rw-r--r--   0        0        0    13972 1970-01-01 00:00:00.000000 gigachain-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-11-15 10:30:09.324245 gigachain-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5778 2024-04-19 07:38:33.866596 gigachain-0.2.0/README.md
+-rw-r--r--   0        0        0    13990 2024-05-24 11:13:19.190487 gigachain-0.2.0/langchain/__init__.py
+-rw-r--r--   0        0        0      733 2024-05-06 14:45:38.407301 gigachain-0.2.0/langchain/_api/__init__.py
+-rw-r--r--   0        0        0      471 2023-12-18 12:05:46.810499 gigachain-0.2.0/langchain/_api/deprecation.py
+-rw-r--r--   0        0        0      139 2024-05-06 14:45:39.438596 gigachain-0.2.0/langchain/_api/interactive_env.py
+-rw-r--r--   0        0        0     6746 2024-05-24 11:13:19.191195 gigachain-0.2.0/langchain/_api/module_import.py
+-rw-r--r--   0        0        0      122 2023-12-18 12:05:46.811728 gigachain-0.2.0/langchain/_api/path.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.531593 gigachain-0.2.0/langchain/adapters/__init__.py
+-rw-r--r--   0        0        0     1996 2024-05-06 14:45:38.408832 gigachain-0.2.0/langchain/adapters/openai.py
+-rw-r--r--   0        0        0     6381 2024-05-06 14:45:38.410191 gigachain-0.2.0/langchain/agents/__init__.py
+-rw-r--r--   0        0        0    56780 2024-05-24 11:13:19.193542 gigachain-0.2.0/langchain/agents/agent.py
+-rw-r--r--   0        0        0    15302 2024-05-24 11:13:19.194970 gigachain-0.2.0/langchain/agents/agent_iterator.py
+-rw-r--r--   0        0        0     7364 2024-05-06 14:45:38.411427 gigachain-0.2.0/langchain/agents/agent_toolkits/__init__.py
+-rw-r--r--   0        0        0       25 2023-08-24 07:36:02.856871 gigachain-0.2.0/langchain/agents/agent_toolkits/ainetwork/__init__.py
+-rw-r--r--   0        0        0      685 2024-05-06 14:45:38.412100 gigachain-0.2.0/langchain/agents/agent_toolkits/ainetwork/toolkit.py
+-rw-r--r--   0        0        0      668 2024-05-06 14:45:38.412756 gigachain-0.2.0/langchain/agents/agent_toolkits/amadeus/toolkit.py
+-rw-r--r--   0        0        0      771 2024-05-06 14:45:38.413380 gigachain-0.2.0/langchain/agents/agent_toolkits/azure_cognitive_services.py
+-rw-r--r--   0        0        0       72 2024-05-06 14:45:38.413845 gigachain-0.2.0/langchain/agents/agent_toolkits/base.py
+-rw-r--r--   0        0        0        0 2023-10-06 14:43:01.368502 gigachain-0.2.0/langchain/agents/agent_toolkits/clickup/__init__.py
+-rw-r--r--   0        0        0      675 2024-05-06 14:45:38.414397 gigachain-0.2.0/langchain/agents/agent_toolkits/clickup/toolkit.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.534160 gigachain-0.2.0/langchain/agents/agent_toolkits/conversational_retrieval/__init__.py
+-rw-r--r--   0        0        0     3235 2024-05-06 14:45:38.414986 gigachain-0.2.0/langchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py
+-rw-r--r--   0        0        0       97 2023-10-30 16:05:53.823759 gigachain-0.2.0/langchain/agents/agent_toolkits/conversational_retrieval/tool.py
+-rw-r--r--   0        0        0     1091 2023-12-18 12:05:46.831119 gigachain-0.2.0/langchain/agents/agent_toolkits/csv/__init__.py
+-rw-r--r--   0        0        0      782 2024-05-06 14:45:38.415584 gigachain-0.2.0/langchain/agents/agent_toolkits/file_management/__init__.py
+-rw-r--r--   0        0        0      745 2024-05-06 14:45:38.416075 gigachain-0.2.0/langchain/agents/agent_toolkits/file_management/toolkit.py
+-rw-r--r--   0        0        0       22 2023-08-21 13:51:28.536932 gigachain-0.2.0/langchain/agents/agent_toolkits/github/__init__.py
+-rw-r--r--   0        0        0     2244 2024-05-06 14:45:38.416565 gigachain-0.2.0/langchain/agents/agent_toolkits/github/toolkit.py
+-rw-r--r--   0        0        0       22 2023-09-19 14:33:02.213182 gigachain-0.2.0/langchain/agents/agent_toolkits/gitlab/__init__.py
+-rw-r--r--   0        0        0      670 2024-05-06 14:45:38.417256 gigachain-0.2.0/langchain/agents/agent_toolkits/gitlab/toolkit.py
+-rw-r--r--   0        0        0       21 2023-08-21 13:51:28.537602 gigachain-0.2.0/langchain/agents/agent_toolkits/gmail/__init__.py
+-rw-r--r--   0        0        0      659 2024-05-06 14:45:38.417980 gigachain-0.2.0/langchain/agents/agent_toolkits/gmail/toolkit.py
+-rw-r--r--   0        0        0       20 2023-08-21 13:51:28.538134 gigachain-0.2.0/langchain/agents/agent_toolkits/jira/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-06 14:45:38.418585 gigachain-0.2.0/langchain/agents/agent_toolkits/jira/toolkit.py
+-rw-r--r--   0        0        0       18 2023-08-21 13:51:28.538568 gigachain-0.2.0/langchain/agents/agent_toolkits/json/__init__.py
+-rw-r--r--   0        0        0      672 2024-05-06 14:45:38.419163 gigachain-0.2.0/langchain/agents/agent_toolkits/json/base.py
+-rw-r--r--   0        0        0      749 2024-05-06 14:45:38.419678 gigachain-0.2.0/langchain/agents/agent_toolkits/json/prompt.py
+-rw-r--r--   0        0        0      654 2024-05-06 14:45:38.420214 gigachain-0.2.0/langchain/agents/agent_toolkits/json/toolkit.py
+-rw-r--r--   0        0        0       23 2023-08-21 13:51:28.539651 gigachain-0.2.0/langchain/agents/agent_toolkits/multion/__init__.py
+-rw-r--r--   0        0        0      675 2024-05-06 14:45:38.420845 gigachain-0.2.0/langchain/agents/agent_toolkits/multion/toolkit.py
+-rw-r--r--   0        0        0       19 2023-12-18 12:05:46.842756 gigachain-0.2.0/langchain/agents/agent_toolkits/nasa/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-06 14:45:38.421464 gigachain-0.2.0/langchain/agents/agent_toolkits/nasa/toolkit.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.540099 gigachain-0.2.0/langchain/agents/agent_toolkits/nla/__init__.py
+-rw-r--r--   0        0        0      634 2024-05-06 14:45:38.422133 gigachain-0.2.0/langchain/agents/agent_toolkits/nla/tool.py
+-rw-r--r--   0        0        0      649 2024-05-06 14:45:38.422743 gigachain-0.2.0/langchain/agents/agent_toolkits/nla/toolkit.py
+-rw-r--r--   0        0        0       25 2023-08-21 13:51:28.541150 gigachain-0.2.0/langchain/agents/agent_toolkits/office365/__init__.py
+-rw-r--r--   0        0        0      670 2024-05-06 14:45:38.423356 gigachain-0.2.0/langchain/agents/agent_toolkits/office365/toolkit.py
+-rw-r--r--   0        0        0       26 2023-08-21 13:51:28.541736 gigachain-0.2.0/langchain/agents/agent_toolkits/openapi/__init__.py
+-rw-r--r--   0        0        0      687 2024-05-06 14:45:38.424067 gigachain-0.2.0/langchain/agents/agent_toolkits/openapi/base.py
+-rw-r--r--   0        0        0     1599 2024-05-06 14:45:38.424593 gigachain-0.2.0/langchain/agents/agent_toolkits/openapi/planner.py
+-rw-r--r--   0        0        0     3526 2024-05-06 14:45:38.425114 gigachain-0.2.0/langchain/agents/agent_toolkits/openapi/planner_prompt.py
+-rw-r--r--   0        0        0      909 2024-05-06 14:45:38.425565 gigachain-0.2.0/langchain/agents/agent_toolkits/openapi/prompt.py
+-rw-r--r--   0        0        0      833 2024-05-06 14:45:38.425993 gigachain-0.2.0/langchain/agents/agent_toolkits/openapi/spec.py
+-rw-r--r--   0        0        0      818 2024-05-06 14:45:38.426419 gigachain-0.2.0/langchain/agents/agent_toolkits/openapi/toolkit.py
+-rw-r--r--   0        0        0     1104 2023-12-18 12:05:46.851835 gigachain-0.2.0/langchain/agents/agent_toolkits/pandas/__init__.py
+-rw-r--r--   0        0        0      762 2024-05-06 14:45:38.426964 gigachain-0.2.0/langchain/agents/agent_toolkits/playwright/__init__.py
+-rw-r--r--   0        0        0      728 2024-05-06 14:45:38.427463 gigachain-0.2.0/langchain/agents/agent_toolkits/playwright/toolkit.py
+-rw-r--r--   0        0        0       22 2023-08-21 13:51:28.545958 gigachain-0.2.0/langchain/agents/agent_toolkits/powerbi/__init__.py
+-rw-r--r--   0        0        0      675 2024-05-06 14:45:38.427914 gigachain-0.2.0/langchain/agents/agent_toolkits/powerbi/base.py
+-rw-r--r--   0        0        0      717 2024-05-06 14:45:38.428556 gigachain-0.2.0/langchain/agents/agent_toolkits/powerbi/chat_base.py
+-rw-r--r--   0        0        0     1084 2024-05-06 14:45:38.429045 gigachain-0.2.0/langchain/agents/agent_toolkits/powerbi/prompt.py
+-rw-r--r--   0        0        0      675 2024-05-06 14:45:38.429478 gigachain-0.2.0/langchain/agents/agent_toolkits/powerbi/toolkit.py
+-rw-r--r--   0        0        0     1094 2023-12-18 12:05:46.857872 gigachain-0.2.0/langchain/agents/agent_toolkits/python/__init__.py
+-rw-r--r--   0        0        0       21 2023-12-18 12:05:46.858297 gigachain-0.2.0/langchain/agents/agent_toolkits/slack/__init__.py
+-rw-r--r--   0        0        0      659 2024-05-06 14:45:38.429905 gigachain-0.2.0/langchain/agents/agent_toolkits/slack/toolkit.py
+-rw-r--r--   0        0        0     1103 2023-12-18 12:05:46.860134 gigachain-0.2.0/langchain/agents/agent_toolkits/spark/__init__.py
+-rw-r--r--   0        0        0       23 2023-08-21 13:51:28.548199 gigachain-0.2.0/langchain/agents/agent_toolkits/spark_sql/__init__.py
+-rw-r--r--   0        0        0      697 2024-05-06 14:45:38.430311 gigachain-0.2.0/langchain/agents/agent_toolkits/spark_sql/base.py
+-rw-r--r--   0        0        0      783 2024-05-06 14:45:38.430706 gigachain-0.2.0/langchain/agents/agent_toolkits/spark_sql/prompt.py
+-rw-r--r--   0        0        0      682 2024-05-06 14:45:38.431036 gigachain-0.2.0/langchain/agents/agent_toolkits/spark_sql/toolkit.py
+-rw-r--r--   0        0        0       17 2023-08-21 13:51:28.549117 gigachain-0.2.0/langchain/agents/agent_toolkits/sql/__init__.py
+-rw-r--r--   0        0        0      661 2024-05-06 14:45:38.431586 gigachain-0.2.0/langchain/agents/agent_toolkits/sql/base.py
+-rw-r--r--   0        0        0      896 2024-05-06 14:45:38.431954 gigachain-0.2.0/langchain/agents/agent_toolkits/sql/prompt.py
+-rw-r--r--   0        0        0      679 2024-05-06 14:45:38.432470 gigachain-0.2.0/langchain/agents/agent_toolkits/sql/toolkit.py
+-rw-r--r--   0        0        0       21 2023-12-18 12:05:46.867144 gigachain-0.2.0/langchain/agents/agent_toolkits/steam/__init__.py
+-rw-r--r--   0        0        0      659 2024-05-06 14:45:38.432901 gigachain-0.2.0/langchain/agents/agent_toolkits/steam/toolkit.py
+-rw-r--r--   0        0        0       56 2023-08-21 13:51:28.549949 gigachain-0.2.0/langchain/agents/agent_toolkits/vectorstore/__init__.py
+-rw-r--r--   0        0        0     4217 2024-04-19 07:38:33.881834 gigachain-0.2.0/langchain/agents/agent_toolkits/vectorstore/base.py
+-rw-r--r--   0        0        0     1557 2023-08-31 07:54:47.805977 gigachain-0.2.0/langchain/agents/agent_toolkits/vectorstore/prompt.py
+-rw-r--r--   0        0        0     3290 2024-05-06 14:45:38.433799 gigachain-0.2.0/langchain/agents/agent_toolkits/vectorstore/toolkit.py
+-rw-r--r--   0        0        0     1095 2023-12-18 12:05:46.870552 gigachain-0.2.0/langchain/agents/agent_toolkits/xorbits/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-21 13:51:28.551302 gigachain-0.2.0/langchain/agents/agent_toolkits/zapier/__init__.py
+-rw-r--r--   0        0        0      670 2024-05-06 14:45:38.434207 gigachain-0.2.0/langchain/agents/agent_toolkits/zapier/toolkit.py
+-rw-r--r--   0        0        0     1949 2024-05-24 11:13:19.196058 gigachain-0.2.0/langchain/agents/agent_types.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.551838 gigachain-0.2.0/langchain/agents/chat/__init__.py
+-rw-r--r--   0        0        0     5110 2024-05-24 11:13:19.196776 gigachain-0.2.0/langchain/agents/chat/base.py
+-rw-r--r--   0        0        0     1977 2024-02-22 08:54:03.079601 gigachain-0.2.0/langchain/agents/chat/output_parser.py
+-rw-r--r--   0        0        0     1776 2023-10-19 12:57:52.688319 gigachain-0.2.0/langchain/agents/chat/prompt.py
+-rw-r--r--   0        0        0       75 2023-08-21 13:51:28.552791 gigachain-0.2.0/langchain/agents/conversational/__init__.py
+-rw-r--r--   0        0        0     4980 2024-05-24 11:13:19.198136 gigachain-0.2.0/langchain/agents/conversational/base.py
+-rw-r--r--   0        0        0     1463 2024-02-22 08:54:03.084332 gigachain-0.2.0/langchain/agents/conversational/output_parser.py
+-rw-r--r--   0        0        0     1312 2023-10-19 12:57:52.695256 gigachain-0.2.0/langchain/agents/conversational/prompt.py
+-rw-r--r--   0        0        0       75 2023-08-21 13:51:28.553657 gigachain-0.2.0/langchain/agents/conversational_chat/__init__.py
+-rw-r--r--   0        0        0     5313 2024-05-24 11:13:19.199448 gigachain-0.2.0/langchain/agents/conversational_chat/base.py
+-rw-r--r--   0        0        0     2394 2024-05-06 14:45:38.434586 gigachain-0.2.0/langchain/agents/conversational_chat/output_parser.py
+-rw-r--r--   0        0        0     2934 2023-10-19 12:57:52.702190 gigachain-0.2.0/langchain/agents/conversational_chat/prompt.py
+-rw-r--r--   0        0        0      956 2024-04-19 07:38:33.888237 gigachain-0.2.0/langchain/agents/format_scratchpad/__init__.py
+-rw-r--r--   0        0        0     2209 2024-02-22 08:54:03.092203 gigachain-0.2.0/langchain/agents/format_scratchpad/gigachat_functions.py
+-rw-r--r--   0        0        0     1885 2024-02-22 08:54:03.093583 gigachain-0.2.0/langchain/agents/format_scratchpad/gigachat_tools.py
+-rw-r--r--   0        0        0      528 2023-12-18 12:05:46.881864 gigachain-0.2.0/langchain/agents/format_scratchpad/log.py
+-rw-r--r--   0        0        0      721 2023-12-18 12:05:46.882588 gigachain-0.2.0/langchain/agents/format_scratchpad/log_to_messages.py
+-rw-r--r--   0        0        0     2203 2023-12-18 12:05:46.883234 gigachain-0.2.0/langchain/agents/format_scratchpad/openai_functions.py
+-rw-r--r--   0        0        0      166 2024-04-19 07:38:33.888898 gigachain-0.2.0/langchain/agents/format_scratchpad/openai_tools.py
+-rw-r--r--   0        0        0     1853 2024-04-19 07:38:33.889312 gigachain-0.2.0/langchain/agents/format_scratchpad/tools.py
+-rw-r--r--   0        0        0      578 2023-12-18 12:05:46.884524 gigachain-0.2.0/langchain/agents/format_scratchpad/xml.py
+-rw-r--r--   0        0        0        0 2024-02-22 08:54:03.093863 gigachain-0.2.0/langchain/agents/gigachat_functions_agent/__init__.py
+-rw-r--r--   0        0        0     2568 2024-04-19 07:38:33.890630 gigachain-0.2.0/langchain/agents/gigachat_functions_agent/agent_token_buffer_memory.py
+-rw-r--r--   0        0        0     4189 2024-05-24 11:13:19.200883 gigachain-0.2.0/langchain/agents/gigachat_functions_agent/base.py
+-rw-r--r--   0        0        0        0 2024-02-22 08:54:03.097626 gigachain-0.2.0/langchain/agents/gigachat_tools/__init__.py
+-rw-r--r--   0        0        0     3237 2024-05-24 11:13:19.202191 gigachain-0.2.0/langchain/agents/gigachat_tools/base.py
+-rw-r--r--   0        0        0     3245 2024-05-24 11:13:19.203374 gigachain-0.2.0/langchain/agents/initialize.py
+-rw-r--r--   0        0        0        0 2024-01-18 15:16:40.615878 gigachain-0.2.0/langchain/agents/json_chat/__init__.py
+-rw-r--r--   0        0        0     7743 2024-04-19 07:38:33.894335 gigachain-0.2.0/langchain/agents/json_chat/base.py
+-rw-r--r--   0        0        0      551 2024-01-18 15:16:40.617394 gigachain-0.2.0/langchain/agents/json_chat/prompt.py
+-rw-r--r--   0        0        0      286 2024-05-06 14:45:38.435444 gigachain-0.2.0/langchain/agents/load_tools.py
+-rw-r--r--   0        0        0     4671 2024-05-24 11:13:19.204379 gigachain-0.2.0/langchain/agents/loading.py
+-rw-r--r--   0        0        0       86 2023-08-21 13:51:28.555248 gigachain-0.2.0/langchain/agents/mrkl/__init__.py
+-rw-r--r--   0        0        0     6065 2024-05-24 11:13:19.205518 gigachain-0.2.0/langchain/agents/mrkl/base.py
+-rw-r--r--   0        0        0     3407 2024-02-22 08:54:03.108171 gigachain-0.2.0/langchain/agents/mrkl/output_parser.py
+-rw-r--r--   0        0        0     1602 2023-12-18 12:05:46.889787 gigachain-0.2.0/langchain/agents/mrkl/prompt.py
+-rw-r--r--   0        0        0      114 2023-12-18 12:05:46.890436 gigachain-0.2.0/langchain/agents/openai_assistant/__init__.py
+-rw-r--r--   0        0        0    27677 2024-05-24 11:13:19.207113 gigachain-0.2.0/langchain/agents/openai_assistant/base.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.556082 gigachain-0.2.0/langchain/agents/openai_functions_agent/__init__.py
+-rw-r--r--   0        0        0     2762 2024-05-06 14:45:38.437961 gigachain-0.2.0/langchain/agents/openai_functions_agent/agent_token_buffer_memory.py
+-rw-r--r--   0        0        0    11634 2024-05-24 11:13:19.208531 gigachain-0.2.0/langchain/agents/openai_functions_agent/base.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.556705 gigachain-0.2.0/langchain/agents/openai_functions_multi_agent/__init__.py
+-rw-r--r--   0        0        0    12007 2024-05-24 11:13:19.209962 gigachain-0.2.0/langchain/agents/openai_functions_multi_agent/base.py
+-rw-r--r--   0        0        0        0 2024-01-18 15:16:40.628412 gigachain-0.2.0/langchain/agents/openai_tools/__init__.py
+-rw-r--r--   0        0        0     3435 2024-04-19 07:38:33.908167 gigachain-0.2.0/langchain/agents/openai_tools/base.py
+-rw-r--r--   0        0        0     1523 2024-04-19 07:38:33.909235 gigachain-0.2.0/langchain/agents/output_parsers/__init__.py
+-rw-r--r--   0        0        0     3224 2024-05-24 11:13:19.211316 gigachain-0.2.0/langchain/agents/output_parsers/gigachat_functions.py
+-rw-r--r--   0        0        0     1846 2024-02-22 08:54:03.125684 gigachain-0.2.0/langchain/agents/output_parsers/json.py
+-rw-r--r--   0        0        0     3467 2024-03-28 07:19:21.421200 gigachain-0.2.0/langchain/agents/output_parsers/openai_functions.py
+-rw-r--r--   0        0        0     2317 2024-04-19 07:38:33.909941 gigachain-0.2.0/langchain/agents/output_parsers/openai_tools.py
+-rw-r--r--   0        0        0     2455 2024-02-22 08:54:03.126947 gigachain-0.2.0/langchain/agents/output_parsers/react_json_single_input.py
+-rw-r--r--   0        0        0     3218 2023-12-18 12:05:46.905924 gigachain-0.2.0/langchain/agents/output_parsers/react_single_input.py
+-rw-r--r--   0        0        0     1545 2023-12-18 12:05:46.906825 gigachain-0.2.0/langchain/agents/output_parsers/self_ask.py
+-rw-r--r--   0        0        0     3753 2024-04-19 07:38:33.910352 gigachain-0.2.0/langchain/agents/output_parsers/tools.py
+-rw-r--r--   0        0        0     1658 2023-12-18 12:05:46.907986 gigachain-0.2.0/langchain/agents/output_parsers/xml.py
+-rw-r--r--   0        0        0       76 2023-08-21 13:51:28.557154 gigachain-0.2.0/langchain/agents/react/__init__.py
+-rw-r--r--   0        0        0     4975 2024-04-19 07:38:33.911676 gigachain-0.2.0/langchain/agents/react/agent.py
+-rw-r--r--   0        0        0     5798 2024-05-24 11:13:19.213272 gigachain-0.2.0/langchain/agents/react/base.py
+-rw-r--r--   0        0        0     1231 2023-12-18 12:05:46.909814 gigachain-0.2.0/langchain/agents/react/output_parser.py
+-rw-r--r--   0        0        0     3005 2023-12-18 12:05:46.910755 gigachain-0.2.0/langchain/agents/react/textworld_prompt.py
+-rw-r--r--   0        0        0    10562 2023-12-18 12:05:46.911736 gigachain-0.2.0/langchain/agents/react/wiki_prompt.py
+-rw-r--r--   0        0        0     1175 2023-12-18 12:05:46.912970 gigachain-0.2.0/langchain/agents/schema.py
+-rw-r--r--   0        0        0      106 2023-08-21 13:51:28.559443 gigachain-0.2.0/langchain/agents/self_ask_with_search/__init__.py
+-rw-r--r--   0        0        0     8304 2024-05-24 11:13:19.215663 gigachain-0.2.0/langchain/agents/self_ask_with_search/base.py
+-rw-r--r--   0        0        0      138 2023-09-25 07:40:35.498979 gigachain-0.2.0/langchain/agents/self_ask_with_search/output_parser.py
+-rw-r--r--   0        0        0     3502 2023-12-18 12:05:46.916766 gigachain-0.2.0/langchain/agents/self_ask_with_search/prompt.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.560593 gigachain-0.2.0/langchain/agents/structured_chat/__init__.py
+-rw-r--r--   0        0        0    10812 2024-05-24 11:13:19.216377 gigachain-0.2.0/langchain/agents/structured_chat/base.py
+-rw-r--r--   0        0        0     3799 2024-04-18 09:51:24.600223 gigachain-0.2.0/langchain/agents/structured_chat/output_parser.py
+-rw-r--r--   0        0        0     1663 2023-09-07 06:38:18.010991 gigachain-0.2.0/langchain/agents/structured_chat/prompt.py
+-rw-r--r--   0        0        0        0 2024-04-19 07:38:33.916625 gigachain-0.2.0/langchain/agents/tool_calling_agent/__init__.py
+-rw-r--r--   0        0        0     3465 2024-05-24 11:13:19.217493 gigachain-0.2.0/langchain/agents/tool_calling_agent/base.py
+-rw-r--r--   0        0        0     1410 2024-04-19 07:38:33.918174 gigachain-0.2.0/langchain/agents/tools.py
+-rw-r--r--   0        0        0     1475 2024-01-29 08:25:46.514870 gigachain-0.2.0/langchain/agents/types.py
+-rw-r--r--   0        0        0      384 2023-12-18 12:05:46.920460 gigachain-0.2.0/langchain/agents/utils.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.562209 gigachain-0.2.0/langchain/agents/xml/__init__.py
+-rw-r--r--   0        0        0     8103 2024-05-24 11:13:19.218308 gigachain-0.2.0/langchain/agents/xml/base.py
+-rw-r--r--   0        0        0      767 2024-01-18 15:16:40.638769 gigachain-0.2.0/langchain/agents/xml/prompt.py
+-rw-r--r--   0        0        0      218 2024-04-19 07:38:33.920136 gigachain-0.2.0/langchain/base_language.py
+-rw-r--r--   0        0        0     2155 2024-05-06 14:45:38.440004 gigachain-0.2.0/langchain/cache.py
+-rw-r--r--   0        0        0     5960 2024-05-06 14:45:38.440717 gigachain-0.2.0/langchain/callbacks/__init__.py
+-rw-r--r--   0        0        0      941 2024-05-06 14:45:38.441176 gigachain-0.2.0/langchain/callbacks/aim_callback.py
+-rw-r--r--   0        0        0      688 2024-05-06 14:45:38.441668 gigachain-0.2.0/langchain/callbacks/argilla_callback.py
+-rw-r--r--   0        0        0      678 2024-05-06 14:45:38.442566 gigachain-0.2.0/langchain/callbacks/arize_callback.py
+-rw-r--r--   0        0        0      683 2024-05-06 14:45:38.443160 gigachain-0.2.0/langchain/callbacks/arthur_callback.py
+-rw-r--r--   0        0        0      654 2024-04-19 07:38:33.922440 gigachain-0.2.0/langchain/callbacks/base.py
+-rw-r--r--   0        0        0      688 2024-05-06 14:45:38.443758 gigachain-0.2.0/langchain/callbacks/clearml_callback.py
+-rw-r--r--   0        0        0      684 2024-05-06 14:45:38.444322 gigachain-0.2.0/langchain/callbacks/comet_ml_callback.py
+-rw-r--r--   0        0        0      695 2024-05-06 14:45:38.444936 gigachain-0.2.0/langchain/callbacks/confident_callback.py
+-rw-r--r--   0        0        0      688 2024-05-06 14:45:38.445469 gigachain-0.2.0/langchain/callbacks/context_callback.py
+-rw-r--r--   0        0        0       97 2024-05-06 14:45:38.445929 gigachain-0.2.0/langchain/callbacks/file.py
+-rw-r--r--   0        0        0      678 2024-05-06 14:45:38.446470 gigachain-0.2.0/langchain/callbacks/flyte_callback.py
+-rw-r--r--   0        0        0      997 2024-05-06 14:45:38.447095 gigachain-0.2.0/langchain/callbacks/human.py
+-rw-r--r--   0        0        0      683 2024-05-06 14:45:38.447672 gigachain-0.2.0/langchain/callbacks/infino_callback.py
+-rw-r--r--   0        0        0     1006 2024-05-06 14:45:38.448180 gigachain-0.2.0/langchain/callbacks/labelstudio_callback.py
+-rw-r--r--   0        0        0      715 2024-05-06 14:45:38.448739 gigachain-0.2.0/langchain/callbacks/llmonitor_callback.py
+-rw-r--r--   0        0        0     2410 2024-05-06 14:45:38.449371 gigachain-0.2.0/langchain/callbacks/manager.py
+-rw-r--r--   0        0        0     1137 2024-05-06 14:45:38.449981 gigachain-0.2.0/langchain/callbacks/mlflow_callback.py
+-rw-r--r--   0        0        0      675 2024-05-06 14:45:38.450488 gigachain-0.2.0/langchain/callbacks/openai_info.py
+-rw-r--r--   0        0        0      725 2024-05-06 14:45:38.450962 gigachain-0.2.0/langchain/callbacks/promptlayer_callback.py
+-rw-r--r--   0        0        0      715 2024-05-06 14:45:38.451534 gigachain-0.2.0/langchain/callbacks/sagemaker_callback.py
+-rw-r--r--   0        0        0      103 2023-12-18 12:05:46.944007 gigachain-0.2.0/langchain/callbacks/stdout.py
+-rw-r--r--   0        0        0     2399 2024-02-22 08:54:03.146818 gigachain-0.2.0/langchain/callbacks/streaming_aiter.py
+-rw-r--r--   0        0        0     3371 2023-12-18 12:05:46.945805 gigachain-0.2.0/langchain/callbacks/streaming_aiter_final_only.py
+-rw-r--r--   0        0        0      174 2024-04-19 07:38:33.924090 gigachain-0.2.0/langchain/callbacks/streaming_stdout.py
+-rw-r--r--   0        0        0     3358 2024-04-19 07:38:33.925199 gigachain-0.2.0/langchain/callbacks/streaming_stdout_final_only.py
+-rw-r--r--   0        0        0     3407 2024-05-24 11:13:19.219378 gigachain-0.2.0/langchain/callbacks/streamlit/__init__.py
+-rw-r--r--   0        0        0      937 2024-05-06 14:45:38.451968 gigachain-0.2.0/langchain/callbacks/streamlit/mutable_expander.py
+-rw-r--r--   0        0        0     1372 2024-05-06 14:45:38.452489 gigachain-0.2.0/langchain/callbacks/streamlit/streamlit_callback_handler.py
+-rw-r--r--   0        0        0     1140 2024-05-06 14:45:38.454182 gigachain-0.2.0/langchain/callbacks/tracers/__init__.py
+-rw-r--r--   0        0        0      154 2023-12-18 12:05:46.950003 gigachain-0.2.0/langchain/callbacks/tracers/base.py
+-rw-r--r--   0        0        0      800 2024-05-06 14:45:38.454601 gigachain-0.2.0/langchain/callbacks/tracers/comet.py
+-rw-r--r--   0        0        0      234 2024-04-19 07:38:33.926692 gigachain-0.2.0/langchain/callbacks/tracers/evaluation.py
+-rw-r--r--   0        0        0      218 2023-12-18 12:05:46.952818 gigachain-0.2.0/langchain/callbacks/tracers/langchain.py
+-rw-r--r--   0        0        0       99 2023-12-18 12:05:46.953574 gigachain-0.2.0/langchain/callbacks/tracers/langchain_v1.py
+-rw-r--r--   0        0        0      226 2023-12-18 12:05:46.954653 gigachain-0.2.0/langchain/callbacks/tracers/log_stream.py
+-rw-r--r--   0        0        0     1384 2023-12-18 12:05:46.955043 gigachain-0.2.0/langchain/callbacks/tracers/logging.py
+-rw-r--r--   0        0        0      105 2023-12-18 12:05:46.955825 gigachain-0.2.0/langchain/callbacks/tracers/root_listeners.py
+-rw-r--r--   0        0        0      120 2023-12-18 12:05:46.956667 gigachain-0.2.0/langchain/callbacks/tracers/run_collector.py
+-rw-r--r--   0        0        0      470 2023-12-18 12:05:46.957919 gigachain-0.2.0/langchain/callbacks/tracers/schemas.py
+-rw-r--r--   0        0        0      168 2023-12-18 12:05:46.958747 gigachain-0.2.0/langchain/callbacks/tracers/stdout.py
+-rw-r--r--   0        0        0      885 2024-05-06 14:45:38.455248 gigachain-0.2.0/langchain/callbacks/tracers/wandb.py
+-rw-r--r--   0        0        0      693 2024-05-06 14:45:38.455784 gigachain-0.2.0/langchain/callbacks/trubrics_callback.py
+-rw-r--r--   0        0        0     1409 2024-05-06 14:45:38.456312 gigachain-0.2.0/langchain/callbacks/utils.py
+-rw-r--r--   0        0        0      678 2024-05-06 14:45:38.456857 gigachain-0.2.0/langchain/callbacks/wandb_callback.py
+-rw-r--r--   0        0        0      688 2024-05-06 14:45:38.457410 gigachain-0.2.0/langchain/callbacks/whylabs_callback.py
+-rw-r--r--   0        0        0     5011 2024-05-24 11:13:19.220458 gigachain-0.2.0/langchain/chains/__init__.py
+-rw-r--r--   0        0        0       84 2023-08-21 13:51:28.576965 gigachain-0.2.0/langchain/chains/api/__init__.py
+-rw-r--r--   0        0        0    10004 2024-05-24 11:13:19.221773 gigachain-0.2.0/langchain/chains/api/base.py
+-rw-r--r--   0        0        0     2452 2024-01-10 09:04:40.341669 gigachain-0.2.0/langchain/chains/api/news_docs.py
+-rw-r--r--   0        0        0     3399 2023-08-21 13:51:28.578041 gigachain-0.2.0/langchain/chains/api/open_meteo_docs.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.578278 gigachain-0.2.0/langchain/chains/api/openapi/__init__.py
+-rw-r--r--   0        0        0      667 2024-05-24 11:13:19.223157 gigachain-0.2.0/langchain/chains/api/openapi/chain.py
+-rw-r--r--   0        0        0      795 2024-05-24 11:13:19.223831 gigachain-0.2.0/langchain/chains/api/openapi/prompts.py
+-rw-r--r--   0        0        0      963 2024-05-24 11:13:19.224587 gigachain-0.2.0/langchain/chains/api/openapi/requests_chain.py
+-rw-r--r--   0        0        0      966 2024-05-24 11:13:19.225108 gigachain-0.2.0/langchain/chains/api/openapi/response_chain.py
+-rw-r--r--   0        0        0     1920 2023-08-21 13:51:28.580702 gigachain-0.2.0/langchain/chains/api/podcast_docs.py
+-rw-r--r--   0        0        0     1326 2023-12-18 12:05:46.970482 gigachain-0.2.0/langchain/chains/api/prompt.py
+-rw-r--r--   0        0        0     1537 2023-08-21 13:51:28.581731 gigachain-0.2.0/langchain/chains/api/tmdb_docs.py
+-rw-r--r--   0        0        0    30706 2024-05-24 11:13:19.227165 gigachain-0.2.0/langchain/chains/base.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.582802 gigachain-0.2.0/langchain/chains/chat_vector_db/__init__.py
+-rw-r--r--   0        0        0     1037 2023-12-18 12:05:46.972569 gigachain-0.2.0/langchain/chains/chat_vector_db/prompts.py
+-rw-r--r--   0        0        0      367 2024-01-10 09:04:40.342648 gigachain-0.2.0/langchain/chains/combine_documents/__init__.py
+-rw-r--r--   0        0        0     8095 2024-04-19 07:38:33.933037 gigachain-0.2.0/langchain/chains/combine_documents/base.py
+-rw-r--r--   0        0        0     1743 2023-11-15 10:30:09.330835 gigachain-0.2.0/langchain/chains/combine_documents/conditional.py
+-rw-r--r--   0        0        0    11781 2024-03-28 12:44:20.511275 gigachain-0.2.0/langchain/chains/combine_documents/map_reduce.py
+-rw-r--r--   0        0        0     8991 2024-03-28 12:44:20.512103 gigachain-0.2.0/langchain/chains/combine_documents/map_rerank.py
+-rw-r--r--   0        0        0    13894 2024-02-22 08:54:03.165440 gigachain-0.2.0/langchain/chains/combine_documents/reduce.py
+-rw-r--r--   0        0        0     9113 2024-02-22 08:54:03.166781 gigachain-0.2.0/langchain/chains/combine_documents/refine.py
+-rw-r--r--   0        0        0    11026 2024-04-19 07:38:33.934139 gigachain-0.2.0/langchain/chains/combine_documents/stuff.py
+-rw-r--r--   0        0        0      107 2023-08-21 13:51:28.587546 gigachain-0.2.0/langchain/chains/constitutional_ai/__init__.py
+-rw-r--r--   0        0        0     6342 2024-04-19 07:38:33.935163 gigachain-0.2.0/langchain/chains/constitutional_ai/base.py
+-rw-r--r--   0        0        0      284 2024-04-19 07:38:33.936074 gigachain-0.2.0/langchain/chains/constitutional_ai/models.py
+-rw-r--r--   0        0        0    21739 2024-04-19 07:38:33.937079 gigachain-0.2.0/langchain/chains/constitutional_ai/principles.py
+-rw-r--r--   0        0        0    14534 2023-12-18 12:05:46.982679 gigachain-0.2.0/langchain/chains/constitutional_ai/prompts.py
+-rw-r--r--   0        0        0       71 2023-08-21 13:51:28.589976 gigachain-0.2.0/langchain/chains/conversation/__init__.py
+-rw-r--r--   0        0        0     2367 2024-04-19 07:38:33.937854 gigachain-0.2.0/langchain/chains/conversation/base.py
+-rw-r--r--   0        0        0     1396 2024-05-24 11:13:19.227740 gigachain-0.2.0/langchain/chains/conversation/memory.py
+-rw-r--r--   0        0        0     1063 2023-12-18 12:05:46.984228 gigachain-0.2.0/langchain/chains/conversation/prompt.py
+-rw-r--r--   0        0        0       49 2023-08-21 13:51:28.591153 gigachain-0.2.0/langchain/chains/conversational_retrieval/__init__.py
+-rw-r--r--   0        0        0    21227 2024-05-06 14:45:38.461772 gigachain-0.2.0/langchain/chains/conversational_retrieval/base.py
+-rw-r--r--   0        0        0     1037 2023-12-18 12:05:46.988192 gigachain-0.2.0/langchain/chains/conversational_retrieval/prompts.py
+-rw-r--r--   0        0        0      126 2023-08-21 13:51:28.592942 gigachain-0.2.0/langchain/chains/elasticsearch_database/__init__.py
+-rw-r--r--   0        0        0     8288 2024-04-19 07:38:33.941270 gigachain-0.2.0/langchain/chains/elasticsearch_database/base.py
+-rw-r--r--   0        0        0     2480 2023-12-18 12:05:46.989727 gigachain-0.2.0/langchain/chains/elasticsearch_database/prompts.py
+-rw-r--r--   0        0        0      669 2023-10-30 16:05:53.857849 gigachain-0.2.0/langchain/chains/encoder.py
+-rw-r--r--   0        0        0     1514 2024-05-24 11:13:19.228444 gigachain-0.2.0/langchain/chains/ernie_functions/__init__.py
+-rw-r--r--   0        0        0     1730 2024-05-24 11:13:19.228916 gigachain-0.2.0/langchain/chains/ernie_functions/base.py
+-rw-r--r--   0        0        0      741 2023-12-18 12:05:46.991949 gigachain-0.2.0/langchain/chains/example_generator.py
+-rw-r--r--   0        0        0       51 2023-08-21 13:51:28.594704 gigachain-0.2.0/langchain/chains/flare/__init__.py
+-rw-r--r--   0        0        0     9081 2024-05-06 14:45:38.464797 gigachain-0.2.0/langchain/chains/flare/base.py
+-rw-r--r--   0        0        0     1949 2023-12-18 12:05:46.993539 gigachain-0.2.0/langchain/chains/flare/prompts.py
+-rw-r--r--   0        0        0        0 2024-05-24 11:13:19.229517 gigachain-0.2.0/langchain/chains/graph_qa/__init__.py
+-rw-r--r--   0        0        0      669 2024-05-24 11:13:19.230199 gigachain-0.2.0/langchain/chains/graph_qa/arangodb.py
+-rw-r--r--   0        0        0      643 2024-05-24 11:13:19.230822 gigachain-0.2.0/langchain/chains/graph_qa/base.py
+-rw-r--r--   0        0        0     1205 2024-05-24 11:13:19.231406 gigachain-0.2.0/langchain/chains/graph_qa/cypher.py
+-rw-r--r--   0        0        0      792 2024-05-24 11:13:19.232173 gigachain-0.2.0/langchain/chains/graph_qa/cypher_utils.py
+-rw-r--r--   0        0        0      925 2024-05-24 11:13:19.232779 gigachain-0.2.0/langchain/chains/graph_qa/falkordb.py
+-rw-r--r--   0        0        0     1090 2024-05-24 11:13:19.233375 gigachain-0.2.0/langchain/chains/graph_qa/gremlin.py
+-rw-r--r--   0        0        0      665 2024-05-24 11:13:19.233933 gigachain-0.2.0/langchain/chains/graph_qa/hugegraph.py
+-rw-r--r--   0        0        0      870 2024-05-24 11:13:19.234554 gigachain-0.2.0/langchain/chains/graph_qa/kuzu.py
+-rw-r--r--   0        0        0      675 2024-05-24 11:13:19.235419 gigachain-0.2.0/langchain/chains/graph_qa/nebulagraph.py
+-rw-r--r--   0        0        0     1232 2024-05-24 11:13:19.236045 gigachain-0.2.0/langchain/chains/graph_qa/neptune_cypher.py
+-rw-r--r--   0        0        0     1137 2024-05-24 11:13:19.236696 gigachain-0.2.0/langchain/chains/graph_qa/neptune_sparql.py
+-rw-r--r--   0        0        0      714 2024-05-24 11:13:19.237249 gigachain-0.2.0/langchain/chains/graph_qa/ontotext_graphdb.py
+-rw-r--r--   0        0        0     4007 2024-05-24 11:13:19.238516 gigachain-0.2.0/langchain/chains/graph_qa/prompts.py
+-rw-r--r--   0        0        0      665 2024-05-24 11:13:19.239201 gigachain-0.2.0/langchain/chains/graph_qa/sparql.py
+-rw-r--r--   0        0        0     2662 2024-01-10 09:04:40.353033 gigachain-0.2.0/langchain/chains/history_aware_retriever.py
+-rw-r--r--   0        0        0       75 2023-08-21 13:51:28.600763 gigachain-0.2.0/langchain/chains/hyde/__init__.py
+-rw-r--r--   0        0        0     3342 2024-04-19 07:38:33.957431 gigachain-0.2.0/langchain/chains/hyde/base.py
+-rw-r--r--   0        0        0     2482 2023-12-18 12:05:47.005583 gigachain-0.2.0/langchain/chains/hyde/prompts.py
+-rw-r--r--   0        0        0    15725 2024-05-06 14:45:38.470787 gigachain-0.2.0/langchain/chains/llm.py
+-rw-r--r--   0        0        0      453 2024-05-06 14:45:38.474757 gigachain-0.2.0/langchain/chains/llm_bash/__init__.py
+-rw-r--r--   0        0        0      139 2023-08-21 13:51:28.604012 gigachain-0.2.0/langchain/chains/llm_checker/__init__.py
+-rw-r--r--   0        0        0     6191 2024-04-19 07:38:33.959340 gigachain-0.2.0/langchain/chains/llm_checker/base.py
+-rw-r--r--   0        0        0     1341 2023-12-18 12:05:47.009556 gigachain-0.2.0/langchain/chains/llm_checker/prompt.py
+-rw-r--r--   0        0        0      143 2023-08-21 13:51:28.605454 gigachain-0.2.0/langchain/chains/llm_math/__init__.py
+-rw-r--r--   0        0        0     6710 2024-05-06 14:45:38.476426 gigachain-0.2.0/langchain/chains/llm_math/base.py
+-rw-r--r--   0        0        0     1158 2023-12-18 12:05:47.012133 gigachain-0.2.0/langchain/chains/llm_math/prompt.py
+-rw-r--r--   0        0        0      653 2024-05-24 11:13:19.239812 gigachain-0.2.0/langchain/chains/llm_requests.py
+-rw-r--r--   0        0        0      352 2023-08-21 13:51:28.607135 gigachain-0.2.0/langchain/chains/llm_summarization_checker/__init__.py
+-rw-r--r--   0        0        0     6582 2024-02-22 08:54:03.202882 gigachain-0.2.0/langchain/chains/llm_summarization_checker/base.py
+-rw-r--r--   0        0        0     1143 2023-08-22 11:25:59.886227 gigachain-0.2.0/langchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt
+-rw-r--r--   0        0        0      696 2023-08-22 11:25:59.887142 gigachain-0.2.0/langchain/chains/llm_summarization_checker/prompts/check_facts.txt
+-rw-r--r--   0        0        0      234 2023-08-22 11:25:59.887992 gigachain-0.2.0/langchain/chains/llm_summarization_checker/prompts/create_facts.txt
+-rw-r--r--   0        0        0      834 2023-08-22 11:25:59.888905 gigachain-0.2.0/langchain/chains/llm_summarization_checker/prompts/revise_summary.txt
+-rw-r--r--   0        0        0      470 2024-05-06 14:45:38.477573 gigachain-0.2.0/langchain/chains/llm_symbolic_math/__init__.py
+-rw-r--r--   0        0        0    28333 2024-05-24 11:13:19.241893 gigachain-0.2.0/langchain/chains/loading.py
+-rw-r--r--   0        0        0     3734 2024-04-19 07:38:33.964088 gigachain-0.2.0/langchain/chains/mapreduce.py
+-rw-r--r--   0        0        0     4406 2024-05-24 11:13:19.242988 gigachain-0.2.0/langchain/chains/moderation.py
+-rw-r--r--   0        0        0       96 2023-08-21 13:51:28.612079 gigachain-0.2.0/langchain/chains/natbot/__init__.py
+-rw-r--r--   0        0        0     4779 2024-05-06 14:45:38.478771 gigachain-0.2.0/langchain/chains/natbot/base.py
+-rw-r--r--   0        0        0    16050 2024-02-22 08:54:03.214508 gigachain-0.2.0/langchain/chains/natbot/crawler.py
+-rw-r--r--   0        0        0     6769 2023-12-18 12:05:47.020892 gigachain-0.2.0/langchain/chains/natbot/prompt.py
+-rw-r--r--   0        0        0     1403 2024-05-06 14:45:38.479332 gigachain-0.2.0/langchain/chains/openai_functions/__init__.py
+-rw-r--r--   0        0        0    10309 2024-05-24 11:13:19.244363 gigachain-0.2.0/langchain/chains/openai_functions/base.py
+-rw-r--r--   0        0        0     3558 2024-04-19 07:38:33.968351 gigachain-0.2.0/langchain/chains/openai_functions/citation_fuzzy_match.py
+-rw-r--r--   0        0        0     7560 2024-05-24 11:13:19.246366 gigachain-0.2.0/langchain/chains/openai_functions/extraction.py
+-rw-r--r--   0        0        0    11911 2024-05-24 11:13:19.248114 gigachain-0.2.0/langchain/chains/openai_functions/openapi.py
+-rw-r--r--   0        0        0     3959 2024-04-19 07:38:33.969828 gigachain-0.2.0/langchain/chains/openai_functions/qa_with_structure.py
+-rw-r--r--   0        0        0     2769 2024-05-06 14:45:38.482651 gigachain-0.2.0/langchain/chains/openai_functions/tagging.py
+-rw-r--r--   0        0        0     1255 2024-05-06 14:45:38.483178 gigachain-0.2.0/langchain/chains/openai_functions/utils.py
+-rw-r--r--   0        0        0      134 2023-11-10 13:07:50.024454 gigachain-0.2.0/langchain/chains/openai_tools/__init__.py
+-rw-r--r--   0        0        0     3428 2024-05-24 11:13:19.248947 gigachain-0.2.0/langchain/chains/openai_tools/extraction.py
+-rw-r--r--   0        0        0     2015 2023-12-18 12:05:47.029972 gigachain-0.2.0/langchain/chains/prompt_selector.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.617097 gigachain-0.2.0/langchain/chains/qa_generation/__init__.py
+-rw-r--r--   0        0        0     2465 2024-04-19 07:38:33.972432 gigachain-0.2.0/langchain/chains/qa_generation/base.py
+-rw-r--r--   0        0        0     2657 2023-12-18 12:05:47.032423 gigachain-0.2.0/langchain/chains/qa_generation/prompt.py
+-rw-r--r--   0        0        0      174 2024-04-19 07:38:33.973523 gigachain-0.2.0/langchain/chains/qa_with_sources/__init__.py
+-rw-r--r--   0        0        0     7998 2024-04-19 07:38:33.974447 gigachain-0.2.0/langchain/chains/qa_with_sources/base.py
+-rw-r--r--   0        0        0     7080 2024-04-19 07:38:33.975372 gigachain-0.2.0/langchain/chains/qa_with_sources/loading.py
+-rw-r--r--   0        0        0     4144 2023-12-18 12:05:47.035020 gigachain-0.2.0/langchain/chains/qa_with_sources/map_reduce_prompt.py
+-rw-r--r--   0        0        0     1764 2023-12-18 12:05:47.035786 gigachain-0.2.0/langchain/chains/qa_with_sources/refine_prompts.py
+-rw-r--r--   0        0        0     2451 2024-05-06 14:45:38.484414 gigachain-0.2.0/langchain/chains/qa_with_sources/retrieval.py
+-rw-r--r--   0        0        0     3471 2023-12-18 12:05:47.037437 gigachain-0.2.0/langchain/chains/qa_with_sources/stuff_prompt.py
+-rw-r--r--   0        0        0     2770 2024-02-22 08:54:03.225130 gigachain-0.2.0/langchain/chains/qa_with_sources/vector_db.py
+-rw-r--r--   0        0        0      131 2024-02-22 08:54:03.225931 gigachain-0.2.0/langchain/chains/query_constructor/__init__.py
+-rw-r--r--   0        0        0    13781 2024-05-06 14:45:38.485856 gigachain-0.2.0/langchain/chains/query_constructor/base.py
+-rw-r--r--   0        0        0      393 2024-05-06 14:45:38.486800 gigachain-0.2.0/langchain/chains/query_constructor/ir.py
+-rw-r--r--   0        0        0     5694 2024-05-06 14:45:38.487583 gigachain-0.2.0/langchain/chains/query_constructor/parser.py
+-rw-r--r--   0        0        0    10146 2023-12-18 12:05:47.041579 gigachain-0.2.0/langchain/chains/query_constructor/prompt.py
+-rw-r--r--   0        0        0      321 2023-12-18 12:05:47.042242 gigachain-0.2.0/langchain/chains/query_constructor/schema.py
+-rw-r--r--   0        0        0      144 2024-05-24 11:13:19.250499 gigachain-0.2.0/langchain/chains/question_answering/__init__.py
+-rw-r--r--   0        0        0     8811 2024-05-24 11:13:19.252311 gigachain-0.2.0/langchain/chains/question_answering/chain.py
+-rw-r--r--   0        0        0     5425 2023-12-18 12:05:47.043620 gigachain-0.2.0/langchain/chains/question_answering/map_reduce_prompt.py
+-rw-r--r--   0        0        0     2477 2023-12-18 12:05:47.044547 gigachain-0.2.0/langchain/chains/question_answering/map_rerank_prompt.py
+-rw-r--r--   0        0        0     3133 2023-12-18 12:05:47.045293 gigachain-0.2.0/langchain/chains/question_answering/refine_prompts.py
+-rw-r--r--   0        0        0     1404 2023-12-18 12:05:47.046327 gigachain-0.2.0/langchain/chains/question_answering/stuff_prompt.py
+-rw-r--r--   0        0        0     2742 2024-01-18 15:16:40.690412 gigachain-0.2.0/langchain/chains/retrieval.py
+-rw-r--r--   0        0        0       62 2023-08-21 13:51:28.631121 gigachain-0.2.0/langchain/chains/retrieval_qa/__init__.py
+-rw-r--r--   0        0        0    11244 2024-05-24 11:13:19.253775 gigachain-0.2.0/langchain/chains/retrieval_qa/base.py
+-rw-r--r--   0        0        0      527 2023-12-18 12:05:47.048474 gigachain-0.2.0/langchain/chains/retrieval_qa/prompt.py
+-rw-r--r--   0        0        0      407 2023-08-21 13:51:28.632647 gigachain-0.2.0/langchain/chains/router/__init__.py
+-rw-r--r--   0        0        0     4572 2024-04-19 07:38:33.982602 gigachain-0.2.0/langchain/chains/router/base.py
+-rw-r--r--   0        0        0     3124 2024-04-19 07:38:33.983033 gigachain-0.2.0/langchain/chains/router/embedding_router.py
+-rw-r--r--   0        0        0     4346 2024-05-06 14:45:38.490492 gigachain-0.2.0/langchain/chains/router/llm_router.py
+-rw-r--r--   0        0        0     2246 2024-04-19 07:38:33.984707 gigachain-0.2.0/langchain/chains/router/multi_prompt.py
+-rw-r--r--   0        0        0     1849 2023-09-04 05:57:22.503454 gigachain-0.2.0/langchain/chains/router/multi_prompt_prompt.py
+-rw-r--r--   0        0        0     1904 2023-08-21 14:03:46.158141 gigachain-0.2.0/langchain/chains/router/multi_retrieval_prompt.py
+-rw-r--r--   0        0        0     4228 2024-05-06 14:45:38.491679 gigachain-0.2.0/langchain/chains/router/multi_retrieval_qa.py
+-rw-r--r--   0        0        0     7511 2024-04-19 07:38:33.986387 gigachain-0.2.0/langchain/chains/sequential.py
+-rw-r--r--   0        0        0       47 2023-08-21 13:51:28.636997 gigachain-0.2.0/langchain/chains/sql_database/__init__.py
+-rw-r--r--   0        0        0    30619 2024-02-22 08:54:03.240301 gigachain-0.2.0/langchain/chains/sql_database/prompt.py
+-rw-r--r--   0        0        0     5367 2024-05-24 11:13:19.254871 gigachain-0.2.0/langchain/chains/sql_database/query.py
+-rw-r--r--   0        0        0      204 2024-02-22 08:54:03.242140 gigachain-0.2.0/langchain/chains/structured_output/__init__.py
+-rw-r--r--   0        0        0    25650 2024-05-24 11:13:19.256874 gigachain-0.2.0/langchain/chains/structured_output/base.py
+-rw-r--r--   0        0        0    11561 2024-04-19 07:38:33.988309 gigachain-0.2.0/langchain/chains/structured_output/gigachat.py
+-rw-r--r--   0        0        0      151 2024-05-24 11:13:19.257785 gigachain-0.2.0/langchain/chains/summarize/__init__.py
+-rw-r--r--   0        0        0     6192 2024-05-24 11:13:19.260473 gigachain-0.2.0/langchain/chains/summarize/chain.py
+-rw-r--r--   0        0        0      271 2023-12-18 12:05:47.059118 gigachain-0.2.0/langchain/chains/summarize/map_reduce_prompt.py
+-rw-r--r--   0        0        0     1138 2023-12-18 12:05:47.060439 gigachain-0.2.0/langchain/chains/summarize/refine_prompts.py
+-rw-r--r--   0        0        0      271 2023-12-18 12:05:47.061163 gigachain-0.2.0/langchain/chains/summarize/stuff_prompt.py
+-rw-r--r--   0        0        0     2370 2024-04-19 07:38:33.991097 gigachain-0.2.0/langchain/chains/transform.py
+-rw-r--r--   0        0        0      452 2023-09-12 10:52:10.662329 gigachain-0.2.0/langchain/chat_loaders/__init__.py
+-rw-r--r--   0        0        0       85 2024-05-06 14:45:38.493510 gigachain-0.2.0/langchain/chat_loaders/base.py
+-rw-r--r--   0        0        0      884 2024-05-06 14:45:38.494377 gigachain-0.2.0/langchain/chat_loaders/facebook_messenger.py
+-rw-r--r--   0        0        0      636 2024-05-06 14:45:38.495985 gigachain-0.2.0/langchain/chat_loaders/gmail.py
+-rw-r--r--   0        0        0      663 2024-05-06 14:45:38.496562 gigachain-0.2.0/langchain/chat_loaders/imessage.py
+-rw-r--r--   0        0        0      851 2024-05-06 14:45:38.497206 gigachain-0.2.0/langchain/chat_loaders/langsmith.py
+-rw-r--r--   0        0        0      648 2024-05-06 14:45:38.497760 gigachain-0.2.0/langchain/chat_loaders/slack.py
+-rw-r--r--   0        0        0      663 2024-05-06 14:45:38.498316 gigachain-0.2.0/langchain/chat_loaders/telegram.py
+-rw-r--r--   0        0        0     1077 2024-05-06 14:45:38.498934 gigachain-0.2.0/langchain/chat_loaders/utils.py
+-rw-r--r--   0        0        0      663 2024-05-06 14:45:38.499781 gigachain-0.2.0/langchain/chat_loaders/whatsapp.py
+-rw-r--r--   0        0        0     1995 2024-05-06 14:45:38.501142 gigachain-0.2.0/langchain/chat_models/__init__.py
+-rw-r--r--   0        0        0      851 2024-05-06 14:45:38.501958 gigachain-0.2.0/langchain/chat_models/anthropic.py
+-rw-r--r--   0        0        0      643 2024-05-06 14:45:38.503463 gigachain-0.2.0/langchain/chat_models/anyscale.py
+-rw-r--r--   0        0        0      660 2024-05-06 14:45:38.504020 gigachain-0.2.0/langchain/chat_models/azure_openai.py
+-rw-r--r--   0        0        0      863 2024-05-06 14:45:38.504557 gigachain-0.2.0/langchain/chat_models/azureml_endpoint.py
+-rw-r--r--   0        0        0      643 2024-05-06 14:45:38.505395 gigachain-0.2.0/langchain/chat_models/baichuan.py
+-rw-r--r--   0        0        0      715 2024-05-06 14:45:38.506064 gigachain-0.2.0/langchain/chat_models/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0      268 2024-01-10 09:04:40.361805 gigachain-0.2.0/langchain/chat_models/base.py
+-rw-r--r--   0        0        0      757 2024-05-06 14:45:38.506616 gigachain-0.2.0/langchain/chat_models/bedrock.py
+-rw-r--r--   0        0        0      633 2024-05-06 14:45:38.507219 gigachain-0.2.0/langchain/chat_models/cohere.py
+-rw-r--r--   0        0        0      653 2024-05-06 14:45:38.507854 gigachain-0.2.0/langchain/chat_models/databricks.py
+-rw-r--r--   0        0        0      637 2024-05-06 14:45:38.508914 gigachain-0.2.0/langchain/chat_models/ernie.py
+-rw-r--r--   0        0        0      643 2024-05-06 14:45:38.509448 gigachain-0.2.0/langchain/chat_models/everlyai.py
+-rw-r--r--   0        0        0      815 2024-05-06 14:45:38.510020 gigachain-0.2.0/langchain/chat_models/fake.py
+-rw-r--r--   0        0        0      648 2024-05-06 14:45:38.510860 gigachain-0.2.0/langchain/chat_models/fireworks.py
+-rw-r--r--   0        0        0      631 2024-05-06 14:45:38.511378 gigachain-0.2.0/langchain/chat_models/gigachat.py
+-rw-r--r--   0        0        0      809 2024-05-06 14:45:38.511898 gigachain-0.2.0/langchain/chat_models/google_palm.py
+-rw-r--r--   0        0        0      658 2024-05-06 14:45:38.512450 gigachain-0.2.0/langchain/chat_models/human.py
+-rw-r--r--   0        0        0      638 2024-05-06 14:45:38.513014 gigachain-0.2.0/langchain/chat_models/hunyuan.py
+-rw-r--r--   0        0        0      821 2024-05-06 14:45:38.513591 gigachain-0.2.0/langchain/chat_models/javelin_ai_gateway.py
+-rw-r--r--   0        0        0      631 2024-05-06 14:45:38.514148 gigachain-0.2.0/langchain/chat_models/jinachat.py
+-rw-r--r--   0        0        0      628 2024-05-06 14:45:38.514751 gigachain-0.2.0/langchain/chat_models/konko.py
+-rw-r--r--   0        0        0      791 2024-05-06 14:45:38.515265 gigachain-0.2.0/langchain/chat_models/litellm.py
+-rw-r--r--   0        0        0      701 2024-05-06 14:45:38.515792 gigachain-0.2.0/langchain/chat_models/meta.py
+-rw-r--r--   0        0        0      638 2024-05-06 14:45:38.516280 gigachain-0.2.0/langchain/chat_models/minimax.py
+-rw-r--r--   0        0        0      633 2024-05-06 14:45:38.516798 gigachain-0.2.0/langchain/chat_models/mlflow.py
+-rw-r--r--   0        0        0      815 2024-05-06 14:45:38.517348 gigachain-0.2.0/langchain/chat_models/mlflow_ai_gateway.py
+-rw-r--r--   0        0        0      633 2024-05-06 14:45:38.517867 gigachain-0.2.0/langchain/chat_models/ollama.py
+-rw-r--r--   0        0        0      633 2024-05-06 14:45:38.518400 gigachain-0.2.0/langchain/chat_models/openai.py
+-rw-r--r--   0        0        0      683 2024-05-06 14:45:38.518888 gigachain-0.2.0/langchain/chat_models/pai_eas_endpoint.py
+-rw-r--r--   0        0        0      696 2024-05-06 14:45:38.519420 gigachain-0.2.0/langchain/chat_models/promptlayer_openai.py
+-rw-r--r--   0        0        0      633 2024-05-06 14:45:38.519787 gigachain-0.2.0/langchain/chat_models/tongyi.py
+-rw-r--r--   0        0        0      643 2024-05-06 14:45:38.520231 gigachain-0.2.0/langchain/chat_models/vertexai.py
+-rw-r--r--   0        0        0      845 2024-05-06 14:45:38.520605 gigachain-0.2.0/langchain/chat_models/volcengine_maas.py
+-rw-r--r--   0        0        0      642 2024-05-06 14:45:38.520997 gigachain-0.2.0/langchain/chat_models/yandex.py
+-rw-r--r--   0        0        0     1245 2024-05-06 14:45:38.521353 gigachain-0.2.0/langchain/docstore/__init__.py
+-rw-r--r--   0        0        0      639 2024-05-06 14:45:38.521770 gigachain-0.2.0/langchain/docstore/arbitrary_fn.py
+-rw-r--r--   0        0        0      715 2024-05-06 14:45:38.522293 gigachain-0.2.0/langchain/docstore/base.py
+-rw-r--r--   0        0        0       70 2023-12-18 12:05:47.108669 gigachain-0.2.0/langchain/docstore/document.py
+-rw-r--r--   0        0        0      651 2024-05-06 14:45:38.522886 gigachain-0.2.0/langchain/docstore/in_memory.py
+-rw-r--r--   0        0        0      630 2024-05-06 14:45:38.523529 gigachain-0.2.0/langchain/docstore/wikipedia.py
+-rw-r--r--   0        0        0    20659 2024-05-06 14:45:38.525135 gigachain-0.2.0/langchain/document_loaders/__init__.py
+-rw-r--r--   0        0        0      635 2024-05-06 14:45:38.525823 gigachain-0.2.0/langchain/document_loaders/acreom.py
+-rw-r--r--   0        0        0     1574 2024-05-06 14:45:38.526342 gigachain-0.2.0/langchain/document_loaders/airbyte.py
+-rw-r--r--   0        0        0      650 2024-05-06 14:45:38.526740 gigachain-0.2.0/langchain/document_loaders/airbyte_json.py
+-rw-r--r--   0        0        0      641 2024-05-06 14:45:38.527248 gigachain-0.2.0/langchain/document_loaders/airtable.py
+-rw-r--r--   0        0        0      653 2024-05-06 14:45:38.528236 gigachain-0.2.0/langchain/document_loaders/apify_dataset.py
+-rw-r--r--   0        0        0      635 2024-05-06 14:45:38.529229 gigachain-0.2.0/langchain/document_loaders/arcgis_loader.py
+-rw-r--r--   0        0        0      632 2024-05-06 14:45:38.529951 gigachain-0.2.0/langchain/document_loaders/arxiv.py
+-rw-r--r--   0        0        0      879 2024-05-06 14:45:38.530625 gigachain-0.2.0/langchain/document_loaders/assemblyai.py
+-rw-r--r--   0        0        0      644 2024-05-06 14:45:38.531123 gigachain-0.2.0/langchain/document_loaders/async_html.py
+-rw-r--r--   0        0        0      641 2024-05-06 14:45:38.531464 gigachain-0.2.0/langchain/document_loaders/azlyrics.py
+-rw-r--r--   0        0        0      650 2024-05-06 14:45:38.531824 gigachain-0.2.0/langchain/document_loaders/azure_ai_data.py
+-rw-r--r--   0        0        0      698 2024-05-06 14:45:38.532233 gigachain-0.2.0/langchain/document_loaders/azure_blob_storage_container.py
+-rw-r--r--   0        0        0      683 2024-05-06 14:45:38.532702 gigachain-0.2.0/langchain/document_loaders/azure_blob_storage_file.py
+-rw-r--r--   0        0        0      758 2024-05-06 14:45:38.533049 gigachain-0.2.0/langchain/document_loaders/baiducloud_bos_directory.py
+-rw-r--r--   0        0        0      716 2024-05-06 14:45:38.533467 gigachain-0.2.0/langchain/document_loaders/baiducloud_bos_file.py
+-rw-r--r--   0        0        0      115 2024-05-06 14:45:38.534013 gigachain-0.2.0/langchain/document_loaders/base.py
+-rw-r--r--   0        0        0      661 2024-05-06 14:45:38.534547 gigachain-0.2.0/langchain/document_loaders/base_o365.py
+-rw-r--r--   0        0        0      635 2024-05-06 14:45:38.535203 gigachain-0.2.0/langchain/document_loaders/bibtex.py
+-rw-r--r--   0        0        0      641 2024-05-06 14:45:38.535869 gigachain-0.2.0/langchain/document_loaders/bigquery.py
+-rw-r--r--   0        0        0      641 2024-05-06 14:45:38.536366 gigachain-0.2.0/langchain/document_loaders/bilibili.py
+-rw-r--r--   0        0        0      647 2024-05-06 14:45:38.536716 gigachain-0.2.0/langchain/document_loaders/blackboard.py
+-rw-r--r--   0        0        0     1005 2024-05-06 14:45:38.537152 gigachain-0.2.0/langchain/document_loaders/blob_loaders/__init__.py
+-rw-r--r--   0        0        0      659 2024-05-06 14:45:38.537505 gigachain-0.2.0/langchain/document_loaders/blob_loaders/file_system.py
+-rw-r--r--   0        0        0      707 2024-05-24 11:13:19.261084 gigachain-0.2.0/langchain/document_loaders/blob_loaders/schema.py
+-rw-r--r--   0        0        0      653 2024-05-06 14:45:38.538819 gigachain-0.2.0/langchain/document_loaders/blob_loaders/youtube_audio.py
+-rw-r--r--   0        0        0      852 2024-05-06 14:45:38.539321 gigachain-0.2.0/langchain/document_loaders/blockchain.py
+-rw-r--r--   0        0        0      650 2024-05-06 14:45:38.539813 gigachain-0.2.0/langchain/document_loaders/brave_search.py
+-rw-r--r--   0        0        0      650 2024-05-06 14:45:38.540274 gigachain-0.2.0/langchain/document_loaders/browserless.py
+-rw-r--r--   0        0        0      819 2024-05-06 14:45:38.540758 gigachain-0.2.0/langchain/document_loaders/chatgpt.py
+-rw-r--r--   0        0        0      656 2024-05-06 14:45:38.541209 gigachain-0.2.0/langchain/document_loaders/chromium.py
+-rw-r--r--   0        0        0      680 2024-05-06 14:45:38.541763 gigachain-0.2.0/langchain/document_loaders/college_confidential.py
+-rw-r--r--   0        0        0      647 2024-05-06 14:45:38.542322 gigachain-0.2.0/langchain/document_loaders/concurrent.py
+-rw-r--r--   0        0        0      825 2024-05-06 14:45:38.542888 gigachain-0.2.0/langchain/document_loaders/confluence.py
+-rw-r--r--   0        0        0      635 2024-05-06 14:45:38.543453 gigachain-0.2.0/langchain/document_loaders/conllu.py
+-rw-r--r--   0        0        0      644 2024-05-06 14:45:38.544014 gigachain-0.2.0/langchain/document_loaders/couchbase.py
+-rw-r--r--   0        0        0      754 2024-05-06 14:45:38.544561 gigachain-0.2.0/langchain/document_loaders/csv_loader.py
+-rw-r--r--   0        0        0      653 2024-05-06 14:45:38.545132 gigachain-0.2.0/langchain/document_loaders/cube_semantic.py
+-rw-r--r--   0        0        0      650 2024-05-06 14:45:38.545647 gigachain-0.2.0/langchain/document_loaders/datadog_logs.py
+-rw-r--r--   0        0        0      838 2024-05-06 14:45:38.546185 gigachain-0.2.0/langchain/document_loaders/dataframe.py
+-rw-r--r--   0        0        0      638 2024-05-06 14:45:38.546746 gigachain-0.2.0/langchain/document_loaders/diffbot.py
+-rw-r--r--   0        0        0      644 2024-05-06 14:45:38.547249 gigachain-0.2.0/langchain/document_loaders/directory.py
+-rw-r--r--   0        0        0      650 2024-05-06 14:45:38.547797 gigachain-0.2.0/langchain/document_loaders/discord.py
+-rw-r--r--   0        0        0      641 2024-05-06 14:45:38.548388 gigachain-0.2.0/langchain/document_loaders/docugami.py
+-rw-r--r--   0        0        0      647 2024-05-06 14:45:38.548914 gigachain-0.2.0/langchain/document_loaders/docusaurus.py
+-rw-r--r--   0        0        0      638 2024-05-06 14:45:38.549406 gigachain-0.2.0/langchain/document_loaders/dropbox.py
+-rw-r--r--   0        0        0      635 2024-05-06 14:45:38.549914 gigachain-0.2.0/langchain/document_loaders/duckdb_loader.py
+-rw-r--r--   0        0        0      818 2024-05-06 14:45:38.550444 gigachain-0.2.0/langchain/document_loaders/email.py
+-rw-r--r--   0        0        0      665 2024-05-06 14:45:38.550973 gigachain-0.2.0/langchain/document_loaders/epub.py
+-rw-r--r--   0        0        0      644 2024-05-06 14:45:38.551493 gigachain-0.2.0/langchain/document_loaders/etherscan.py
+-rw-r--r--   0        0        0      641 2024-05-06 14:45:38.552063 gigachain-0.2.0/langchain/document_loaders/evernote.py
+-rw-r--r--   0        0        0      668 2024-05-06 14:45:38.552627 gigachain-0.2.0/langchain/document_loaders/excel.py
+-rw-r--r--   0        0        0      846 2024-05-06 14:45:38.553171 gigachain-0.2.0/langchain/document_loaders/facebook_chat.py
+-rw-r--r--   0        0        0      632 2024-05-06 14:45:38.553722 gigachain-0.2.0/langchain/document_loaders/fauna.py
+-rw-r--r--   0        0        0      644 2024-05-06 14:45:38.554276 gigachain-0.2.0/langchain/document_loaders/figma.py
+-rw-r--r--   0        0        0      653 2024-05-06 14:45:38.554936 gigachain-0.2.0/langchain/document_loaders/gcs_directory.py
+-rw-r--r--   0        0        0      638 2024-05-06 14:45:38.555515 gigachain-0.2.0/langchain/document_loaders/gcs_file.py
+-rw-r--r--   0        0        0      654 2024-05-06 14:45:38.556066 gigachain-0.2.0/langchain/document_loaders/generic.py
+-rw-r--r--   0        0        0      653 2024-05-06 14:45:38.556594 gigachain-0.2.0/langchain/document_loaders/geodataframe.py
+-rw-r--r--   0        0        0      626 2024-05-06 14:45:38.557892 gigachain-0.2.0/langchain/document_loaders/git.py
+-rw-r--r--   0        0        0      638 2024-05-06 14:45:38.558478 gigachain-0.2.0/langchain/document_loaders/gitbook.py
+-rw-r--r--   0        0        0      832 2024-05-06 14:45:38.559017 gigachain-0.2.0/langchain/document_loaders/github.py
+-rw-r--r--   0        0        0      671 2024-05-06 14:45:38.559516 gigachain-0.2.0/langchain/document_loaders/google_speech_to_text.py
+-rw-r--r--   0        0        0      650 2024-05-06 14:45:38.560056 gigachain-0.2.0/langchain/document_loaders/googledrive.py
+-rw-r--r--   0        0        0      644 2024-05-06 14:45:38.560592 gigachain-0.2.0/langchain/document_loaders/gutenberg.py
+-rw-r--r--   0        0        0      812 2024-05-06 14:45:38.562286 gigachain-0.2.0/langchain/document_loaders/helpers.py
+-rw-r--r--   0        0        0      623 2024-05-06 14:45:38.563186 gigachain-0.2.0/langchain/document_loaders/hn.py
+-rw-r--r--   0        0        0      665 2024-05-06 14:45:38.563703 gigachain-0.2.0/langchain/document_loaders/html.py
+-rw-r--r--   0        0        0      635 2024-05-06 14:45:38.564313 gigachain-0.2.0/langchain/document_loaders/html_bs.py
+-rw-r--r--   0        0        0      671 2024-05-06 14:45:38.565153 gigachain-0.2.0/langchain/document_loaders/hugging_face_dataset.py
+-rw-r--r--   0        0        0      635 2024-05-06 14:45:38.565728 gigachain-0.2.0/langchain/document_loaders/ifixit.py
+-rw-r--r--   0        0        0      668 2024-05-06 14:45:38.566282 gigachain-0.2.0/langchain/document_loaders/image.py
+-rw-r--r--   0        0        0      653 2024-05-06 14:45:38.566855 gigachain-0.2.0/langchain/document_loaders/image_captions.py
+-rw-r--r--   0        0        0      632 2024-05-06 14:45:38.567592 gigachain-0.2.0/langchain/document_loaders/imsdb.py
+-rw-r--r--   0        0        0      629 2024-05-06 14:45:38.568274 gigachain-0.2.0/langchain/document_loaders/iugu.py
+-rw-r--r--   0        0        0      635 2024-05-06 14:45:38.568935 gigachain-0.2.0/langchain/document_loaders/joplin.py
+-rw-r--r--   0        0        0      629 2024-05-06 14:45:38.569519 gigachain-0.2.0/langchain/document_loaders/json_loader.py
+-rw-r--r--   0        0        0      964 2024-05-06 14:45:38.570074 gigachain-0.2.0/langchain/document_loaders/lakefs.py
+-rw-r--r--   0        0        0      653 2024-05-06 14:45:38.570752 gigachain-0.2.0/langchain/document_loaders/larksuite.py
+-rw-r--r--   0        0        0      683 2024-05-06 14:45:38.571294 gigachain-0.2.0/langchain/document_loaders/markdown.py
+-rw-r--r--   0        0        0      656 2024-05-06 14:45:38.571867 gigachain-0.2.0/langchain/document_loaders/mastodon.py
+-rw-r--r--   0        0        0      647 2024-05-06 14:45:38.572434 gigachain-0.2.0/langchain/document_loaders/max_compute.py
+-rw-r--r--   0        0        0      635 2024-05-06 14:45:38.573158 gigachain-0.2.0/langchain/document_loaders/mediawikidump.py
+-rw-r--r--   0        0        0      647 2024-05-06 14:45:38.573753 gigachain-0.2.0/langchain/document_loaders/merge.py
+-rw-r--r--   0        0        0      632 2024-05-06 14:45:38.574253 gigachain-0.2.0/langchain/document_loaders/mhtml.py
+-rw-r--r--   0        0        0      659 2024-05-06 14:45:38.574856 gigachain-0.2.0/langchain/document_loaders/modern_treasury.py
+-rw-r--r--   0        0        0      638 2024-05-06 14:45:38.575489 gigachain-0.2.0/langchain/document_loaders/mongodb.py
+-rw-r--r--   0        0        0      638 2024-05-06 14:45:38.576046 gigachain-0.2.0/langchain/document_loaders/news.py
+-rw-r--r--   0        0        0      964 2024-05-06 14:45:38.576788 gigachain-0.2.0/langchain/document_loaders/notebook.py
+-rw-r--r--   0        0        0      662 2024-05-06 14:45:38.577407 gigachain-0.2.0/langchain/document_loaders/notion.py
+-rw-r--r--   0        0        0      641 2024-05-06 14:45:38.578183 gigachain-0.2.0/langchain/document_loaders/notiondb.py
+-rw-r--r--   0        0        0      649 2024-05-06 14:45:38.578853 gigachain-0.2.0/langchain/document_loaders/nuclia.py
+-rw-r--r--   0        0        0      653 2024-05-06 14:45:38.579384 gigachain-0.2.0/langchain/document_loaders/obs_directory.py
+-rw-r--r--   0        0        0      638 2024-05-06 14:45:38.579882 gigachain-0.2.0/langchain/document_loaders/obs_file.py
+-rw-r--r--   0        0        0      641 2024-05-06 14:45:38.580563 gigachain-0.2.0/langchain/document_loaders/obsidian.py
+-rw-r--r--   0        0        0      662 2024-05-06 14:45:38.581302 gigachain-0.2.0/langchain/document_loaders/odt.py
+-rw-r--r--   0        0        0      641 2024-05-06 14:45:38.582248 gigachain-0.2.0/langchain/document_loaders/onedrive.py
+-rw-r--r--   0        0        0      653 2024-05-06 14:45:38.582845 gigachain-0.2.0/langchain/document_loaders/onedrive_file.py
+-rw-r--r--   0        0        0      654 2024-05-06 14:45:38.583452 gigachain-0.2.0/langchain/document_loaders/onenote.py
+-rw-r--r--   0        0        0      653 2024-05-06 14:45:38.584049 gigachain-0.2.0/langchain/document_loaders/open_city_data.py
+-rw-r--r--   0        0        0      680 2024-05-06 14:45:38.584552 gigachain-0.2.0/langchain/document_loaders/org_mode.py
+-rw-r--r--   0        0        0     2142 2024-05-06 14:45:38.585333 gigachain-0.2.0/langchain/document_loaders/parsers/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-06 14:45:38.586083 gigachain-0.2.0/langchain/document_loaders/parsers/audio.py
+-rw-r--r--   0        0        0      821 2024-05-06 14:45:38.586655 gigachain-0.2.0/langchain/document_loaders/parsers/docai.py
+-rw-r--r--   0        0        0      694 2024-05-06 14:45:38.587301 gigachain-0.2.0/langchain/document_loaders/parsers/generic.py
+-rw-r--r--   0        0        0      848 2024-05-06 14:45:38.588436 gigachain-0.2.0/langchain/document_loaders/parsers/grobid.py
+-rw-r--r--   0        0        0      678 2024-05-06 14:45:38.589052 gigachain-0.2.0/langchain/document_loaders/parsers/html/__init__.py
+-rw-r--r--   0        0        0      678 2024-05-06 14:45:38.589683 gigachain-0.2.0/langchain/document_loaders/parsers/html/bs4.py
+-rw-r--r--   0        0        0      747 2024-05-06 14:45:38.590301 gigachain-0.2.0/langchain/document_loaders/parsers/language/__init__.py
+-rw-r--r--   0        0        0      710 2024-05-06 14:45:38.590797 gigachain-0.2.0/langchain/document_loaders/parsers/language/cobol.py
+-rw-r--r--   0        0        0      742 2024-05-06 14:45:38.591306 gigachain-0.2.0/langchain/document_loaders/parsers/language/code_segmenter.py
+-rw-r--r--   0        0        0      752 2024-05-06 14:45:38.591872 gigachain-0.2.0/langchain/document_loaders/parsers/language/javascript.py
+-rw-r--r--   0        0        0      747 2024-05-06 14:45:38.592401 gigachain-0.2.0/langchain/document_loaders/parsers/language/language_parser.py
+-rw-r--r--   0        0        0      715 2024-05-24 11:13:19.261775 gigachain-0.2.0/langchain/document_loaders/parsers/language/python.py
+-rw-r--r--   0        0        0      671 2024-05-06 14:45:38.592917 gigachain-0.2.0/langchain/document_loaders/parsers/msword.py
+-rw-r--r--   0        0        0     1662 2024-05-06 14:45:38.593463 gigachain-0.2.0/langchain/document_loaders/parsers/pdf.py
+-rw-r--r--   0        0        0      669 2024-05-06 14:45:38.594347 gigachain-0.2.0/langchain/document_loaders/parsers/registry.py
+-rw-r--r--   0        0        0      653 2024-05-06 14:45:38.594869 gigachain-0.2.0/langchain/document_loaders/parsers/txt.py
+-rw-r--r--   0        0        0     2181 2024-05-06 14:45:38.595348 gigachain-0.2.0/langchain/document_loaders/pdf.py
+-rw-r--r--   0        0        0      662 2024-05-06 14:45:38.595872 gigachain-0.2.0/langchain/document_loaders/polars_dataframe.py
+-rw-r--r--   0        0        0      689 2024-05-06 14:45:38.596341 gigachain-0.2.0/langchain/document_loaders/powerpoint.py
+-rw-r--r--   0        0        0      638 2024-05-06 14:45:38.596856 gigachain-0.2.0/langchain/document_loaders/psychic.py
+-rw-r--r--   0        0        0      635 2024-05-06 14:45:38.597362 gigachain-0.2.0/langchain/document_loaders/pubmed.py
+-rw-r--r--   0        0        0      718 2024-05-24 11:13:19.262754 gigachain-0.2.0/langchain/document_loaders/pyspark_dataframe.py
+-rw-r--r--   0        0        0      643 2024-05-24 11:13:19.263485 gigachain-0.2.0/langchain/document_loaders/python.py
+-rw-r--r--   0        0        0      639 2024-05-06 14:45:38.597853 gigachain-0.2.0/langchain/document_loaders/quip.py
+-rw-r--r--   0        0        0      650 2024-05-06 14:45:38.598430 gigachain-0.2.0/langchain/document_loaders/readthedocs.py
+-rw-r--r--   0        0        0      653 2024-05-06 14:45:38.599220 gigachain-0.2.0/langchain/document_loaders/recursive_url_loader.py
+-rw-r--r--   0        0        0      650 2024-05-06 14:45:38.599730 gigachain-0.2.0/langchain/document_loaders/reddit.py
+-rw-r--r--   0        0        0      629 2024-05-06 14:45:38.600347 gigachain-0.2.0/langchain/document_loaders/roam.py
+-rw-r--r--   0        0        0      638 2024-05-06 14:45:38.601392 gigachain-0.2.0/langchain/document_loaders/rocksetdb.py
+-rw-r--r--   0        0        0      649 2024-05-06 14:45:38.601921 gigachain-0.2.0/langchain/document_loaders/rspace.py
+-rw-r--r--   0        0        0      638 2024-05-06 14:45:38.602430 gigachain-0.2.0/langchain/document_loaders/rss.py
+-rw-r--r--   0        0        0      662 2024-05-06 14:45:38.602910 gigachain-0.2.0/langchain/document_loaders/rst.py
+-rw-r--r--   0        0        0      662 2024-05-06 14:45:38.603493 gigachain-0.2.0/langchain/document_loaders/rtf.py
+-rw-r--r--   0        0        0      650 2024-05-06 14:45:38.605590 gigachain-0.2.0/langchain/document_loaders/s3_directory.py
+-rw-r--r--   0        0        0      635 2024-05-06 14:45:38.611153 gigachain-0.2.0/langchain/document_loaders/s3_file.py
+-rw-r--r--   0        0        0      647 2024-05-06 14:45:38.668492 gigachain-0.2.0/langchain/document_loaders/sharepoint.py
+-rw-r--r--   0        0        0      638 2024-05-06 14:45:38.672239 gigachain-0.2.0/langchain/document_loaders/sitemap.py
+-rw-r--r--   0        0        0      659 2024-05-06 14:45:38.673280 gigachain-0.2.0/langchain/document_loaders/slack_directory.py
+-rw-r--r--   0        0        0      644 2024-05-06 14:45:38.674909 gigachain-0.2.0/langchain/document_loaders/snowflake_loader.py
+-rw-r--r--   0        0        0      641 2024-05-06 14:45:38.675640 gigachain-0.2.0/langchain/document_loaders/spreedly.py
+-rw-r--r--   0        0        0      626 2024-05-06 14:45:38.676269 gigachain-0.2.0/langchain/document_loaders/srt.py
+-rw-r--r--   0        0        0      635 2024-05-06 14:45:38.677191 gigachain-0.2.0/langchain/document_loaders/stripe.py
+-rw-r--r--   0        0        0     1122 2024-05-06 14:45:38.677841 gigachain-0.2.0/langchain/document_loaders/telegram.py
+-rw-r--r--   0        0        0      680 2024-05-06 14:45:38.678926 gigachain-0.2.0/langchain/document_loaders/tencent_cos_directory.py
+-rw-r--r--   0        0        0      659 2024-05-06 14:45:38.679562 gigachain-0.2.0/langchain/document_loaders/tencent_cos_file.py
+-rw-r--r--   0        0        0      668 2024-05-06 14:45:38.682907 gigachain-0.2.0/langchain/document_loaders/tensorflow_datasets.py
+-rw-r--r--   0        0        0      629 2024-05-06 14:45:38.683558 gigachain-0.2.0/langchain/document_loaders/text.py
+-rw-r--r--   0        0        0      647 2024-05-06 14:45:38.684105 gigachain-0.2.0/langchain/document_loaders/tomarkdown.py
+-rw-r--r--   0        0        0      629 2024-05-06 14:45:38.684726 gigachain-0.2.0/langchain/document_loaders/toml.py
+-rw-r--r--   0        0        0      635 2024-05-06 14:45:38.685196 gigachain-0.2.0/langchain/document_loaders/trello.py
+-rw-r--r--   0        0        0      662 2024-05-06 14:45:38.685716 gigachain-0.2.0/langchain/document_loaders/tsv.py
+-rw-r--r--   0        0        0      653 2024-05-06 14:45:38.686300 gigachain-0.2.0/langchain/document_loaders/twitter.py
+-rw-r--r--   0        0        0     1855 2024-05-06 14:45:38.686889 gigachain-0.2.0/langchain/document_loaders/unstructured.py
+-rw-r--r--   0        0        0      662 2024-05-06 14:45:38.687421 gigachain-0.2.0/langchain/document_loaders/url.py
+-rw-r--r--   0        0        0     1033 2024-05-06 14:45:38.688032 gigachain-0.2.0/langchain/document_loaders/url_playwright.py
+-rw-r--r--   0        0        0      650 2024-05-06 14:45:38.688578 gigachain-0.2.0/langchain/document_loaders/url_selenium.py
+-rw-r--r--   0        0        0      650 2024-05-06 14:45:38.689107 gigachain-0.2.0/langchain/document_loaders/weather.py
+-rw-r--r--   0        0        0      638 2024-05-06 14:45:38.689674 gigachain-0.2.0/langchain/document_loaders/web_base.py
+-rw-r--r--   0        0        0      846 2024-05-06 14:45:38.690197 gigachain-0.2.0/langchain/document_loaders/whatsapp_chat.py
+-rw-r--r--   0        0        0      644 2024-05-06 14:45:38.690718 gigachain-0.2.0/langchain/document_loaders/wikipedia.py
+-rw-r--r--   0        0        0      821 2024-05-06 14:45:38.691226 gigachain-0.2.0/langchain/document_loaders/word_document.py
+-rw-r--r--   0        0        0      662 2024-05-06 14:45:38.691744 gigachain-0.2.0/langchain/document_loaders/xml.py
+-rw-r--r--   0        0        0      638 2024-05-06 14:45:38.692267 gigachain-0.2.0/langchain/document_loaders/xorbits.py
+-rw-r--r--   0        0        0      905 2024-05-06 14:45:38.692772 gigachain-0.2.0/langchain/document_loaders/youtube.py
+-rw-r--r--   0        0        0     2573 2024-05-06 14:45:38.693908 gigachain-0.2.0/langchain/document_transformers/__init__.py
+-rw-r--r--   0        0        0      687 2024-05-06 14:45:38.694471 gigachain-0.2.0/langchain/document_transformers/beautiful_soup_transformer.py
+-rw-r--r--   0        0        0      687 2024-05-06 14:45:38.694956 gigachain-0.2.0/langchain/document_transformers/doctran_text_extract.py
+-rw-r--r--   0        0        0      675 2024-05-06 14:45:38.695440 gigachain-0.2.0/langchain/document_transformers/doctran_text_qa.py
+-rw-r--r--   0        0        0      678 2024-05-06 14:45:38.695956 gigachain-0.2.0/langchain/document_transformers/doctran_text_translate.py
+-rw-r--r--   0        0        0     1667 2024-05-06 14:45:38.696506 gigachain-0.2.0/langchain/document_transformers/embeddings_redundant_filter.py
+-rw-r--r--   0        0        0      693 2024-05-06 14:45:38.697121 gigachain-0.2.0/langchain/document_transformers/google_translate.py
+-rw-r--r--   0        0        0      675 2024-05-06 14:45:38.697640 gigachain-0.2.0/langchain/document_transformers/html2text.py
+-rw-r--r--   0        0        0     2042 2023-10-30 16:05:53.900619 gigachain-0.2.0/langchain/document_transformers/loading.py
+-rw-r--r--   0        0        0      663 2024-05-06 14:45:38.698142 gigachain-0.2.0/langchain/document_transformers/long_context_reorder.py
+-rw-r--r--   0        0        0      678 2024-05-06 14:45:38.698665 gigachain-0.2.0/langchain/document_transformers/nuclia_text_transform.py
+-rw-r--r--   0        0        0      929 2024-05-06 14:45:38.699179 gigachain-0.2.0/langchain/document_transformers/openai_functions.py
+-rw-r--r--   0        0        0     2103 2023-10-30 16:05:53.902104 gigachain-0.2.0/langchain/document_transformers/serializers.py
+-rw-r--r--   0        0        0     6033 2023-10-06 14:43:01.456268 gigachain-0.2.0/langchain/document_transformers/xsl/html_chunks_with_headers.xslt
+-rw-r--r--   0        0        0     8313 2024-05-06 14:45:38.701353 gigachain-0.2.0/langchain/embeddings/__init__.py
+-rw-r--r--   0        0        0      890 2024-05-06 14:45:38.702121 gigachain-0.2.0/langchain/embeddings/aleph_alpha.py
+-rw-r--r--   0        0        0      626 2024-05-06 14:45:38.702686 gigachain-0.2.0/langchain/embeddings/awa.py
+-rw-r--r--   0        0        0      650 2024-05-06 14:45:38.703264 gigachain-0.2.0/langchain/embeddings/azure_openai.py
+-rw-r--r--   0        0        0      662 2024-05-06 14:45:38.703770 gigachain-0.2.0/langchain/embeddings/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0      113 2023-12-18 12:05:47.286522 gigachain-0.2.0/langchain/embeddings/base.py
+-rw-r--r--   0        0        0      638 2024-05-06 14:45:38.704384 gigachain-0.2.0/langchain/embeddings/bedrock.py
+-rw-r--r--   0        0        0      638 2024-05-06 14:45:38.704919 gigachain-0.2.0/langchain/embeddings/bookend.py
+-rw-r--r--   0        0        0    10207 2024-05-24 11:13:19.264952 gigachain-0.2.0/langchain/embeddings/cache.py
+-rw-r--r--   0        0        0      641 2024-05-06 14:45:38.705439 gigachain-0.2.0/langchain/embeddings/clarifai.py
+-rw-r--r--   0        0        0      756 2024-05-06 14:45:38.705976 gigachain-0.2.0/langchain/embeddings/cloudflare_workersai.py
+-rw-r--r--   0        0        0      635 2024-05-06 14:45:38.706439 gigachain-0.2.0/langchain/embeddings/cohere.py
+-rw-r--r--   0        0        0      644 2024-05-06 14:45:38.706919 gigachain-0.2.0/langchain/embeddings/dashscope.py
+-rw-r--r--   0        0        0      647 2024-05-06 14:45:38.707532 gigachain-0.2.0/langchain/embeddings/databricks.py
+-rw-r--r--   0        0        0      644 2024-05-06 14:45:38.708063 gigachain-0.2.0/langchain/embeddings/deepinfra.py
+-rw-r--r--   0        0        0      635 2024-05-06 14:45:38.708572 gigachain-0.2.0/langchain/embeddings/edenai.py
+-rw-r--r--   0        0        0      656 2024-05-06 14:45:38.709080 gigachain-0.2.0/langchain/embeddings/elasticsearch.py
+-rw-r--r--   0        0        0      635 2024-05-06 14:45:38.709561 gigachain-0.2.0/langchain/embeddings/embaas.py
+-rw-r--r--   0        0        0      632 2024-05-06 14:45:38.710058 gigachain-0.2.0/langchain/embeddings/ernie.py
+-rw-r--r--   0        0        0      791 2024-05-06 14:45:38.710619 gigachain-0.2.0/langchain/embeddings/fake.py
+-rw-r--r--   0        0        0      644 2024-05-06 14:45:38.711084 gigachain-0.2.0/langchain/embeddings/fastembed.py
+-rw-r--r--   0        0        0      647 2024-05-06 14:45:38.711639 gigachain-0.2.0/langchain/embeddings/google_palm.py
+-rw-r--r--   0        0        0      638 2024-05-06 14:45:38.712176 gigachain-0.2.0/langchain/embeddings/gpt4all.py
+-rw-r--r--   0        0        0      641 2024-05-06 14:45:38.712701 gigachain-0.2.0/langchain/embeddings/gradient_ai.py
+-rw-r--r--   0        0        0     1112 2024-05-06 14:45:38.713220 gigachain-0.2.0/langchain/embeddings/huggingface.py
+-rw-r--r--   0        0        0      659 2024-05-06 14:45:38.713762 gigachain-0.2.0/langchain/embeddings/huggingface_hub.py
+-rw-r--r--   0        0        0      895 2024-05-06 14:45:38.714299 gigachain-0.2.0/langchain/embeddings/infinity.py
+-rw-r--r--   0        0        0      665 2024-05-06 14:45:38.714806 gigachain-0.2.0/langchain/embeddings/javelin_ai_gateway.py
+-rw-r--r--   0        0        0      629 2024-05-06 14:45:38.715342 gigachain-0.2.0/langchain/embeddings/jina.py
+-rw-r--r--   0        0        0      653 2024-05-06 14:45:38.715966 gigachain-0.2.0/langchain/embeddings/johnsnowlabs.py
+-rw-r--r--   0        0        0      641 2024-05-06 14:45:38.716489 gigachain-0.2.0/langchain/embeddings/llamacpp.py
+-rw-r--r--   0        0        0      641 2024-05-06 14:45:38.716988 gigachain-0.2.0/langchain/embeddings/llm_rails.py
+-rw-r--r--   0        0        0      638 2024-05-06 14:45:38.717456 gigachain-0.2.0/langchain/embeddings/localai.py
+-rw-r--r--   0        0        0      638 2024-05-06 14:45:38.717900 gigachain-0.2.0/langchain/embeddings/minimax.py
+-rw-r--r--   0        0        0      635 2024-05-06 14:45:38.718936 gigachain-0.2.0/langchain/embeddings/mlflow.py
+-rw-r--r--   0        0        0      662 2024-05-06 14:45:38.719500 gigachain-0.2.0/langchain/embeddings/mlflow_gateway.py
+-rw-r--r--   0        0        0      647 2024-05-06 14:45:38.720062 gigachain-0.2.0/langchain/embeddings/modelscope_hub.py
+-rw-r--r--   0        0        0      671 2024-05-06 14:45:38.720607 gigachain-0.2.0/langchain/embeddings/mosaicml.py
+-rw-r--r--   0        0        0      641 2024-05-06 14:45:38.721120 gigachain-0.2.0/langchain/embeddings/nlpcloud.py
+-rw-r--r--   0        0        0      635 2024-05-06 14:45:38.721635 gigachain-0.2.0/langchain/embeddings/octoai_embeddings.py
+-rw-r--r--   0        0        0      635 2024-05-06 14:45:38.722111 gigachain-0.2.0/langchain/embeddings/ollama.py
+-rw-r--r--   0        0        0      635 2024-05-06 14:45:38.722616 gigachain-0.2.0/langchain/embeddings/openai.py
+-rw-r--r--   0        0        0      900 2024-05-06 14:45:38.723126 gigachain-0.2.0/langchain/embeddings/sagemaker_endpoint.py
+-rw-r--r--   0        0        0      647 2024-05-06 14:45:38.723708 gigachain-0.2.0/langchain/embeddings/self_hosted.py
+-rw-r--r--   0        0        0      881 2024-05-06 14:45:38.724577 gigachain-0.2.0/langchain/embeddings/self_hosted_hugging_face.py
+-rw-r--r--   0        0        0      667 2024-05-24 11:13:19.265645 gigachain-0.2.0/langchain/embeddings/sentence_transformer.py
+-rw-r--r--   0        0        0      632 2024-05-06 14:45:38.725277 gigachain-0.2.0/langchain/embeddings/spacy_embeddings.py
+-rw-r--r--   0        0        0      656 2024-05-06 14:45:38.725829 gigachain-0.2.0/langchain/embeddings/tensorflow_hub.py
+-rw-r--r--   0        0        0      641 2024-05-06 14:45:38.726318 gigachain-0.2.0/langchain/embeddings/vertexai.py
+-rw-r--r--   0        0        0      635 2024-05-06 14:45:38.726799 gigachain-0.2.0/langchain/embeddings/voyageai.py
+-rw-r--r--   0        0        0      647 2024-05-06 14:45:38.727278 gigachain-0.2.0/langchain/embeddings/xinference.py
+-rw-r--r--   0        0        0      476 2023-08-21 13:51:28.799282 gigachain-0.2.0/langchain/env.py
+-rw-r--r--   0        0        0     5803 2024-04-19 07:38:34.000540 gigachain-0.2.0/langchain/evaluation/__init__.py
+-rw-r--r--   0        0        0      166 2024-04-19 07:38:34.001406 gigachain-0.2.0/langchain/evaluation/agents/__init__.py
+-rw-r--r--   0        0        0    13915 2024-04-19 07:38:34.001878 gigachain-0.2.0/langchain/evaluation/agents/trajectory_eval_chain.py
+-rw-r--r--   0        0        0     9689 2024-04-19 07:38:34.003102 gigachain-0.2.0/langchain/evaluation/agents/trajectory_eval_prompt.py
+-rw-r--r--   0        0        0     1401 2024-04-19 07:38:34.004003 gigachain-0.2.0/langchain/evaluation/comparison/__init__.py
+-rw-r--r--   0        0        0    15935 2024-05-06 14:45:38.728624 gigachain-0.2.0/langchain/evaluation/comparison/eval_chain.py
+-rw-r--r--   0        0        0     2359 2024-04-19 07:38:34.005613 gigachain-0.2.0/langchain/evaluation/comparison/prompt.py
+-rw-r--r--   0        0        0     1647 2024-01-18 15:16:40.716003 gigachain-0.2.0/langchain/evaluation/criteria/__init__.py
+-rw-r--r--   0        0        0    21304 2024-05-06 14:45:38.730097 gigachain-0.2.0/langchain/evaluation/criteria/eval_chain.py
+-rw-r--r--   0        0        0     2723 2023-12-18 12:05:47.336070 gigachain-0.2.0/langchain/evaluation/criteria/prompt.py
+-rw-r--r--   0        0        0      324 2024-04-19 07:38:34.007101 gigachain-0.2.0/langchain/evaluation/embedding_distance/__init__.py
+-rw-r--r--   0        0        0    17096 2024-05-24 11:13:19.266877 gigachain-0.2.0/langchain/evaluation/embedding_distance/base.py
+-rw-r--r--   0        0        0        0 2023-10-03 07:51:15.890624 gigachain-0.2.0/langchain/evaluation/exact_match/__init__.py
+-rw-r--r--   0        0        0     2751 2023-10-03 07:51:15.891318 gigachain-0.2.0/langchain/evaluation/exact_match/base.py
+-rw-r--r--   0        0        0     7328 2024-05-06 14:45:38.732958 gigachain-0.2.0/langchain/evaluation/loading.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.807950 gigachain-0.2.0/langchain/evaluation/parsing/__init__.py
+-rw-r--r--   0        0        0     5242 2024-05-06 14:45:38.733928 gigachain-0.2.0/langchain/evaluation/parsing/base.py
+-rw-r--r--   0        0        0     3662 2024-05-06 14:45:38.734346 gigachain-0.2.0/langchain/evaluation/parsing/json_distance.py
+-rw-r--r--   0        0        0     3180 2024-05-06 14:45:38.734863 gigachain-0.2.0/langchain/evaluation/parsing/json_schema.py
+-rw-r--r--   0        0        0      345 2024-04-19 07:38:34.011427 gigachain-0.2.0/langchain/evaluation/qa/__init__.py
+-rw-r--r--   0        0        0    10892 2024-04-19 07:38:34.013030 gigachain-0.2.0/langchain/evaluation/qa/eval_chain.py
+-rw-r--r--   0        0        0     6525 2023-12-18 12:05:47.340520 gigachain-0.2.0/langchain/evaluation/qa/eval_prompt.py
+-rw-r--r--   0        0        0     1053 2024-04-19 07:38:34.014495 gigachain-0.2.0/langchain/evaluation/qa/generate_chain.py
+-rw-r--r--   0        0        0      917 2023-12-18 12:05:47.341977 gigachain-0.2.0/langchain/evaluation/qa/generate_prompt.py
+-rw-r--r--   0        0        0        0 2023-10-03 07:51:15.892405 gigachain-0.2.0/langchain/evaluation/regex_match/__init__.py
+-rw-r--r--   0        0        0     2407 2023-10-03 07:51:15.893632 gigachain-0.2.0/langchain/evaluation/regex_match/base.py
+-rw-r--r--   0        0        0    18198 2024-04-19 07:38:34.015691 gigachain-0.2.0/langchain/evaluation/schema.py
+-rw-r--r--   0        0        0     1113 2024-04-19 07:38:34.016568 gigachain-0.2.0/langchain/evaluation/scoring/__init__.py
+-rw-r--r--   0        0        0    15477 2024-05-24 11:13:19.268593 gigachain-0.2.0/langchain/evaluation/scoring/eval_chain.py
+-rw-r--r--   0        0        0     2130 2024-04-19 07:38:34.018364 gigachain-0.2.0/langchain/evaluation/scoring/prompt.py
+-rw-r--r--   0        0        0      286 2024-04-19 07:38:34.019368 gigachain-0.2.0/langchain/evaluation/string_distance/__init__.py
+-rw-r--r--   0        0        0    14019 2024-04-19 07:38:34.020480 gigachain-0.2.0/langchain/evaluation/string_distance/base.py
+-rw-r--r--   0        0        0      142 2024-04-19 07:38:34.021715 gigachain-0.2.0/langchain/example_generator.py
+-rw-r--r--   0        0        0      168 2024-04-19 07:38:34.022793 gigachain-0.2.0/langchain/formatting.py
+-rw-r--r--   0        0        0     7436 2024-04-19 07:38:34.024025 gigachain-0.2.0/langchain/globals/__init__.py
+-rw-r--r--   0        0        0     1527 2024-05-06 14:45:38.735475 gigachain-0.2.0/langchain/graphs/__init__.py
+-rw-r--r--   0        0        0      796 2024-05-06 14:45:38.735870 gigachain-0.2.0/langchain/graphs/arangodb_graph.py
+-rw-r--r--   0        0        0      618 2024-05-06 14:45:38.736210 gigachain-0.2.0/langchain/graphs/falkordb_graph.py
+-rw-r--r--   0        0        0      862 2024-05-06 14:45:38.736533 gigachain-0.2.0/langchain/graphs/graph_document.py
+-rw-r--r--   0        0        0      633 2024-05-06 14:45:38.736903 gigachain-0.2.0/langchain/graphs/graph_store.py
+-rw-r--r--   0        0        0      606 2024-05-06 14:45:38.737235 gigachain-0.2.0/langchain/graphs/hugegraph.py
+-rw-r--r--   0        0        0      606 2024-05-06 14:45:38.737570 gigachain-0.2.0/langchain/graphs/kuzu_graph.py
+-rw-r--r--   0        0        0      618 2024-05-06 14:45:38.737892 gigachain-0.2.0/langchain/graphs/memgraph_graph.py
+-rw-r--r--   0        0        0      612 2024-05-06 14:45:38.738228 gigachain-0.2.0/langchain/graphs/nebula_graph.py
+-rw-r--r--   0        0        0      609 2024-05-06 14:45:38.738564 gigachain-0.2.0/langchain/graphs/neo4j_graph.py
+-rw-r--r--   0        0        0      615 2024-05-06 14:45:38.738890 gigachain-0.2.0/langchain/graphs/neptune_graph.py
+-rw-r--r--   0        0        0     1042 2024-05-06 14:45:38.739436 gigachain-0.2.0/langchain/graphs/networkx_graph.py
+-rw-r--r--   0        0        0      603 2024-05-06 14:45:38.739967 gigachain-0.2.0/langchain/graphs/rdf_graph.py
+-rw-r--r--   0        0        0     3462 2024-05-06 14:45:38.740317 gigachain-0.2.0/langchain/hub.py
+-rw-r--r--   0        0        0     1480 2024-05-24 11:13:19.269294 gigachain-0.2.0/langchain/indexes/__init__.py
+-rw-r--r--   0        0        0      252 2024-05-06 14:45:38.741076 gigachain-0.2.0/langchain/indexes/_api.py
+-rw-r--r--   0        0        0    20641 2024-05-06 14:45:38.742323 gigachain-0.2.0/langchain/indexes/_sql_record_manager.py
+-rw-r--r--   0        0        0      906 2024-05-24 11:13:19.269998 gigachain-0.2.0/langchain/indexes/graph.py
+-rw-r--r--   0        0        0      357 2024-05-06 14:45:38.743487 gigachain-0.2.0/langchain/indexes/prompts/__init__.py
+-rw-r--r--   0        0        0     3241 2023-12-18 12:05:47.364265 gigachain-0.2.0/langchain/indexes/prompts/entity_extraction.py
+-rw-r--r--   0        0        0     1797 2023-12-18 12:05:47.365149 gigachain-0.2.0/langchain/indexes/prompts/entity_summarization.py
+-rw-r--r--   0        0        0     2231 2024-05-24 11:13:19.271291 gigachain-0.2.0/langchain/indexes/prompts/knowledge_triplet_extraction.py
+-rw-r--r--   0        0        0     7067 2024-05-24 11:13:19.272030 gigachain-0.2.0/langchain/indexes/vectorstore.py
+-rw-r--r--   0        0        0      283 2024-04-19 07:38:34.032341 gigachain-0.2.0/langchain/input.py
+-rw-r--r--   0        0        0    17117 2024-05-24 11:13:19.273678 gigachain-0.2.0/langchain/llms/__init__.py
+-rw-r--r--   0        0        0      735 2024-05-06 14:45:38.746584 gigachain-0.2.0/langchain/llms/ai21.py
+-rw-r--r--   0        0        0      605 2024-05-06 14:45:38.747153 gigachain-0.2.0/langchain/llms/aleph_alpha.py
+-rw-r--r--   0        0        0      623 2024-05-06 14:45:38.747686 gigachain-0.2.0/langchain/llms/amazon_api_gateway.py
+-rw-r--r--   0        0        0      602 2024-05-06 14:45:38.748438 gigachain-0.2.0/langchain/llms/anthropic.py
+-rw-r--r--   0        0        0      599 2024-05-06 14:45:38.749053 gigachain-0.2.0/langchain/llms/anyscale.py
+-rw-r--r--   0        0        0      590 2024-05-06 14:45:38.749600 gigachain-0.2.0/langchain/llms/arcee.py
+-rw-r--r--   0        0        0      593 2024-05-06 14:45:38.750258 gigachain-0.2.0/langchain/llms/aviary.py
+-rw-r--r--   0        0        0     1649 2024-05-06 14:45:38.750816 gigachain-0.2.0/langchain/llms/azureml_endpoint.py
+-rw-r--r--   0        0        0      629 2024-05-06 14:45:38.751614 gigachain-0.2.0/langchain/llms/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0      593 2024-05-06 14:45:38.752417 gigachain-0.2.0/langchain/llms/bananadev.py
+-rw-r--r--   0        0        0      228 2024-01-10 09:04:40.449816 gigachain-0.2.0/langchain/llms/base.py
+-rw-r--r--   0        0        0      596 2024-05-06 14:45:38.752987 gigachain-0.2.0/langchain/llms/baseten.py
+-rw-r--r--   0        0        0      587 2024-05-06 14:45:38.753504 gigachain-0.2.0/langchain/llms/beam.py
+-rw-r--r--   0        0        0      738 2024-05-06 14:45:38.754052 gigachain-0.2.0/langchain/llms/bedrock.py
+-rw-r--r--   0        0        0      617 2024-05-06 14:45:38.754651 gigachain-0.2.0/langchain/llms/bittensor.py
+-rw-r--r--   0        0        0      608 2024-05-06 14:45:38.755111 gigachain-0.2.0/langchain/llms/cerebriumai.py
+-rw-r--r--   0        0        0      596 2024-05-06 14:45:38.755529 gigachain-0.2.0/langchain/llms/chatglm.py
+-rw-r--r--   0        0        0      599 2024-05-06 14:45:38.756029 gigachain-0.2.0/langchain/llms/clarifai.py
+-rw-r--r--   0        0        0      680 2024-05-06 14:45:38.756652 gigachain-0.2.0/langchain/llms/cloudflare_workersai.py
+-rw-r--r--   0        0        0      593 2024-05-06 14:45:38.757246 gigachain-0.2.0/langchain/llms/cohere.py
+-rw-r--r--   0        0        0      614 2024-05-06 14:45:38.757800 gigachain-0.2.0/langchain/llms/ctransformers.py
+-rw-r--r--   0        0        0      608 2024-05-06 14:45:38.758285 gigachain-0.2.0/langchain/llms/ctranslate2.py
+-rw-r--r--   0        0        0      605 2024-05-06 14:45:38.758827 gigachain-0.2.0/langchain/llms/databricks.py
+-rw-r--r--   0        0        0      602 2024-05-06 14:45:38.759355 gigachain-0.2.0/langchain/llms/deepinfra.py
+-rw-r--r--   0        0        0      605 2024-05-06 14:45:38.760001 gigachain-0.2.0/langchain/llms/deepsparse.py
+-rw-r--r--   0        0        0      593 2024-05-06 14:45:38.760652 gigachain-0.2.0/langchain/llms/edenai.py
+-rw-r--r--   0        0        0      777 2024-05-24 11:13:19.274286 gigachain-0.2.0/langchain/llms/fake.py
+-rw-r--r--   0        0        0      602 2024-05-06 14:45:38.762001 gigachain-0.2.0/langchain/llms/fireworks.py
+-rw-r--r--   0        0        0      608 2024-05-06 14:45:38.762598 gigachain-0.2.0/langchain/llms/forefrontai.py
+-rw-r--r--   0        0        0      599 2024-05-06 14:45:38.763135 gigachain-0.2.0/langchain/llms/gigachat.py
+-rw-r--r--   0        0        0      605 2024-05-06 14:45:38.763693 gigachain-0.2.0/langchain/llms/google_palm.py
+-rw-r--r--   0        0        0      596 2024-05-06 14:45:38.764263 gigachain-0.2.0/langchain/llms/gooseai.py
+-rw-r--r--   0        0        0      596 2024-05-06 14:45:38.764922 gigachain-0.2.0/langchain/llms/gpt4all.py
+-rw-r--r--   0        0        0      758 2024-05-06 14:45:38.765525 gigachain-0.2.0/langchain/llms/gradient_ai.py
+-rw-r--r--   0        0        0      664 2023-08-29 13:18:02.701979 gigachain-0.2.0/langchain/llms/grammars/json.gbnf
+-rw-r--r--   0        0        0      167 2023-08-29 13:18:02.702167 gigachain-0.2.0/langchain/llms/grammars/list.gbnf
+-rw-r--r--   0        0        0      632 2024-05-06 14:45:38.766149 gigachain-0.2.0/langchain/llms/huggingface_endpoint.py
+-rw-r--r--   0        0        0      617 2024-05-06 14:45:38.766771 gigachain-0.2.0/langchain/llms/huggingface_hub.py
+-rw-r--r--   0        0        0      632 2024-05-06 14:45:38.767280 gigachain-0.2.0/langchain/llms/huggingface_pipeline.py
+-rw-r--r--   0        0        0      656 2024-05-06 14:45:38.767904 gigachain-0.2.0/langchain/llms/huggingface_text_gen_inference.py
+-rw-r--r--   0        0        0      614 2024-05-06 14:45:38.768469 gigachain-0.2.0/langchain/llms/human.py
+-rw-r--r--   0        0        0      772 2024-05-06 14:45:38.769017 gigachain-0.2.0/langchain/llms/javelin_ai_gateway.py
+-rw-r--r--   0        0        0      611 2024-05-06 14:45:38.769614 gigachain-0.2.0/langchain/llms/koboldai.py
+-rw-r--r--   0        0        0      599 2024-05-06 14:45:38.770378 gigachain-0.2.0/langchain/llms/llamacpp.py
+-rw-r--r--   0        0        0      736 2024-05-06 14:45:38.770928 gigachain-0.2.0/langchain/llms/loading.py
+-rw-r--r--   0        0        0      620 2024-05-06 14:45:38.772756 gigachain-0.2.0/langchain/llms/manifest.py
+-rw-r--r--   0        0        0      596 2024-05-06 14:45:38.773255 gigachain-0.2.0/langchain/llms/minimax.py
+-rw-r--r--   0        0        0      593 2024-05-06 14:45:38.773833 gigachain-0.2.0/langchain/llms/mlflow.py
+-rw-r--r--   0        0        0      620 2024-05-06 14:45:38.774402 gigachain-0.2.0/langchain/llms/mlflow_ai_gateway.py
+-rw-r--r--   0        0        0      590 2024-05-06 14:45:38.774958 gigachain-0.2.0/langchain/llms/modal.py
+-rw-r--r--   0        0        0      599 2024-05-06 14:45:38.775540 gigachain-0.2.0/langchain/llms/mosaicml.py
+-rw-r--r--   0        0        0      599 2024-05-06 14:45:38.776064 gigachain-0.2.0/langchain/llms/nlpcloud.py
+-rw-r--r--   0        0        0      617 2024-05-06 14:45:38.776600 gigachain-0.2.0/langchain/llms/octoai_endpoint.py
+-rw-r--r--   0        0        0      593 2024-05-06 14:45:38.777113 gigachain-0.2.0/langchain/llms/ollama.py
+-rw-r--r--   0        0        0      614 2024-05-06 14:45:38.777619 gigachain-0.2.0/langchain/llms/opaqueprompts.py
+-rw-r--r--   0        0        0      885 2024-05-06 14:45:38.778125 gigachain-0.2.0/langchain/llms/openai.py
+-rw-r--r--   0        0        0      596 2024-05-06 14:45:38.778636 gigachain-0.2.0/langchain/llms/openllm.py
+-rw-r--r--   0        0        0      593 2024-05-06 14:45:38.779247 gigachain-0.2.0/langchain/llms/openlm.py
+-rw-r--r--   0        0        0      617 2024-05-06 14:45:38.779929 gigachain-0.2.0/langchain/llms/pai_eas_endpoint.py
+-rw-r--r--   0        0        0      593 2024-05-06 14:45:38.780502 gigachain-0.2.0/langchain/llms/petals.py
+-rw-r--r--   0        0        0      605 2024-05-06 14:45:38.783451 gigachain-0.2.0/langchain/llms/pipelineai.py
+-rw-r--r--   0        0        0      602 2024-05-06 14:45:38.784062 gigachain-0.2.0/langchain/llms/predibase.py
+-rw-r--r--   0        0        0      620 2024-05-06 14:45:38.786877 gigachain-0.2.0/langchain/llms/predictionguard.py
+-rw-r--r--   0        0        0      742 2024-05-06 14:45:38.790103 gigachain-0.2.0/langchain/llms/promptlayer_openai.py
+-rw-r--r--   0        0        0      602 2024-05-06 14:45:38.790891 gigachain-0.2.0/langchain/llms/replicate.py
+-rw-r--r--   0        0        0      587 2024-05-06 14:45:38.791561 gigachain-0.2.0/langchain/llms/rwkv.py
+-rw-r--r--   0        0        0      808 2024-05-06 14:45:38.792170 gigachain-0.2.0/langchain/llms/sagemaker_endpoint.py
+-rw-r--r--   0        0        0      629 2024-05-06 14:45:38.792772 gigachain-0.2.0/langchain/llms/self_hosted.py
+-rw-r--r--   0        0        0      647 2024-05-06 14:45:38.793329 gigachain-0.2.0/langchain/llms/self_hosted_hugging_face.py
+-rw-r--r--   0        0        0      611 2024-05-06 14:45:38.794027 gigachain-0.2.0/langchain/llms/stochasticai.py
+-rw-r--r--   0        0        0      593 2024-05-06 14:45:38.794746 gigachain-0.2.0/langchain/llms/symblai_nebula.py
+-rw-r--r--   0        0        0      596 2024-05-06 14:45:38.795485 gigachain-0.2.0/langchain/llms/textgen.py
+-rw-r--r--   0        0        0      611 2024-05-06 14:45:38.796101 gigachain-0.2.0/langchain/llms/titan_takeoff.py
+-rw-r--r--   0        0        0      620 2024-05-24 11:13:19.274908 gigachain-0.2.0/langchain/llms/titan_takeoff_pro.py
+-rw-r--r--   0        0        0      599 2024-05-06 14:45:38.797249 gigachain-0.2.0/langchain/llms/together.py
+-rw-r--r--   0        0        0      593 2024-05-06 14:45:38.797965 gigachain-0.2.0/langchain/llms/tongyi.py
+-rw-r--r--   0        0        0      644 2024-05-06 14:45:38.798528 gigachain-0.2.0/langchain/llms/utils.py
+-rw-r--r--   0        0        0      709 2024-05-06 14:45:38.799445 gigachain-0.2.0/langchain/llms/vertexai.py
+-rw-r--r--   0        0        0      670 2024-05-06 14:45:38.800065 gigachain-0.2.0/langchain/llms/vllm.py
+-rw-r--r--   0        0        0      805 2024-05-06 14:45:38.800678 gigachain-0.2.0/langchain/llms/volcengine_maas.py
+-rw-r--r--   0        0        0      605 2024-05-06 14:45:38.801233 gigachain-0.2.0/langchain/llms/watsonxllm.py
+-rw-r--r--   0        0        0      593 2024-05-06 14:45:38.801851 gigachain-0.2.0/langchain/llms/writer.py
+-rw-r--r--   0        0        0      605 2024-05-06 14:45:38.802399 gigachain-0.2.0/langchain/llms/xinference.py
+-rw-r--r--   0        0        0      602 2024-05-06 14:45:38.802987 gigachain-0.2.0/langchain/llms/yandex.py
+-rw-r--r--   0        0        0      207 2024-04-19 07:38:34.035339 gigachain-0.2.0/langchain/load/__init__.py
+-rw-r--r--   0        0        0      100 2023-12-18 12:05:47.446683 gigachain-0.2.0/langchain/load/dump.py
+-rw-r--r--   0        0        0       98 2023-12-18 12:05:47.447484 gigachain-0.2.0/langchain/load/load.py
+-rw-r--r--   0        0        0      412 2023-12-18 12:05:47.448066 gigachain-0.2.0/langchain/load/serializable.py
+-rw-r--r--   0        0        0     5389 2024-05-24 11:13:19.275871 gigachain-0.2.0/langchain/memory/__init__.py
+-rw-r--r--   0        0        0     4861 2024-02-22 08:54:03.274556 gigachain-0.2.0/langchain/memory/buffer.py
+-rw-r--r--   0        0        0     1616 2024-03-28 12:44:20.544688 gigachain-0.2.0/langchain/memory/buffer_window.py
+-rw-r--r--   0        0        0     2795 2024-05-06 14:45:38.803989 gigachain-0.2.0/langchain/memory/chat_memory.py
+-rw-r--r--   0        0        0     3506 2024-05-24 11:13:19.276839 gigachain-0.2.0/langchain/memory/chat_message_histories/__init__.py
+-rw-r--r--   0        0        0      692 2024-05-24 11:13:19.277819 gigachain-0.2.0/langchain/memory/chat_message_histories/astradb.py
+-rw-r--r--   0        0        0      698 2024-05-24 11:13:19.278698 gigachain-0.2.0/langchain/memory/chat_message_histories/cassandra.py
+-rw-r--r--   0        0        0      695 2024-05-24 11:13:19.279744 gigachain-0.2.0/langchain/memory/chat_message_histories/cosmos_db.py
+-rw-r--r--   0        0        0      695 2024-05-24 11:13:19.280287 gigachain-0.2.0/langchain/memory/chat_message_histories/dynamodb.py
+-rw-r--r--   0        0        0      727 2024-05-24 11:13:19.280837 gigachain-0.2.0/langchain/memory/chat_message_histories/elasticsearch.py
+-rw-r--r--   0        0        0      683 2024-05-24 11:13:19.281478 gigachain-0.2.0/langchain/memory/chat_message_histories/file.py
+-rw-r--r--   0        0        0      698 2024-05-24 11:13:19.281988 gigachain-0.2.0/langchain/memory/chat_message_histories/firestore.py
+-rw-r--r--   0        0        0      130 2024-05-24 11:13:19.283010 gigachain-0.2.0/langchain/memory/chat_message_histories/in_memory.py
+-rw-r--r--   0        0        0      692 2024-05-24 11:13:19.283994 gigachain-0.2.0/langchain/memory/chat_message_histories/momento.py
+-rw-r--r--   0        0        0      692 2024-05-24 11:13:19.284544 gigachain-0.2.0/langchain/memory/chat_message_histories/mongodb.py
+-rw-r--r--   0        0        0      686 2024-05-24 11:13:19.285073 gigachain-0.2.0/langchain/memory/chat_message_histories/neo4j.py
+-rw-r--r--   0        0        0      695 2024-05-24 11:13:19.285614 gigachain-0.2.0/langchain/memory/chat_message_histories/postgres.py
+-rw-r--r--   0        0        0      686 2024-05-24 11:13:19.286149 gigachain-0.2.0/langchain/memory/chat_message_histories/redis.py
+-rw-r--r--   0        0        0      692 2024-05-24 11:13:19.286938 gigachain-0.2.0/langchain/memory/chat_message_histories/rocksetdb.py
+-rw-r--r--   0        0        0      727 2024-05-24 11:13:19.287811 gigachain-0.2.0/langchain/memory/chat_message_histories/singlestoredb.py
+-rw-r--r--   0        0        0     1033 2024-05-24 11:13:19.288939 gigachain-0.2.0/langchain/memory/chat_message_histories/sql.py
+-rw-r--r--   0        0        0      698 2024-05-24 11:13:19.289594 gigachain-0.2.0/langchain/memory/chat_message_histories/streamlit.py
+-rw-r--r--   0        0        0      724 2024-05-24 11:13:19.290276 gigachain-0.2.0/langchain/memory/chat_message_histories/upstash_redis.py
+-rw-r--r--   0        0        0      683 2024-05-24 11:13:19.290887 gigachain-0.2.0/langchain/memory/chat_message_histories/xata.py
+-rw-r--r--   0        0        0      680 2024-05-24 11:13:19.291640 gigachain-0.2.0/langchain/memory/chat_message_histories/zep.py
+-rw-r--r--   0        0        0     2912 2023-12-18 12:05:47.480430 gigachain-0.2.0/langchain/memory/combined.py
+-rw-r--r--   0        0        0    15936 2024-05-24 11:13:19.292799 gigachain-0.2.0/langchain/memory/entity.py
+-rw-r--r--   0        0        0      645 2024-05-24 11:13:19.295441 gigachain-0.2.0/langchain/memory/kg.py
+-rw-r--r--   0        0        0      658 2024-05-24 11:13:19.296090 gigachain-0.2.0/langchain/memory/motorhead_memory.py
+-rw-r--r--   0        0        0    13128 2023-12-18 12:05:47.483791 gigachain-0.2.0/langchain/memory/prompt.py
+-rw-r--r--   0        0        0      792 2024-05-06 14:45:38.806610 gigachain-0.2.0/langchain/memory/readonly.py
+-rw-r--r--   0        0        0      761 2023-12-18 12:05:47.485293 gigachain-0.2.0/langchain/memory/simple.py
+-rw-r--r--   0        0        0     3389 2023-12-18 12:05:47.485998 gigachain-0.2.0/langchain/memory/summary.py
+-rw-r--r--   0        0        0     3043 2024-05-24 11:13:19.296691 gigachain-0.2.0/langchain/memory/summary_buffer.py
+-rw-r--r--   0        0        0     2144 2023-12-18 12:05:47.487927 gigachain-0.2.0/langchain/memory/token_buffer.py
+-rw-r--r--   0        0        0      617 2023-08-29 13:18:02.706587 gigachain-0.2.0/langchain/memory/utils.py
+-rw-r--r--   0        0        0     3875 2024-05-06 14:45:38.807664 gigachain-0.2.0/langchain/memory/vectorstore.py
+-rw-r--r--   0        0        0      628 2024-05-24 11:13:19.297427 gigachain-0.2.0/langchain/memory/zep_memory.py
+-rw-r--r--   0        0        0     3278 2024-02-22 08:54:03.280782 gigachain-0.2.0/langchain/model_laboratory.py
+-rw-r--r--   0        0        0     2719 2024-05-06 14:45:38.808804 gigachain-0.2.0/langchain/output_parsers/__init__.py
+-rw-r--r--   0        0        0     1689 2024-04-19 07:38:34.039563 gigachain-0.2.0/langchain/output_parsers/boolean.py
+-rw-r--r--   0        0        0     1799 2023-12-18 12:05:47.492673 gigachain-0.2.0/langchain/output_parsers/combining.py
+-rw-r--r--   0        0        0     1924 2024-02-22 08:54:03.283314 gigachain-0.2.0/langchain/output_parsers/datetime.py
+-rw-r--r--   0        0        0     1205 2023-12-18 12:05:47.494416 gigachain-0.2.0/langchain/output_parsers/enum.py
+-rw-r--r--   0        0        0     1427 2024-05-06 14:45:38.809506 gigachain-0.2.0/langchain/output_parsers/ernie_functions.py
+-rw-r--r--   0        0        0     3150 2024-05-06 14:45:38.810267 gigachain-0.2.0/langchain/output_parsers/fix.py
+-rw-r--r--   0        0        0     3958 2024-01-18 15:16:40.741558 gigachain-0.2.0/langchain/output_parsers/format_instructions.py
+-rw-r--r--   0        0        0      340 2024-04-19 07:38:34.040304 gigachain-0.2.0/langchain/output_parsers/json.py
+-rw-r--r--   0        0        0      310 2023-12-18 12:05:47.500021 gigachain-0.2.0/langchain/output_parsers/list.py
+-rw-r--r--   0        0        0      702 2023-08-21 13:51:28.860635 gigachain-0.2.0/langchain/output_parsers/loading.py
+-rw-r--r--   0        0        0      364 2024-03-28 12:44:20.546827 gigachain-0.2.0/langchain/output_parsers/openai_functions.py
+-rw-r--r--   0        0        0      229 2024-03-28 12:44:20.547235 gigachain-0.2.0/langchain/output_parsers/openai_tools.py
+-rw-r--r--   0        0        0     6548 2024-02-22 08:54:03.288456 gigachain-0.2.0/langchain/output_parsers/pandas_dataframe.py
+-rw-r--r--   0        0        0      699 2023-12-18 12:05:47.503286 gigachain-0.2.0/langchain/output_parsers/prompts.py
+-rw-r--r--   0        0        0       99 2024-03-28 12:44:20.547654 gigachain-0.2.0/langchain/output_parsers/pydantic.py
+-rw-r--r--   0        0        0      691 2024-05-06 14:45:38.813006 gigachain-0.2.0/langchain/output_parsers/rail_parser.py
+-rw-r--r--   0        0        0     1214 2023-12-18 12:05:47.506059 gigachain-0.2.0/langchain/output_parsers/regex.py
+-rw-r--r--   0        0        0     1709 2023-12-18 12:05:47.506885 gigachain-0.2.0/langchain/output_parsers/regex_dict.py
+-rw-r--r--   0        0        0     7786 2024-05-06 14:45:38.813684 gigachain-0.2.0/langchain/output_parsers/retry.py
+-rw-r--r--   0        0        0     3132 2024-05-06 14:45:38.814243 gigachain-0.2.0/langchain/output_parsers/structured.py
+-rw-r--r--   0        0        0       93 2024-01-10 09:04:40.496050 gigachain-0.2.0/langchain/output_parsers/xml.py
+-rw-r--r--   0        0        0     2181 2024-02-22 08:54:03.295025 gigachain-0.2.0/langchain/output_parsers/yaml.py
+-rw-r--r--   0        0        0     3152 2024-05-06 14:45:38.814849 gigachain-0.2.0/langchain/prompts/__init__.py
+-rw-r--r--   0        0        0      565 2023-12-18 12:05:47.511466 gigachain-0.2.0/langchain/prompts/base.py
+-rw-r--r--   0        0        0     1045 2023-12-18 12:05:47.512665 gigachain-0.2.0/langchain/prompts/chat.py
+-rw-r--r--   0        0        0     1152 2024-05-06 14:45:38.815501 gigachain-0.2.0/langchain/prompts/example_selector/__init__.py
+-rw-r--r--   0        0        0      105 2023-12-18 12:05:47.514537 gigachain-0.2.0/langchain/prompts/example_selector/base.py
+-rw-r--r--   0        0        0      136 2023-12-18 12:05:47.515578 gigachain-0.2.0/langchain/prompts/example_selector/length_based.py
+-rw-r--r--   0        0        0      877 2024-05-06 14:45:38.816038 gigachain-0.2.0/langchain/prompts/example_selector/ngram_overlap.py
+-rw-r--r--   0        0        0      288 2023-12-18 12:05:47.517451 gigachain-0.2.0/langchain/prompts/example_selector/semantic_similarity.py
+-rw-r--r--   0        0        0      265 2023-12-18 12:05:47.518312 gigachain-0.2.0/langchain/prompts/few_shot.py
+-rw-r--r--   0        0        0      128 2023-12-18 12:05:47.519153 gigachain-0.2.0/langchain/prompts/few_shot_with_templates.py
+-rw-r--r--   0        0        0      530 2023-12-18 12:05:47.519896 gigachain-0.2.0/langchain/prompts/loading.py
+-rw-r--r--   0        0        0      133 2023-12-18 12:05:47.520643 gigachain-0.2.0/langchain/prompts/pipeline.py
+-rw-r--r--   0        0        0      153 2023-12-18 12:05:47.521708 gigachain-0.2.0/langchain/prompts/prompt.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.868214 gigachain-0.2.0/langchain/py.typed
+-rw-r--r--   0        0        0      897 2023-08-21 13:51:28.868582 gigachain-0.2.0/langchain/pydantic_v1/__init__.py
+-rw-r--r--   0        0        0      134 2023-08-21 13:51:28.868846 gigachain-0.2.0/langchain/pydantic_v1/dataclasses.py
+-rw-r--r--   0        0        0      120 2023-08-21 13:51:28.869090 gigachain-0.2.0/langchain/pydantic_v1/main.py
+-rw-r--r--   0        0        0      462 2024-05-24 11:13:19.297989 gigachain-0.2.0/langchain/python.py
+-rw-r--r--   0        0        0      905 2024-05-06 14:45:38.816585 gigachain-0.2.0/langchain/requests.py
+-rw-r--r--   0        0        0     6660 2024-05-24 11:13:19.298938 gigachain-0.2.0/langchain/retrievers/__init__.py
+-rw-r--r--   0        0        0      629 2024-05-06 14:45:38.818705 gigachain-0.2.0/langchain/retrievers/arcee.py
+-rw-r--r--   0        0        0      629 2024-05-06 14:45:38.819278 gigachain-0.2.0/langchain/retrievers/arxiv.py
+-rw-r--r--   0        0        0      824 2024-05-06 14:45:38.819730 gigachain-0.2.0/langchain/retrievers/azure_ai_search.py
+-rw-r--r--   0        0        0      979 2024-05-06 14:45:38.820340 gigachain-0.2.0/langchain/retrievers/bedrock.py
+-rw-r--r--   0        0        0      819 2024-05-06 14:45:38.820874 gigachain-0.2.0/langchain/retrievers/bm25.py
+-rw-r--r--   0        0        0      641 2024-05-06 14:45:38.821443 gigachain-0.2.0/langchain/retrievers/chaindesk.py
+-rw-r--r--   0        0        0      653 2024-05-06 14:45:38.821966 gigachain-0.2.0/langchain/retrievers/chatgpt_plugin_retriever.py
+-rw-r--r--   0        0        0      641 2024-05-06 14:45:38.822506 gigachain-0.2.0/langchain/retrievers/cohere_rag_retriever.py
+-rw-r--r--   0        0        0     2290 2024-05-06 14:45:38.823062 gigachain-0.2.0/langchain/retrievers/contextual_compression.py
+-rw-r--r--   0        0        0      661 2024-05-06 14:45:38.823972 gigachain-0.2.0/langchain/retrievers/databerry.py
+-rw-r--r--   0        0        0      791 2024-05-06 14:45:38.824562 gigachain-0.2.0/langchain/retrievers/docarray.py
+-rw-r--r--   0        0        0     1141 2024-05-24 11:13:19.302286 gigachain-0.2.0/langchain/retrievers/document_compressors/__init__.py
+-rw-r--r--   0        0        0     2942 2024-04-19 07:38:34.050164 gigachain-0.2.0/langchain/retrievers/document_compressors/base.py
+-rw-r--r--   0        0        0     4216 2024-05-24 11:13:19.306222 gigachain-0.2.0/langchain/retrievers/document_compressors/chain_extract.py
+-rw-r--r--   0        0        0      621 2023-08-21 13:51:28.874260 gigachain-0.2.0/langchain/retrievers/document_compressors/chain_extract_prompt.py
+-rw-r--r--   0        0        0     2936 2024-05-24 11:13:19.308559 gigachain-0.2.0/langchain/retrievers/document_compressors/chain_filter.py
+-rw-r--r--   0        0        0      336 2023-09-04 15:41:37.267607 gigachain-0.2.0/langchain/retrievers/document_compressors/chain_filter_prompt.py
+-rw-r--r--   0        0        0     4542 2024-05-24 11:13:19.309413 gigachain-0.2.0/langchain/retrievers/document_compressors/cohere_rerank.py
+-rw-r--r--   0        0        0      393 2024-05-24 11:13:19.310522 gigachain-0.2.0/langchain/retrievers/document_compressors/cross_encoder.py
+-rw-r--r--   0        0        0     1597 2024-05-24 11:13:19.311898 gigachain-0.2.0/langchain/retrievers/document_compressors/cross_encoder_rerank.py
+-rw-r--r--   0        0        0     3614 2024-05-24 11:13:19.312642 gigachain-0.2.0/langchain/retrievers/document_compressors/embeddings_filter.py
+-rw-r--r--   0        0        0      709 2024-05-24 11:13:19.314036 gigachain-0.2.0/langchain/retrievers/document_compressors/flashrank_rerank.py
+-rw-r--r--   0        0        0      665 2024-05-06 14:45:38.825763 gigachain-0.2.0/langchain/retrievers/elastic_search_bm25.py
+-rw-r--r--   0        0        0      644 2024-05-06 14:45:38.826165 gigachain-0.2.0/langchain/retrievers/embedchain.py
+-rw-r--r--   0        0        0     9992 2024-05-06 14:45:38.827370 gigachain-0.2.0/langchain/retrievers/ensemble.py
+-rw-r--r--   0        0        0      695 2024-05-06 14:45:38.827921 gigachain-0.2.0/langchain/retrievers/google_cloud_documentai_warehouse.py
+-rw-r--r--   0        0        0     1040 2024-05-06 14:45:38.828488 gigachain-0.2.0/langchain/retrievers/google_vertex_ai_search.py
+-rw-r--r--   0        0        0      629 2024-05-06 14:45:38.828982 gigachain-0.2.0/langchain/retrievers/kay.py
+-rw-r--r--   0        0        0     2235 2024-05-06 14:45:38.829442 gigachain-0.2.0/langchain/retrievers/kendra.py
+-rw-r--r--   0        0        0      623 2024-05-06 14:45:38.829974 gigachain-0.2.0/langchain/retrievers/knn.py
+-rw-r--r--   0        0        0      800 2024-05-06 14:45:38.830505 gigachain-0.2.0/langchain/retrievers/llama_index.py
+-rw-r--r--   0        0        0     3601 2024-05-06 14:45:38.831384 gigachain-0.2.0/langchain/retrievers/merger_retriever.py
+-rw-r--r--   0        0        0      629 2024-05-06 14:45:38.831937 gigachain-0.2.0/langchain/retrievers/metal.py
+-rw-r--r--   0        0        0      796 2024-05-06 14:45:38.832467 gigachain-0.2.0/langchain/retrievers/milvus.py
+-rw-r--r--   0        0        0     7112 2024-05-06 14:45:38.833972 gigachain-0.2.0/langchain/retrievers/multi_query.py
+-rw-r--r--   0        0        0     3920 2024-02-22 08:54:03.309148 gigachain-0.2.0/langchain/retrievers/multi_vector.py
+-rw-r--r--   0        0        0      635 2024-05-06 14:45:38.834522 gigachain-0.2.0/langchain/retrievers/outline.py
+-rw-r--r--   0        0        0     5198 2024-04-19 07:38:34.057304 gigachain-0.2.0/langchain/retrievers/parent_document_retriever.py
+-rw-r--r--   0        0        0      674 2024-05-06 14:45:38.835067 gigachain-0.2.0/langchain/retrievers/pinecone_hybrid_search.py
+-rw-r--r--   0        0        0      632 2024-05-06 14:45:38.835556 gigachain-0.2.0/langchain/retrievers/pubmed.py
+-rw-r--r--   0        0        0      632 2024-05-06 14:45:38.835882 gigachain-0.2.0/langchain/retrievers/pupmed.py
+-rw-r--r--   0        0        0     2926 2024-05-06 14:45:38.836917 gigachain-0.2.0/langchain/retrievers/re_phraser.py
+-rw-r--r--   0        0        0      659 2024-05-06 14:45:38.837476 gigachain-0.2.0/langchain/retrievers/remote_retriever.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.882217 gigachain-0.2.0/langchain/retrievers/self_query/__init__.py
+-rw-r--r--   0        0        0      670 2024-05-24 11:13:19.315235 gigachain-0.2.0/langchain/retrievers/self_query/astradb.py
+-rw-r--r--   0        0        0    12383 2024-05-24 11:13:19.318584 gigachain-0.2.0/langchain/retrievers/self_query/base.py
+-rw-r--r--   0        0        0      665 2024-05-24 11:13:19.322337 gigachain-0.2.0/langchain/retrievers/self_query/chroma.py
+-rw-r--r--   0        0        0      685 2024-05-24 11:13:19.323029 gigachain-0.2.0/langchain/retrievers/self_query/dashvector.py
+-rw-r--r--   0        0        0      782 2024-05-24 11:13:19.323589 gigachain-0.2.0/langchain/retrievers/self_query/databricks_vector_search.py
+-rw-r--r--   0        0        0      816 2024-05-24 11:13:19.324262 gigachain-0.2.0/langchain/retrievers/self_query/deeplake.py
+-rw-r--r--   0        0        0      666 2024-05-24 11:13:19.324821 gigachain-0.2.0/langchain/retrievers/self_query/dingo.py
+-rw-r--r--   0        0        0      717 2024-05-24 11:13:19.325509 gigachain-0.2.0/langchain/retrievers/self_query/elasticsearch.py
+-rw-r--r--   0        0        0      792 2024-05-24 11:13:19.326077 gigachain-0.2.0/langchain/retrievers/self_query/milvus.py
+-rw-r--r--   0        0        0      714 2024-05-24 11:13:19.326662 gigachain-0.2.0/langchain/retrievers/self_query/mongodb_atlas.py
+-rw-r--r--   0        0        0      670 2024-05-24 11:13:19.328116 gigachain-0.2.0/langchain/retrievers/self_query/myscale.py
+-rw-r--r--   0        0        0      685 2024-05-24 11:13:19.329383 gigachain-0.2.0/langchain/retrievers/self_query/opensearch.py
+-rw-r--r--   0        0        0      675 2024-05-24 11:13:19.329988 gigachain-0.2.0/langchain/retrievers/self_query/pgvector.py
+-rw-r--r--   0        0        0      675 2024-05-24 11:13:19.330990 gigachain-0.2.0/langchain/retrievers/self_query/pinecone.py
+-rw-r--r--   0        0        0      665 2024-05-24 11:13:19.332596 gigachain-0.2.0/langchain/retrievers/self_query/qdrant.py
+-rw-r--r--   0        0        0      660 2024-05-24 11:13:19.335020 gigachain-0.2.0/langchain/retrievers/self_query/redis.py
+-rw-r--r--   0        0        0      693 2024-05-24 11:13:19.335916 gigachain-0.2.0/langchain/retrievers/self_query/supabase.py
+-rw-r--r--   0        0        0      743 2024-05-24 11:13:19.338559 gigachain-0.2.0/langchain/retrievers/self_query/tencentvectordb.py
+-rw-r--r--   0        0        0      743 2024-05-24 11:13:19.339250 gigachain-0.2.0/langchain/retrievers/self_query/timescalevector.py
+-rw-r--r--   0        0        0      798 2024-05-24 11:13:19.339874 gigachain-0.2.0/langchain/retrievers/self_query/vectara.py
+-rw-r--r--   0        0        0      675 2024-05-24 11:13:19.340498 gigachain-0.2.0/langchain/retrievers/self_query/weaviate.py
+-rw-r--r--   0        0        0      623 2024-05-06 14:45:38.855931 gigachain-0.2.0/langchain/retrievers/svm.py
+-rw-r--r--   0        0        0      833 2024-05-06 14:45:38.856457 gigachain-0.2.0/langchain/retrievers/tavily_search_api.py
+-rw-r--r--   0        0        0      629 2024-05-06 14:45:38.857002 gigachain-0.2.0/langchain/retrievers/tfidf.py
+-rw-r--r--   0        0        0     7649 2024-04-19 07:38:34.069556 gigachain-0.2.0/langchain/retrievers/time_weighted_retriever.py
+-rw-r--r--   0        0        0      629 2024-05-06 14:45:38.857850 gigachain-0.2.0/langchain/retrievers/vespa_retriever.py
+-rw-r--r--   0        0        0      674 2024-05-06 14:45:38.858459 gigachain-0.2.0/langchain/retrievers/weaviate_hybrid_search.py
+-rw-r--r--   0        0        0      939 2024-05-24 11:14:32.419149 gigachain-0.2.0/langchain/retrievers/web_research.py
+-rw-r--r--   0        0        0      641 2024-05-06 14:45:38.859170 gigachain-0.2.0/langchain/retrievers/wikipedia.py
+-rw-r--r--   0        0        0      623 2024-05-06 14:45:38.859741 gigachain-0.2.0/langchain/retrievers/you.py
+-rw-r--r--   0        0        0      855 2024-05-06 14:45:38.860229 gigachain-0.2.0/langchain/retrievers/zep.py
+-rw-r--r--   0        0        0      796 2024-05-06 14:45:38.860733 gigachain-0.2.0/langchain/retrievers/zilliz.py
+-rw-r--r--   0        0        0      693 2024-04-19 07:38:34.071437 gigachain-0.2.0/langchain/runnables/__init__.py
+-rw-r--r--   0        0        0      809 2023-12-18 12:05:47.571530 gigachain-0.2.0/langchain/runnables/hub.py
+-rw-r--r--   0        0        0     1525 2024-03-28 12:44:20.559025 gigachain-0.2.0/langchain/runnables/openai_functions.py
+-rw-r--r--   0        0        0     2066 2024-04-19 07:38:34.072360 gigachain-0.2.0/langchain/schema/__init__.py
+-rw-r--r--   0        0        0      149 2023-12-18 12:05:47.576297 gigachain-0.2.0/langchain/schema/agent.py
+-rw-r--r--   0        0        0      105 2023-12-18 12:05:47.576979 gigachain-0.2.0/langchain/schema/cache.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:47.577169 gigachain-0.2.0/langchain/schema/callbacks/__init__.py
+-rw-r--r--   0        0        0      511 2023-12-18 12:05:47.577786 gigachain-0.2.0/langchain/schema/callbacks/base.py
+-rw-r--r--   0        0        0     1511 2023-12-18 12:05:47.578611 gigachain-0.2.0/langchain/schema/callbacks/manager.py
+-rw-r--r--   0        0        0      103 2023-12-18 12:05:47.579043 gigachain-0.2.0/langchain/schema/callbacks/stdout.py
+-rw-r--r--   0        0        0      131 2023-12-18 12:05:47.579408 gigachain-0.2.0/langchain/schema/callbacks/streaming_stdout.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:47.579637 gigachain-0.2.0/langchain/schema/callbacks/tracers/__init__.py
+-rw-r--r--   0        0        0      113 2023-12-18 12:05:47.580043 gigachain-0.2.0/langchain/schema/callbacks/tracers/base.py
+-rw-r--r--   0        0        0      176 2023-12-18 12:05:47.580505 gigachain-0.2.0/langchain/schema/callbacks/tracers/evaluation.py
+-rw-r--r--   0        0        0      219 2023-12-18 12:05:47.580868 gigachain-0.2.0/langchain/schema/callbacks/tracers/langchain.py
+-rw-r--r--   0        0        0      127 2023-12-18 12:05:47.581282 gigachain-0.2.0/langchain/schema/callbacks/tracers/langchain_v1.py
+-rw-r--r--   0        0        0      226 2023-12-18 12:05:47.581685 gigachain-0.2.0/langchain/schema/callbacks/tracers/log_stream.py
+-rw-r--r--   0        0        0      105 2023-12-18 12:05:47.582039 gigachain-0.2.0/langchain/schema/callbacks/tracers/root_listeners.py
+-rw-r--r--   0        0        0      120 2023-12-18 12:05:47.582518 gigachain-0.2.0/langchain/schema/callbacks/tracers/run_collector.py
+-rw-r--r--   0        0        0      470 2023-12-18 12:05:47.582779 gigachain-0.2.0/langchain/schema/callbacks/tracers/schemas.py
+-rw-r--r--   0        0        0      257 2023-12-18 12:05:47.583106 gigachain-0.2.0/langchain/schema/callbacks/tracers/stdout.py
+-rw-r--r--   0        0        0       80 2023-12-18 12:05:47.583799 gigachain-0.2.0/langchain/schema/chat.py
+-rw-r--r--   0        0        0      101 2023-12-18 12:05:47.584843 gigachain-0.2.0/langchain/schema/chat_history.py
+-rw-r--r--   0        0        0      122 2023-12-18 12:05:47.585605 gigachain-0.2.0/langchain/schema/document.py
+-rw-r--r--   0        0        0       75 2023-12-18 12:05:47.586431 gigachain-0.2.0/langchain/schema/embeddings.py
+-rw-r--r--   0        0        0       91 2023-12-18 12:05:47.587468 gigachain-0.2.0/langchain/schema/exceptions.py
+-rw-r--r--   0        0        0      367 2023-12-18 12:05:47.588176 gigachain-0.2.0/langchain/schema/language_model.py
+-rw-r--r--   0        0        0       71 2023-12-18 12:05:47.588957 gigachain-0.2.0/langchain/schema/memory.py
+-rw-r--r--   0        0        0     1048 2023-12-18 12:05:47.589743 gigachain-0.2.0/langchain/schema/messages.py
+-rw-r--r--   0        0        0      320 2023-12-18 12:05:47.590462 gigachain-0.2.0/langchain/schema/output.py
+-rw-r--r--   0        0        0      651 2023-12-18 12:05:47.591291 gigachain-0.2.0/langchain/schema/output_parser.py
+-rw-r--r--   0        0        0       80 2023-12-18 12:05:47.592095 gigachain-0.2.0/langchain/schema/prompt.py
+-rw-r--r--   0        0        0      124 2023-12-18 12:05:47.592918 gigachain-0.2.0/langchain/schema/prompt_template.py
+-rw-r--r--   0        0        0       81 2023-12-18 12:05:47.593622 gigachain-0.2.0/langchain/schema/retriever.py
+-rw-r--r--   0        0        0     1797 2024-04-19 07:38:34.073306 gigachain-0.2.0/langchain/schema/runnable/__init__.py
+-rw-r--r--   0        0        0      781 2023-12-18 12:05:47.595763 gigachain-0.2.0/langchain/schema/runnable/base.py
+-rw-r--r--   0        0        0       89 2023-12-18 12:05:47.596655 gigachain-0.2.0/langchain/schema/runnable/branch.py
+-rw-r--r--   0        0        0      665 2023-12-18 12:05:47.597563 gigachain-0.2.0/langchain/schema/runnable/config.py
+-rw-r--r--   0        0        0      333 2023-12-18 12:05:47.598462 gigachain-0.2.0/langchain/schema/runnable/configurable.py
+-rw-r--r--   0        0        0      106 2023-12-18 12:05:47.599358 gigachain-0.2.0/langchain/schema/runnable/fallbacks.py
+-rw-r--r--   0        0        0      260 2023-12-18 12:05:47.600021 gigachain-0.2.0/langchain/schema/runnable/history.py
+-rw-r--r--   0        0        0      205 2023-12-18 12:05:47.600672 gigachain-0.2.0/langchain/schema/runnable/passthrough.py
+-rw-r--r--   0        0        0       94 2023-12-18 12:05:47.601412 gigachain-0.2.0/langchain/schema/runnable/retry.py
+-rw-r--r--   0        0        0      117 2023-12-18 12:05:47.602442 gigachain-0.2.0/langchain/schema/runnable/router.py
+-rw-r--r--   0        0        0     1118 2023-12-18 12:05:47.603240 gigachain-0.2.0/langchain/schema/runnable/utils.py
+-rw-r--r--   0        0        0       85 2023-12-18 12:05:47.604392 gigachain-0.2.0/langchain/schema/storage.py
+-rw-r--r--   0        0        0      137 2023-12-18 12:05:47.605680 gigachain-0.2.0/langchain/schema/vectorstore.py
+-rw-r--r--   0        0        0      662 2024-05-06 14:45:38.861288 gigachain-0.2.0/langchain/serpapi.py
+-rw-r--r--   0        0        0     3509 2024-04-19 07:38:34.080201 gigachain-0.2.0/langchain/smith/__init__.py
+-rw-r--r--   0        0        0     2198 2024-04-19 07:38:34.083198 gigachain-0.2.0/langchain/smith/evaluation/__init__.py
+-rw-r--r--   0        0        0    13429 2024-04-19 07:38:34.084610 gigachain-0.2.0/langchain/smith/evaluation/config.py
+-rw-r--r--   0        0        0     9936 2023-12-18 12:05:47.609341 gigachain-0.2.0/langchain/smith/evaluation/name_generation.py
+-rw-r--r--   0        0        0     3310 2024-03-28 12:44:20.560885 gigachain-0.2.0/langchain/smith/evaluation/progress.py
+-rw-r--r--   0        0        0    54230 2024-05-06 14:45:38.868256 gigachain-0.2.0/langchain/smith/evaluation/runner_utils.py
+-rw-r--r--   0        0        0    17113 2024-04-19 07:38:34.087528 gigachain-0.2.0/langchain/smith/evaluation/string_run_evaluator.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.895985 gigachain-0.2.0/langchain/smith/evaluation/utils.py
+-rw-r--r--   0        0        0      663 2024-05-06 14:45:38.869236 gigachain-0.2.0/langchain/sql_database.py
+-rw-r--r--   0        0        0     1584 2024-05-06 14:45:38.869889 gigachain-0.2.0/langchain/storage/__init__.py
+-rw-r--r--   0        0        0     2518 2024-04-19 07:38:34.092225 gigachain-0.2.0/langchain/storage/_lc_store.py
+-rw-r--r--   0        0        0     4333 2024-04-19 07:38:34.093006 gigachain-0.2.0/langchain/storage/encoder_backed.py
+-rw-r--r--   0        0        0       89 2024-05-06 14:45:38.870401 gigachain-0.2.0/langchain/storage/exceptions.py
+-rw-r--r--   0        0        0     6107 2024-05-24 11:13:19.346753 gigachain-0.2.0/langchain/storage/file_system.py
+-rw-r--r--   0        0        0      368 2024-05-06 14:45:38.870971 gigachain-0.2.0/langchain/storage/in_memory.py
+-rw-r--r--   0        0        0      611 2024-05-06 14:45:38.871533 gigachain-0.2.0/langchain/storage/redis.py
+-rw-r--r--   0        0        0      751 2024-05-06 14:45:38.872083 gigachain-0.2.0/langchain/storage/upstash_redis.py
+-rw-r--r--   0        0        0     1554 2024-04-19 07:38:34.099272 gigachain-0.2.0/langchain/text_splitter.py
+-rw-r--r--   0        0        0     5663 2024-05-06 14:45:38.873979 gigachain-0.2.0/langchain/tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 11:13:19.348191 gigachain-0.2.0/langchain/tools/ainetwork/__init__.py
+-rw-r--r--   0        0        0      863 2024-05-24 11:13:19.348921 gigachain-0.2.0/langchain/tools/ainetwork/app.py
+-rw-r--r--   0        0        0      748 2024-05-24 11:13:19.349480 gigachain-0.2.0/langchain/tools/ainetwork/base.py
+-rw-r--r--   0        0        0      767 2024-05-24 11:13:19.350014 gigachain-0.2.0/langchain/tools/ainetwork/owner.py
+-rw-r--r--   0        0        0      762 2024-05-24 11:13:19.350586 gigachain-0.2.0/langchain/tools/ainetwork/rule.py
+-rw-r--r--   0        0        0      785 2024-05-24 11:13:19.351167 gigachain-0.2.0/langchain/tools/ainetwork/transfer.py
+-rw-r--r--   0        0        0      770 2024-05-24 11:13:19.352616 gigachain-0.2.0/langchain/tools/ainetwork/value.py
+-rw-r--r--   0        0        0      905 2024-05-06 14:45:38.874673 gigachain-0.2.0/langchain/tools/amadeus/__init__.py
+-rw-r--r--   0        0        0      648 2024-05-06 14:45:38.875343 gigachain-0.2.0/langchain/tools/amadeus/base.py
+-rw-r--r--   0        0        0      851 2024-05-06 14:45:38.875995 gigachain-0.2.0/langchain/tools/amadeus/closest_airport.py
+-rw-r--r--   0        0        0      833 2024-05-06 14:45:38.876640 gigachain-0.2.0/langchain/tools/amadeus/flight_search.py
+-rw-r--r--   0        0        0       25 2023-08-21 13:51:28.901095 gigachain-0.2.0/langchain/tools/arxiv/__init__.py
+-rw-r--r--   0        0        0      763 2024-05-06 14:45:38.877657 gigachain-0.2.0/langchain/tools/arxiv/tool.py
+-rw-r--r--   0        0        0     1258 2024-05-06 14:45:38.878288 gigachain-0.2.0/langchain/tools/azure_cognitive_services/__init__.py
+-rw-r--r--   0        0        0      658 2024-05-06 14:45:38.878826 gigachain-0.2.0/langchain/tools/azure_cognitive_services/form_recognizer.py
+-rw-r--r--   0        0        0      655 2024-05-06 14:45:38.879338 gigachain-0.2.0/langchain/tools/azure_cognitive_services/image_analysis.py
+-rw-r--r--   0        0        0      649 2024-05-06 14:45:38.879841 gigachain-0.2.0/langchain/tools/azure_cognitive_services/speech2text.py
+-rw-r--r--   0        0        0      649 2024-05-06 14:45:38.880282 gigachain-0.2.0/langchain/tools/azure_cognitive_services/text2speech.py
+-rw-r--r--   0        0        0      673 2024-05-06 14:45:38.880829 gigachain-0.2.0/langchain/tools/azure_cognitive_services/text_analytics_health.py
+-rw-r--r--   0        0        0      332 2024-01-10 09:04:40.515503 gigachain-0.2.0/langchain/tools/base.py
+-rw-r--r--   0        0        0        0 2023-10-19 12:57:53.049903 gigachain-0.2.0/langchain/tools/bearly/__init__.py
+-rw-r--r--   0        0        0      957 2024-05-06 14:45:38.881421 gigachain-0.2.0/langchain/tools/bearly/tool.py
+-rw-r--r--   0        0        0      752 2024-05-06 14:45:38.882113 gigachain-0.2.0/langchain/tools/bing_search/__init__.py
+-rw-r--r--   0        0        0      721 2024-05-06 14:45:38.882539 gigachain-0.2.0/langchain/tools/bing_search/tool.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.906784 gigachain-0.2.0/langchain/tools/brave_search/__init__.py
+-rw-r--r--   0        0        0      610 2024-05-06 14:45:38.882881 gigachain-0.2.0/langchain/tools/brave_search/tool.py
+-rw-r--r--   0        0        0        0 2023-10-06 14:43:01.562867 gigachain-0.2.0/langchain/tools/clickup/__init__.py
+-rw-r--r--   0        0        0      642 2024-05-06 14:45:38.883283 gigachain-0.2.0/langchain/tools/clickup/tool.py
+-rw-r--r--   0        0        0      157 2024-02-22 08:54:03.337885 gigachain-0.2.0/langchain/tools/convert_to_openai.py
+-rw-r--r--   0        0        0      927 2024-05-06 14:45:38.883886 gigachain-0.2.0/langchain/tools/dataforseo_api_search/__init__.py
+-rw-r--r--   0        0        0      897 2024-05-06 14:45:38.884293 gigachain-0.2.0/langchain/tools/dataforseo_api_search/tool.py
+-rw-r--r--   0        0        0      671 2024-05-06 14:45:38.884882 gigachain-0.2.0/langchain/tools/ddg_search/__init__.py
+-rw-r--r--   0        0        0     1024 2024-05-06 14:45:38.885279 gigachain-0.2.0/langchain/tools/ddg_search/tool.py
+-rw-r--r--   0        0        0        0 2023-10-30 16:05:53.968119 gigachain-0.2.0/langchain/tools/e2b_data_analysis/__init__.py
+-rw-r--r--   0        0        0      990 2024-05-06 14:45:38.885683 gigachain-0.2.0/langchain/tools/e2b_data_analysis/tool.py
+-rw-r--r--   0        0        0     1513 2024-05-06 14:45:38.886016 gigachain-0.2.0/langchain/tools/edenai/__init__.py
+-rw-r--r--   0        0        0      643 2024-05-06 14:45:38.886330 gigachain-0.2.0/langchain/tools/edenai/audio_speech_to_text.py
+-rw-r--r--   0        0        0      643 2024-05-06 14:45:38.886803 gigachain-0.2.0/langchain/tools/edenai/audio_text_to_speech.py
+-rw-r--r--   0        0        0      607 2024-05-06 14:45:38.887166 gigachain-0.2.0/langchain/tools/edenai/edenai_base_tool.py
+-rw-r--r--   0        0        0      646 2024-05-06 14:45:38.887588 gigachain-0.2.0/langchain/tools/edenai/image_explicitcontent.py
+-rw-r--r--   0        0        0      652 2024-05-06 14:45:38.888132 gigachain-0.2.0/langchain/tools/edenai/image_objectdetection.py
+-rw-r--r--   0        0        0      634 2024-05-06 14:45:38.888711 gigachain-0.2.0/langchain/tools/edenai/ocr_identityparser.py
+-rw-r--r--   0        0        0      649 2024-05-06 14:45:38.889293 gigachain-0.2.0/langchain/tools/edenai/ocr_invoiceparser.py
+-rw-r--r--   0        0        0      649 2024-05-06 14:45:38.889930 gigachain-0.2.0/langchain/tools/edenai/text_moderation.py
+-rw-r--r--   0        0        0      686 2024-05-06 14:45:38.890599 gigachain-0.2.0/langchain/tools/eleven_labs/__init__.py
+-rw-r--r--   0        0        0      660 2024-05-06 14:45:38.891159 gigachain-0.2.0/langchain/tools/eleven_labs/models.py
+-rw-r--r--   0        0        0      652 2024-05-06 14:45:38.891674 gigachain-0.2.0/langchain/tools/eleven_labs/text2speech.py
+-rw-r--r--   0        0        0     1242 2024-05-06 14:45:38.892300 gigachain-0.2.0/langchain/tools/file_management/__init__.py
+-rw-r--r--   0        0        0      789 2024-05-06 14:45:38.892821 gigachain-0.2.0/langchain/tools/file_management/copy.py
+-rw-r--r--   0        0        0      805 2024-05-06 14:45:38.893396 gigachain-0.2.0/langchain/tools/file_management/delete.py
+-rw-r--r--   0        0        0      815 2024-05-06 14:45:38.893971 gigachain-0.2.0/langchain/tools/file_management/file_search.py
+-rw-r--r--   0        0        0      836 2024-05-06 14:45:38.894533 gigachain-0.2.0/langchain/tools/file_management/list_dir.py
+-rw-r--r--   0        0        0      789 2024-05-06 14:45:38.895027 gigachain-0.2.0/langchain/tools/file_management/move.py
+-rw-r--r--   0        0        0      789 2024-05-06 14:45:38.895534 gigachain-0.2.0/langchain/tools/file_management/read.py
+-rw-r--r--   0        0        0      797 2024-05-06 14:45:38.896019 gigachain-0.2.0/langchain/tools/file_management/write.py
+-rw-r--r--   0        0        0       18 2024-04-19 07:38:34.103325 gigachain-0.2.0/langchain/tools/github/__init__.py
+-rw-r--r--   0        0        0      637 2024-05-06 14:45:38.896555 gigachain-0.2.0/langchain/tools/github/tool.py
+-rw-r--r--   0        0        0       18 2024-04-19 07:38:34.104361 gigachain-0.2.0/langchain/tools/gitlab/__init__.py
+-rw-r--r--   0        0        0      637 2024-05-06 14:45:38.897086 gigachain-0.2.0/langchain/tools/gitlab/tool.py
+-rw-r--r--   0        0        0     1056 2024-05-06 14:45:38.897959 gigachain-0.2.0/langchain/tools/gmail/__init__.py
+-rw-r--r--   0        0        0      638 2024-05-06 14:45:38.898474 gigachain-0.2.0/langchain/tools/gmail/base.py
+-rw-r--r--   0        0        0      809 2024-05-06 14:45:38.898997 gigachain-0.2.0/langchain/tools/gmail/create_draft.py
+-rw-r--r--   0        0        0      801 2024-05-06 14:45:38.899539 gigachain-0.2.0/langchain/tools/gmail/get_message.py
+-rw-r--r--   0        0        0      793 2024-05-06 14:45:38.900104 gigachain-0.2.0/langchain/tools/gmail/get_thread.py
+-rw-r--r--   0        0        0      863 2024-05-06 14:45:38.900693 gigachain-0.2.0/langchain/tools/gmail/search.py
+-rw-r--r--   0        0        0      809 2024-05-06 14:45:38.901269 gigachain-0.2.0/langchain/tools/gmail/send_message.py
+-rw-r--r--   0        0        0      681 2024-05-06 14:45:38.901868 gigachain-0.2.0/langchain/tools/golden_query/__init__.py
+-rw-r--r--   0        0        0      655 2024-05-06 14:45:38.902420 gigachain-0.2.0/langchain/tools/golden_query/tool.py
+-rw-r--r--   0        0        0      684 2024-05-06 14:45:38.902967 gigachain-0.2.0/langchain/tools/google_cloud/__init__.py
+-rw-r--r--   0        0        0      658 2024-05-06 14:45:38.903438 gigachain-0.2.0/langchain/tools/google_cloud/texttospeech.py
+-rw-r--r--   0        0        0      720 2024-05-06 14:45:38.904147 gigachain-0.2.0/langchain/tools/google_finance/__init__.py
+-rw-r--r--   0        0        0      686 2024-05-06 14:45:38.904526 gigachain-0.2.0/langchain/tools/google_finance/tool.py
+-rw-r--r--   0        0        0      696 2024-05-06 14:45:38.906054 gigachain-0.2.0/langchain/tools/google_jobs/__init__.py
+-rw-r--r--   0        0        0      665 2024-05-06 14:45:38.906623 gigachain-0.2.0/langchain/tools/google_jobs/tool.py
+-rw-r--r--   0        0        0      696 2024-05-06 14:45:38.907195 gigachain-0.2.0/langchain/tools/google_lens/__init__.py
+-rw-r--r--   0        0        0      665 2024-05-06 14:45:38.907799 gigachain-0.2.0/langchain/tools/google_lens/tool.py
+-rw-r--r--   0        0        0      658 2024-05-06 14:45:38.908368 gigachain-0.2.0/langchain/tools/google_places/__init__.py
+-rw-r--r--   0        0        0      812 2024-05-06 14:45:38.908913 gigachain-0.2.0/langchain/tools/google_places/tool.py
+-rw-r--r--   0        0        0      720 2024-05-06 14:45:38.909567 gigachain-0.2.0/langchain/tools/google_scholar/__init__.py
+-rw-r--r--   0        0        0      686 2024-05-06 14:45:38.910117 gigachain-0.2.0/langchain/tools/google_scholar/tool.py
+-rw-r--r--   0        0        0      766 2024-05-06 14:45:38.910742 gigachain-0.2.0/langchain/tools/google_search/__init__.py
+-rw-r--r--   0        0        0      733 2024-05-06 14:45:38.911311 gigachain-0.2.0/langchain/tools/google_search/tool.py
+-rw-r--r--   0        0        0      815 2024-05-06 14:45:38.911870 gigachain-0.2.0/langchain/tools/google_serper/__init__.py
+-rw-r--r--   0        0        0      733 2024-05-06 14:45:38.912375 gigachain-0.2.0/langchain/tools/google_serper/tool.py
+-rw-r--r--   0        0        0      714 2024-05-06 14:45:38.912923 gigachain-0.2.0/langchain/tools/google_trends/__init__.py
+-rw-r--r--   0        0        0      681 2024-05-06 14:45:38.913444 gigachain-0.2.0/langchain/tools/google_trends/tool.py
+-rw-r--r--   0        0        0       47 2023-08-21 13:51:28.921484 gigachain-0.2.0/langchain/tools/graphql/__init__.py
+-rw-r--r--   0        0        0      622 2024-05-06 14:45:38.913963 gigachain-0.2.0/langchain/tools/graphql/tool.py
+-rw-r--r--   0        0        0      655 2024-05-06 14:45:38.914502 gigachain-0.2.0/langchain/tools/human/__init__.py
+-rw-r--r--   0        0        0      616 2024-05-06 14:45:38.914993 gigachain-0.2.0/langchain/tools/human/tool.py
+-rw-r--r--   0        0        0      613 2024-05-06 14:45:38.915530 gigachain-0.2.0/langchain/tools/ifttt.py
+-rw-r--r--   0        0        0       43 2023-08-21 13:51:28.923495 gigachain-0.2.0/langchain/tools/interaction/__init__.py
+-rw-r--r--   0        0        0      625 2024-05-06 14:45:38.916471 gigachain-0.2.0/langchain/tools/interaction/tool.py
+-rw-r--r--   0        0        0       17 2023-08-21 13:51:28.924161 gigachain-0.2.0/langchain/tools/jira/__init__.py
+-rw-r--r--   0        0        0      607 2024-05-06 14:45:38.917068 gigachain-0.2.0/langchain/tools/jira/tool.py
+-rw-r--r--   0        0        0       46 2023-08-21 13:51:28.925352 gigachain-0.2.0/langchain/tools/json/__init__.py
+-rw-r--r--   0        0        0      859 2024-05-06 14:45:38.917619 gigachain-0.2.0/langchain/tools/json/tool.py
+-rw-r--r--   0        0        0      677 2024-05-06 14:45:38.918132 gigachain-0.2.0/langchain/tools/memorize/__init__.py
+-rw-r--r--   0        0        0      733 2024-05-06 14:45:38.918644 gigachain-0.2.0/langchain/tools/memorize/tool.py
+-rw-r--r--   0        0        0       35 2023-12-18 12:05:47.720059 gigachain-0.2.0/langchain/tools/merriam_webster/__init__.py
+-rw-r--r--   0        0        0      643 2024-05-06 14:45:38.919299 gigachain-0.2.0/langchain/tools/merriam_webster/tool.py
+-rw-r--r--   0        0        0      675 2024-05-06 14:45:38.919805 gigachain-0.2.0/langchain/tools/metaphor_search/__init__.py
+-rw-r--r--   0        0        0      640 2024-05-06 14:45:38.920230 gigachain-0.2.0/langchain/tools/metaphor_search/tool.py
+-rw-r--r--   0        0        0     1105 2024-05-06 14:45:38.920723 gigachain-0.2.0/langchain/tools/multion/__init__.py
+-rw-r--r--   0        0        0      833 2024-05-06 14:45:38.921205 gigachain-0.2.0/langchain/tools/multion/close_session.py
+-rw-r--r--   0        0        0      842 2024-05-06 14:45:38.921640 gigachain-0.2.0/langchain/tools/multion/create_session.py
+-rw-r--r--   0        0        0      842 2024-05-06 14:45:38.922036 gigachain-0.2.0/langchain/tools/multion/update_session.py
+-rw-r--r--   0        0        0        0 2023-12-18 12:05:47.724833 gigachain-0.2.0/langchain/tools/nasa/__init__.py
+-rw-r--r--   0        0        0      607 2024-05-06 14:45:38.922517 gigachain-0.2.0/langchain/tools/nasa/tool.py
+-rw-r--r--   0        0        0      667 2024-05-06 14:45:38.922922 gigachain-0.2.0/langchain/tools/nuclia/__init__.py
+-rw-r--r--   0        0        0      760 2024-05-06 14:45:38.923457 gigachain-0.2.0/langchain/tools/nuclia/tool.py
+-rw-r--r--   0        0        0     1085 2024-05-06 14:45:38.924081 gigachain-0.2.0/langchain/tools/office365/__init__.py
+-rw-r--r--   0        0        0      643 2024-05-06 14:45:38.924476 gigachain-0.2.0/langchain/tools/office365/base.py
+-rw-r--r--   0        0        0      905 2024-05-06 14:45:38.924822 gigachain-0.2.0/langchain/tools/office365/create_draft_message.py
+-rw-r--r--   0        0        0      819 2024-05-06 14:45:38.925176 gigachain-0.2.0/langchain/tools/office365/events_search.py
+-rw-r--r--   0        0        0      823 2024-05-06 14:45:38.925512 gigachain-0.2.0/langchain/tools/office365/messages_search.py
+-rw-r--r--   0        0        0      798 2024-05-06 14:45:38.925850 gigachain-0.2.0/langchain/tools/office365/send_event.py
+-rw-r--r--   0        0        0      814 2024-05-06 14:45:38.926423 gigachain-0.2.0/langchain/tools/office365/send_message.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.933159 gigachain-0.2.0/langchain/tools/openapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.933535 gigachain-0.2.0/langchain/tools/openapi/utils/__init__.py
+-rw-r--r--   0        0        0     1859 2024-05-06 14:45:38.926900 gigachain-0.2.0/langchain/tools/openapi/utils/api_models.py
+-rw-r--r--   0        0        0      833 2024-05-06 14:45:38.927339 gigachain-0.2.0/langchain/tools/openapi/utils/openapi_utils.py
+-rw-r--r--   0        0        0      677 2024-05-06 14:45:38.927784 gigachain-0.2.0/langchain/tools/openweathermap/__init__.py
+-rw-r--r--   0        0        0      643 2024-05-06 14:45:38.928213 gigachain-0.2.0/langchain/tools/openweathermap/tool.py
+-rw-r--r--   0        0        0     1282 2024-05-06 14:45:38.928641 gigachain-0.2.0/langchain/tools/playwright/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-06 14:45:38.929069 gigachain-0.2.0/langchain/tools/playwright/base.py
+-rw-r--r--   0        0        0      775 2024-05-06 14:45:38.929423 gigachain-0.2.0/langchain/tools/playwright/click.py
+-rw-r--r--   0        0        0      631 2024-05-06 14:45:38.929748 gigachain-0.2.0/langchain/tools/playwright/current_page.py
+-rw-r--r--   0        0        0      906 2024-05-06 14:45:38.930075 gigachain-0.2.0/langchain/tools/playwright/extract_hyperlinks.py
+-rw-r--r--   0        0        0      622 2024-05-06 14:45:38.930387 gigachain-0.2.0/langchain/tools/playwright/extract_text.py
+-rw-r--r--   0        0        0      825 2024-05-06 14:45:38.930786 gigachain-0.2.0/langchain/tools/playwright/get_elements.py
+-rw-r--r--   0        0        0      799 2024-05-06 14:45:38.931147 gigachain-0.2.0/langchain/tools/playwright/navigate.py
+-rw-r--r--   0        0        0      625 2024-05-06 14:45:38.931483 gigachain-0.2.0/langchain/tools/playwright/navigate_back.py
+-rw-r--r--   0        0        0      935 2024-05-06 14:45:38.931988 gigachain-0.2.0/langchain/tools/plugin.py
+-rw-r--r--   0        0        0       52 2023-08-21 13:51:28.940033 gigachain-0.2.0/langchain/tools/powerbi/__init__.py
+-rw-r--r--   0        0        0      849 2024-05-06 14:45:38.932547 gigachain-0.2.0/langchain/tools/powerbi/tool.py
+-rw-r--r--   0        0        0       26 2023-08-21 13:51:28.941121 gigachain-0.2.0/langchain/tools/pubmed/__init__.py
+-rw-r--r--   0        0        0      619 2024-05-06 14:45:38.933060 gigachain-0.2.0/langchain/tools/pubmed/tool.py
+-rw-r--r--   0        0        0      515 2024-05-06 14:45:38.933654 gigachain-0.2.0/langchain/tools/python/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-10 09:04:40.541802 gigachain-0.2.0/langchain/tools/reddit_search/__init__.py
+-rw-r--r--   0        0        0      730 2024-05-06 14:45:38.934192 gigachain-0.2.0/langchain/tools/reddit_search/tool.py
+-rw-r--r--   0        0        0      705 2024-05-06 14:45:38.935108 gigachain-0.2.0/langchain/tools/render.py
+-rw-r--r--   0        0        0       52 2023-08-21 13:51:28.942395 gigachain-0.2.0/langchain/tools/requests/__init__.py
+-rw-r--r--   0        0        0     1167 2024-05-06 14:45:38.935929 gigachain-0.2.0/langchain/tools/requests/tool.py
+-rw-r--r--   0        0        0      328 2024-05-06 14:45:38.936370 gigachain-0.2.0/langchain/tools/retriever.py
+-rw-r--r--   0        0        0       31 2023-08-21 13:51:28.943010 gigachain-0.2.0/langchain/tools/scenexplain/__init__.py
+-rw-r--r--   0        0        0      799 2024-05-06 14:45:38.936830 gigachain-0.2.0/langchain/tools/scenexplain/tool.py
+-rw-r--r--   0        0        0      797 2024-05-06 14:45:38.937290 gigachain-0.2.0/langchain/tools/searchapi/__init__.py
+-rw-r--r--   0        0        0      715 2024-05-06 14:45:38.937639 gigachain-0.2.0/langchain/tools/searchapi/tool.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.943553 gigachain-0.2.0/langchain/tools/searx_search/__init__.py
+-rw-r--r--   0        0        0      727 2024-05-06 14:45:38.938151 gigachain-0.2.0/langchain/tools/searx_search/tool.py
+-rw-r--r--   0        0        0      622 2024-05-06 14:45:38.938693 gigachain-0.2.0/langchain/tools/shell/__init__.py
+-rw-r--r--   0        0        0      751 2024-05-06 14:45:38.939234 gigachain-0.2.0/langchain/tools/shell/tool.py
+-rw-r--r--   0        0        0      983 2024-05-06 14:45:38.939734 gigachain-0.2.0/langchain/tools/slack/__init__.py
+-rw-r--r--   0        0        0      638 2024-05-06 14:45:38.940319 gigachain-0.2.0/langchain/tools/slack/base.py
+-rw-r--r--   0        0        0      622 2024-05-06 14:45:38.940846 gigachain-0.2.0/langchain/tools/slack/get_channel.py
+-rw-r--r--   0        0        0      816 2024-05-06 14:45:38.941286 gigachain-0.2.0/langchain/tools/slack/get_message.py
+-rw-r--r--   0        0        0      841 2024-05-06 14:45:38.941751 gigachain-0.2.0/langchain/tools/slack/schedule_message.py
+-rw-r--r--   0        0        0      809 2024-05-06 14:45:38.942287 gigachain-0.2.0/langchain/tools/slack/send_message.py
+-rw-r--r--   0        0        0       18 2023-08-21 13:51:28.944873 gigachain-0.2.0/langchain/tools/sleep/__init__.py
+-rw-r--r--   0        0        0      751 2024-05-06 14:45:38.942828 gigachain-0.2.0/langchain/tools/sleep/tool.py
+-rw-r--r--   0        0        0       44 2023-08-21 13:51:28.945531 gigachain-0.2.0/langchain/tools/spark_sql/__init__.py
+-rw-r--r--   0        0        0     1064 2024-05-06 14:45:38.943336 gigachain-0.2.0/langchain/tools/spark_sql/tool.py
+-rw-r--r--   0        0        0       49 2023-08-21 13:51:28.946602 gigachain-0.2.0/langchain/tools/sql_database/__init__.py
+-rw-r--r--   0        0        0      504 2024-05-24 11:13:19.353405 gigachain-0.2.0/langchain/tools/sql_database/prompt.py
+-rw-r--r--   0        0        0     1109 2024-05-06 14:45:38.943869 gigachain-0.2.0/langchain/tools/sql_database/tool.py
+-rw-r--r--   0        0        0       33 2023-12-18 12:05:47.764989 gigachain-0.2.0/langchain/tools/stackexchange/__init__.py
+-rw-r--r--   0        0        0      628 2024-05-06 14:45:38.944387 gigachain-0.2.0/langchain/tools/stackexchange/tool.py
+-rw-r--r--   0        0        0       24 2023-12-18 12:05:47.765850 gigachain-0.2.0/langchain/tools/steam/__init__.py
+-rw-r--r--   0        0        0      634 2024-05-06 14:45:38.945081 gigachain-0.2.0/langchain/tools/steam/tool.py
+-rw-r--r--   0        0        0      694 2024-05-06 14:45:38.945662 gigachain-0.2.0/langchain/tools/steamship_image_generation/__init__.py
+-rw-r--r--   0        0        0      847 2024-05-06 14:45:38.946128 gigachain-0.2.0/langchain/tools/steamship_image_generation/tool.py
+-rw-r--r--   0        0        0      839 2024-05-06 14:45:38.946736 gigachain-0.2.0/langchain/tools/tavily_search/__init__.py
+-rw-r--r--   0        0        0      913 2024-05-06 14:45:38.947265 gigachain-0.2.0/langchain/tools/tavily_search/tool.py
+-rw-r--r--   0        0        0       51 2023-08-21 13:51:28.948611 gigachain-0.2.0/langchain/tools/vectorstore/__init__.py
+-rw-r--r--   0        0        0      791 2024-05-06 14:45:38.948199 gigachain-0.2.0/langchain/tools/vectorstore/tool.py
+-rw-r--r--   0        0        0       29 2023-08-21 13:51:28.949334 gigachain-0.2.0/langchain/tools/wikipedia/__init__.py
+-rw-r--r--   0        0        0      628 2024-05-06 14:45:38.948789 gigachain-0.2.0/langchain/tools/wikipedia/tool.py
+-rw-r--r--   0        0        0      670 2024-05-06 14:45:38.949362 gigachain-0.2.0/langchain/tools/wolfram_alpha/__init__.py
+-rw-r--r--   0        0        0      637 2024-05-06 14:45:38.949897 gigachain-0.2.0/langchain/tools/wolfram_alpha/tool.py
+-rw-r--r--   0        0        0      637 2024-05-06 14:45:38.950499 gigachain-0.2.0/langchain/tools/yahoo_finance_news.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.950523 gigachain-0.2.0/langchain/tools/youtube/__init__.py
+-rw-r--r--   0        0        0      628 2024-05-06 14:45:38.951060 gigachain-0.2.0/langchain/tools/youtube/search.py
+-rw-r--r--   0        0        0      764 2024-05-06 14:45:38.951711 gigachain-0.2.0/langchain/tools/zapier/__init__.py
+-rw-r--r--   0        0        0      745 2024-05-06 14:45:38.952300 gigachain-0.2.0/langchain/tools/zapier/tool.py
+-rw-r--r--   0        0        0     5891 2024-05-06 14:45:38.953277 gigachain-0.2.0/langchain/utilities/__init__.py
+-rw-r--r--   0        0        0      651 2024-05-06 14:45:38.953971 gigachain-0.2.0/langchain/utilities/alpha_vantage.py
+-rw-r--r--   0        0        0      839 2024-05-06 14:45:38.954555 gigachain-0.2.0/langchain/utilities/anthropic.py
+-rw-r--r--   0        0        0      621 2024-05-06 14:45:38.954975 gigachain-0.2.0/langchain/utilities/apify.py
+-rw-r--r--   0        0        0     1336 2024-05-06 14:45:38.955392 gigachain-0.2.0/langchain/utilities/arcee.py
+-rw-r--r--   0        0        0      630 2024-05-06 14:45:38.955948 gigachain-0.2.0/langchain/utilities/arxiv.py
+-rw-r--r--   0        0        0      274 2023-08-21 13:51:28.954857 gigachain-0.2.0/langchain/utilities/asyncio.py
+-rw-r--r--   0        0        0      624 2024-05-06 14:45:38.956486 gigachain-0.2.0/langchain/utilities/awslambda.py
+-rw-r--r--   0        0        0      642 2024-05-06 14:45:38.957005 gigachain-0.2.0/langchain/utilities/bibtex.py
+-rw-r--r--   0        0        0      645 2024-05-06 14:45:38.957627 gigachain-0.2.0/langchain/utilities/bing_search.py
+-rw-r--r--   0        0        0      639 2024-05-06 14:45:38.958220 gigachain-0.2.0/langchain/utilities/brave_search.py
+-rw-r--r--   0        0        0     1180 2024-05-06 14:45:38.958732 gigachain-0.2.0/langchain/utilities/clickup.py
+-rw-r--r--   0        0        0      680 2024-05-06 14:45:38.959224 gigachain-0.2.0/langchain/utilities/dalle_image_generator.py
+-rw-r--r--   0        0        0      695 2024-05-06 14:45:38.959759 gigachain-0.2.0/langchain/utilities/dataforseo_api_search.py
+-rw-r--r--   0        0        0      663 2024-05-06 14:45:38.960397 gigachain-0.2.0/langchain/utilities/duckduckgo_search.py
+-rw-r--r--   0        0        0      647 2024-05-06 14:45:38.960983 gigachain-0.2.0/langchain/utilities/github.py
+-rw-r--r--   0        0        0      647 2024-05-06 14:45:38.961609 gigachain-0.2.0/langchain/utilities/gitlab.py
+-rw-r--r--   0        0        0      648 2024-05-06 14:45:38.962213 gigachain-0.2.0/langchain/utilities/golden_query.py
+-rw-r--r--   0        0        0      654 2024-05-06 14:45:38.962768 gigachain-0.2.0/langchain/utilities/google_finance.py
+-rw-r--r--   0        0        0      645 2024-05-06 14:45:38.963356 gigachain-0.2.0/langchain/utilities/google_jobs.py
+-rw-r--r--   0        0        0      645 2024-05-06 14:45:38.964027 gigachain-0.2.0/langchain/utilities/google_lens.py
+-rw-r--r--   0        0        0      651 2024-05-06 14:45:38.964626 gigachain-0.2.0/langchain/utilities/google_places_api.py
+-rw-r--r--   0        0        0      654 2024-05-06 14:45:38.965375 gigachain-0.2.0/langchain/utilities/google_scholar.py
+-rw-r--r--   0        0        0      651 2024-05-06 14:45:38.965952 gigachain-0.2.0/langchain/utilities/google_search.py
+-rw-r--r--   0        0        0      651 2024-05-06 14:45:38.966542 gigachain-0.2.0/langchain/utilities/google_serper.py
+-rw-r--r--   0        0        0      651 2024-05-06 14:45:38.967180 gigachain-0.2.0/langchain/utilities/google_trends.py
+-rw-r--r--   0        0        0      636 2024-05-06 14:45:38.967816 gigachain-0.2.0/langchain/utilities/graphql.py
+-rw-r--r--   0        0        0      627 2024-05-06 14:45:38.968540 gigachain-0.2.0/langchain/utilities/jira.py
+-rw-r--r--   0        0        0      122 2023-12-18 12:05:47.798009 gigachain-0.2.0/langchain/utilities/loading.py
+-rw-r--r--   0        0        0      645 2024-05-06 14:45:38.969150 gigachain-0.2.0/langchain/utilities/max_compute.py
+-rw-r--r--   0        0        0      657 2024-05-06 14:45:38.969828 gigachain-0.2.0/langchain/utilities/merriam_webster.py
+-rw-r--r--   0        0        0      657 2024-05-06 14:45:38.970455 gigachain-0.2.0/langchain/utilities/metaphor_search.py
+-rw-r--r--   0        0        0      627 2024-05-06 14:45:38.971048 gigachain-0.2.0/langchain/utilities/nasa.py
+-rw-r--r--   0        0        0      739 2024-05-06 14:45:38.972155 gigachain-0.2.0/langchain/utilities/opaqueprompts.py
+-rw-r--r--   0        0        0      753 2024-05-06 14:45:38.972704 gigachain-0.2.0/langchain/utilities/openapi.py
+-rw-r--r--   0        0        0      657 2024-05-06 14:45:38.973242 gigachain-0.2.0/langchain/utilities/openweathermap.py
+-rw-r--r--   0        0        0      636 2024-05-06 14:45:38.973783 gigachain-0.2.0/langchain/utilities/outline.py
+-rw-r--r--   0        0        0      606 2024-05-06 14:45:38.974163 gigachain-0.2.0/langchain/utilities/portkey.py
+-rw-r--r--   0        0        0      627 2024-05-06 14:45:38.976342 gigachain-0.2.0/langchain/utilities/powerbi.py
+-rw-r--r--   0        0        0      633 2024-05-06 14:45:38.976902 gigachain-0.2.0/langchain/utilities/pubmed.py
+-rw-r--r--   0        0        0      462 2024-05-24 11:13:19.354347 gigachain-0.2.0/langchain/utilities/python.py
+-rw-r--r--   0        0        0      685 2024-05-06 14:45:38.977405 gigachain-0.2.0/langchain/utilities/reddit_search.py
+-rw-r--r--   0        0        0      889 2024-05-06 14:45:38.977997 gigachain-0.2.0/langchain/utilities/redis.py
+-rw-r--r--   0        0        0      712 2024-05-06 14:45:38.978416 gigachain-0.2.0/langchain/utilities/requests.py
+-rw-r--r--   0        0        0      648 2024-05-06 14:45:38.979480 gigachain-0.2.0/langchain/utilities/scenexplain.py
+-rw-r--r--   0        0        0      642 2024-05-06 14:45:38.979883 gigachain-0.2.0/langchain/utilities/searchapi.py
+-rw-r--r--   0        0        0      804 2024-05-06 14:45:38.980207 gigachain-0.2.0/langchain/utilities/searx_search.py
+-rw-r--r--   0        0        0      782 2024-05-06 14:45:38.980769 gigachain-0.2.0/langchain/utilities/serpapi.py
+-rw-r--r--   0        0        0      609 2024-05-06 14:45:38.981275 gigachain-0.2.0/langchain/utilities/spark_sql.py
+-rw-r--r--   0        0        0      786 2024-05-06 14:45:38.981672 gigachain-0.2.0/langchain/utilities/sql_database.py
+-rw-r--r--   0        0        0      654 2024-05-06 14:45:38.982026 gigachain-0.2.0/langchain/utilities/stackexchange.py
+-rw-r--r--   0        0        0      639 2024-05-06 14:45:38.982495 gigachain-0.2.0/langchain/utilities/steam.py
+-rw-r--r--   0        0        0      685 2024-05-06 14:45:38.982931 gigachain-0.2.0/langchain/utilities/tavily_search.py
+-rw-r--r--   0        0        0      639 2024-05-06 14:45:38.983545 gigachain-0.2.0/langchain/utilities/tensorflow_datasets.py
+-rw-r--r--   0        0        0      633 2024-05-06 14:45:38.983985 gigachain-0.2.0/langchain/utilities/twilio.py
+-rw-r--r--   0        0        0     1056 2024-05-06 14:45:38.984340 gigachain-0.2.0/langchain/utilities/vertexai.py
+-rw-r--r--   0        0        0      642 2024-05-06 14:45:38.984795 gigachain-0.2.0/langchain/utilities/wikipedia.py
+-rw-r--r--   0        0        0      651 2024-05-06 14:45:38.985429 gigachain-0.2.0/langchain/utilities/wolfram_alpha.py
+-rw-r--r--   0        0        0      633 2024-05-06 14:45:38.985872 gigachain-0.2.0/langchain/utilities/zapier.py
+-rw-r--r--   0        0        0     1846 2024-05-06 14:45:38.986515 gigachain-0.2.0/langchain/utils/__init__.py
+-rw-r--r--   0        0        0      102 2023-12-18 12:05:47.825271 gigachain-0.2.0/langchain/utils/aiter.py
+-rw-r--r--   0        0        0      124 2023-12-18 12:05:47.826109 gigachain-0.2.0/langchain/utils/env.py
+-rw-r--r--   0        0        0     1140 2024-05-06 14:45:38.987050 gigachain-0.2.0/langchain/utils/ernie_functions.py
+-rw-r--r--   0        0        0       91 2023-12-18 12:05:47.827383 gigachain-0.2.0/langchain/utils/formatting.py
+-rw-r--r--   0        0        0      421 2023-12-18 12:05:47.828299 gigachain-0.2.0/langchain/utils/html.py
+-rw-r--r--   0        0        0      211 2023-12-18 12:05:47.829085 gigachain-0.2.0/langchain/utils/input.py
+-rw-r--r--   0        0        0      133 2023-12-18 12:05:47.829865 gigachain-0.2.0/langchain/utils/iter.py
+-rw-r--r--   0        0        0      258 2023-12-18 12:05:47.830615 gigachain-0.2.0/langchain/utils/json_schema.py
+-rw-r--r--   0        0        0       92 2023-12-18 12:05:47.831372 gigachain-0.2.0/langchain/utils/loading.py
+-rw-r--r--   0        0        0      918 2024-05-06 14:45:38.987413 gigachain-0.2.0/langchain/utils/math.py
+-rw-r--r--   0        0        0      627 2024-05-06 14:45:38.987746 gigachain-0.2.0/langchain/utils/openai.py
+-rw-r--r--   0        0        0      325 2024-05-06 14:45:38.988074 gigachain-0.2.0/langchain/utils/openai_functions.py
+-rw-r--r--   0        0        0      111 2023-12-18 12:05:47.835107 gigachain-0.2.0/langchain/utils/pydantic.py
+-rw-r--r--   0        0        0      148 2023-12-18 12:05:47.835836 gigachain-0.2.0/langchain/utils/strings.py
+-rw-r--r--   0        0        0      446 2023-12-18 12:05:47.836793 gigachain-0.2.0/langchain/utils/utils.py
+-rw-r--r--   0        0        0     8070 2024-05-24 11:13:19.355198 gigachain-0.2.0/langchain/vectorstores/__init__.py
+-rw-r--r--   0        0        0      833 2024-05-06 14:45:38.989121 gigachain-0.2.0/langchain/vectorstores/alibabacloud_opensearch.py
+-rw-r--r--   0        0        0      621 2024-05-06 14:45:38.989547 gigachain-0.2.0/langchain/vectorstores/analyticdb.py
+-rw-r--r--   0        0        0      606 2024-05-06 14:45:38.990137 gigachain-0.2.0/langchain/vectorstores/annoy.py
+-rw-r--r--   0        0        0      612 2024-05-06 14:45:38.990509 gigachain-0.2.0/langchain/vectorstores/astradb.py
+-rw-r--r--   0        0        0      612 2024-05-06 14:45:38.990838 gigachain-0.2.0/langchain/vectorstores/atlas.py
+-rw-r--r--   0        0        0      606 2024-05-06 14:45:38.991250 gigachain-0.2.0/langchain/vectorstores/awadb.py
+-rw-r--r--   0        0        0      873 2024-05-06 14:45:38.991807 gigachain-0.2.0/langchain/vectorstores/azure_cosmos_db.py
+-rw-r--r--   0        0        0      867 2024-05-06 14:45:38.992338 gigachain-0.2.0/langchain/vectorstores/azuresearch.py
+-rw-r--r--   0        0        0      606 2024-05-06 14:45:38.992837 gigachain-0.2.0/langchain/vectorstores/bageldb.py
+-rw-r--r--   0        0        0      633 2024-05-06 14:45:38.993437 gigachain-0.2.0/langchain/vectorstores/baiducloud_vector_search.py
+-rw-r--r--   0        0        0      125 2023-12-18 12:05:47.847689 gigachain-0.2.0/langchain/vectorstores/base.py
+-rw-r--r--   0        0        0      618 2024-05-06 14:45:38.993964 gigachain-0.2.0/langchain/vectorstores/cassandra.py
+-rw-r--r--   0        0        0      609 2024-05-06 14:45:38.994482 gigachain-0.2.0/langchain/vectorstores/chroma.py
+-rw-r--r--   0        0        0      615 2024-05-06 14:45:38.994965 gigachain-0.2.0/langchain/vectorstores/clarifai.py
+-rw-r--r--   0        0        0      736 2024-05-06 14:45:38.995507 gigachain-0.2.0/langchain/vectorstores/clickhouse.py
+-rw-r--r--   0        0        0      621 2024-05-06 14:45:38.996007 gigachain-0.2.0/langchain/vectorstores/dashvector.py
+-rw-r--r--   0        0        0      657 2024-05-06 14:45:38.996539 gigachain-0.2.0/langchain/vectorstores/databricks_vector_search.py
+-rw-r--r--   0        0        0      615 2024-05-06 14:45:38.997078 gigachain-0.2.0/langchain/vectorstores/deeplake.py
+-rw-r--r--   0        0        0      606 2024-05-06 14:45:38.997728 gigachain-0.2.0/langchain/vectorstores/dingo.py
+-rw-r--r--   0        0        0      797 2024-05-06 14:45:38.998315 gigachain-0.2.0/langchain/vectorstores/docarray/__init__.py
+-rw-r--r--   0        0        0      658 2024-05-06 14:45:38.998845 gigachain-0.2.0/langchain/vectorstores/docarray/base.py
+-rw-r--r--   0        0        0      645 2024-05-06 14:45:38.999349 gigachain-0.2.0/langchain/vectorstores/docarray/hnsw.py
+-rw-r--r--   0        0        0      657 2024-05-06 14:45:38.999902 gigachain-0.2.0/langchain/vectorstores/docarray/in_memory.py
+-rw-r--r--   0        0        0      757 2024-05-06 14:45:39.000566 gigachain-0.2.0/langchain/vectorstores/elastic_vector_search.py
+-rw-r--r--   0        0        0     1294 2024-05-06 14:45:39.001090 gigachain-0.2.0/langchain/vectorstores/elasticsearch.py
+-rw-r--r--   0        0        0      612 2024-05-06 14:45:39.001598 gigachain-0.2.0/langchain/vectorstores/epsilla.py
+-rw-r--r--   0        0        0      606 2024-05-06 14:45:39.002121 gigachain-0.2.0/langchain/vectorstores/faiss.py
+-rw-r--r--   0        0        0      618 2024-05-06 14:45:39.002641 gigachain-0.2.0/langchain/vectorstores/hippo.py
+-rw-r--r--   0        0        0      615 2024-05-06 14:45:39.003144 gigachain-0.2.0/langchain/vectorstores/hologres.py
+-rw-r--r--   0        0        0      612 2024-05-06 14:45:39.003608 gigachain-0.2.0/langchain/vectorstores/lancedb.py
+-rw-r--r--   0        0        0      795 2024-05-06 14:45:39.004140 gigachain-0.2.0/langchain/vectorstores/llm_rails.py
+-rw-r--r--   0        0        0      606 2024-05-06 14:45:39.004607 gigachain-0.2.0/langchain/vectorstores/marqo.py
+-rw-r--r--   0        0        0      633 2024-05-06 14:45:39.005089 gigachain-0.2.0/langchain/vectorstores/matching_engine.py
+-rw-r--r--   0        0        0      624 2024-05-06 14:45:39.005565 gigachain-0.2.0/langchain/vectorstores/meilisearch.py
+-rw-r--r--   0        0        0      609 2024-05-06 14:45:39.006096 gigachain-0.2.0/langchain/vectorstores/milvus.py
+-rw-r--r--   0        0        0      645 2024-05-06 14:45:39.006755 gigachain-0.2.0/langchain/vectorstores/momento_vector_index.py
+-rw-r--r--   0        0        0      663 2024-05-06 14:45:39.007336 gigachain-0.2.0/langchain/vectorstores/mongodb_atlas.py
+-rw-r--r--   0        0        0      890 2024-05-06 14:45:39.007862 gigachain-0.2.0/langchain/vectorstores/myscale.py
+-rw-r--r--   0        0        0      789 2024-05-06 14:45:39.008434 gigachain-0.2.0/langchain/vectorstores/neo4j_vector.py
+-rw-r--r--   0        0        0      633 2024-05-06 14:45:39.008945 gigachain-0.2.0/langchain/vectorstores/nucliadb.py
+-rw-r--r--   0        0        0      657 2024-05-06 14:45:39.009480 gigachain-0.2.0/langchain/vectorstores/opensearch_vector_search.py
+-rw-r--r--   0        0        0     1042 2024-05-06 14:45:39.010007 gigachain-0.2.0/langchain/vectorstores/pgembedding.py
+-rw-r--r--   0        0        0      643 2024-05-06 14:45:39.010529 gigachain-0.2.0/langchain/vectorstores/pgvecto_rs.py
+-rw-r--r--   0        0        0      790 2024-05-06 14:45:39.011074 gigachain-0.2.0/langchain/vectorstores/pgvector.py
+-rw-r--r--   0        0        0      615 2024-05-06 14:45:39.011620 gigachain-0.2.0/langchain/vectorstores/pinecone.py
+-rw-r--r--   0        0        0      777 2024-05-06 14:45:39.012215 gigachain-0.2.0/langchain/vectorstores/qdrant.py
+-rw-r--r--   0        0        0     1295 2024-05-06 14:45:39.012867 gigachain-0.2.0/langchain/vectorstores/redis/__init__.py
+-rw-r--r--   0        0        0      956 2024-05-06 14:45:39.013394 gigachain-0.2.0/langchain/vectorstores/redis/base.py
+-rw-r--r--   0        0        0     1514 2024-05-06 14:45:39.013870 gigachain-0.2.0/langchain/vectorstores/redis/filters.py
+-rw-r--r--   0        0        0     1745 2024-05-06 14:45:39.014385 gigachain-0.2.0/langchain/vectorstores/redis/schema.py
+-rw-r--r--   0        0        0      612 2024-05-06 14:45:39.014921 gigachain-0.2.0/langchain/vectorstores/rocksetdb.py
+-rw-r--r--   0        0        0      606 2024-05-06 14:45:39.015427 gigachain-0.2.0/langchain/vectorstores/scann.py
+-rw-r--r--   0        0        0      609 2024-05-06 14:45:39.015924 gigachain-0.2.0/langchain/vectorstores/semadb.py
+-rw-r--r--   0        0        0      630 2024-05-06 14:45:39.016406 gigachain-0.2.0/langchain/vectorstores/singlestoredb.py
+-rw-r--r--   0        0        0     1325 2024-05-06 14:45:39.016966 gigachain-0.2.0/langchain/vectorstores/sklearn.py
+-rw-r--r--   0        0        0      618 2024-05-06 14:45:39.017458 gigachain-0.2.0/langchain/vectorstores/sqlitevss.py
+-rw-r--r--   0        0        0      798 2024-05-06 14:45:39.017972 gigachain-0.2.0/langchain/vectorstores/starrocks.py
+-rw-r--r--   0        0        0      648 2024-05-06 14:45:39.018459 gigachain-0.2.0/langchain/vectorstores/supabase.py
+-rw-r--r--   0        0        0      603 2024-05-06 14:45:39.018928 gigachain-0.2.0/langchain/vectorstores/tair.py
+-rw-r--r--   0        0        0      953 2024-05-06 14:45:39.019289 gigachain-0.2.0/langchain/vectorstores/tencentvectordb.py
+-rw-r--r--   0        0        0      609 2024-05-06 14:45:39.019628 gigachain-0.2.0/langchain/vectorstores/tigris.py
+-rw-r--r--   0        0        0      609 2024-05-06 14:45:39.020195 gigachain-0.2.0/langchain/vectorstores/tiledb.py
+-rw-r--r--   0        0        0      636 2024-05-06 14:45:39.022188 gigachain-0.2.0/langchain/vectorstores/timescalevector.py
+-rw-r--r--   0        0        0      618 2024-05-06 14:45:39.023401 gigachain-0.2.0/langchain/vectorstores/typesense.py
+-rw-r--r--   0        0        0      612 2024-05-06 14:45:39.023776 gigachain-0.2.0/langchain/vectorstores/usearch.py
+-rw-r--r--   0        0        0      958 2024-05-06 14:45:39.024114 gigachain-0.2.0/langchain/vectorstores/utils.py
+-rw-r--r--   0        0        0      603 2024-05-06 14:45:39.024490 gigachain-0.2.0/langchain/vectorstores/vald.py
+-rw-r--r--   0        0        0      609 2024-05-06 14:45:39.025001 gigachain-0.2.0/langchain/vectorstores/vearch.py
+-rw-r--r--   0        0        0      785 2024-05-06 14:45:39.025367 gigachain-0.2.0/langchain/vectorstores/vectara.py
+-rw-r--r--   0        0        0      621 2024-05-06 14:45:39.025831 gigachain-0.2.0/langchain/vectorstores/vespa.py
+-rw-r--r--   0        0        0      615 2024-05-06 14:45:39.026661 gigachain-0.2.0/langchain/vectorstores/weaviate.py
+-rw-r--r--   0        0        0      646 2024-05-06 14:45:39.027194 gigachain-0.2.0/langchain/vectorstores/xata.py
+-rw-r--r--   0        0        0      624 2024-05-06 14:45:39.027582 gigachain-0.2.0/langchain/vectorstores/yellowbrick.py
+-rw-r--r--   0        0        0      798 2024-05-06 14:45:39.027929 gigachain-0.2.0/langchain/vectorstores/zep.py
+-rw-r--r--   0        0        0      609 2024-05-06 14:45:39.028396 gigachain-0.2.0/langchain/vectorstores/zilliz.py
+-rw-r--r--   0        0        0    11838 2024-05-24 11:13:19.372586 gigachain-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    13776 1970-01-01 00:00:00.000000 gigachain-0.2.0/PKG-INFO
```

### Comparing `gigachain-0.1.9/LICENSE` & `gigachain-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/README.md` & `gigachain-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -30,63 +30,59 @@
 
 ## 🤔 What is this?
 
 Large language models (LLMs) are emerging as a transformative technology, enabling developers to build applications that they previously could not. However, using these LLMs in isolation is often insufficient for creating a truly powerful app - the real power comes when you can combine them with other sources of computation or knowledge.
 
 This library aims to assist in the development of those types of applications. Common examples of these applications include:
 
-**❓ Question Answering over specific documents**
+**❓ Question answering with RAG**
 
 - [Documentation](https://python.langchain.com/docs/use_cases/question_answering/)
-- End-to-end Example: [Question Answering over Notion Database](https://github.com/hwchase17/notion-qa)
+- End-to-end Example: [Chat LangChain](https://chat.langchain.com) and [repo](https://github.com/langchain-ai/chat-langchain)
 
-**💬 Chatbots**
+**🧱 Extracting structured output**
 
-- [Documentation](https://python.langchain.com/docs/use_cases/chatbots/)
-- End-to-end Example: [Chat-LangChain](https://github.com/langchain-ai/chat-langchain)
+- [Documentation](https://python.langchain.com/docs/use_cases/extraction/)
+- End-to-end Example: [SQL Llama2 Template](https://github.com/langchain-ai/langchain-extract/)
 
-**🤖 Agents**
+**🤖 Chatbots**
 
-- [Documentation](https://python.langchain.com/docs/modules/agents/)
-- End-to-end Example: [GPT+WolframAlpha](https://huggingface.co/spaces/JavaFXpert/Chat-GPT-LangChain)
+- [Documentation](https://python.langchain.com/docs/use_cases/chatbots)
+- End-to-end Example: [Web LangChain (web researcher chatbot)](https://weblangchain.vercel.app) and [repo](https://github.com/langchain-ai/weblangchain)
 
 ## 📖 Documentation
 
 Please see [here](https://python.langchain.com) for full documentation on:
 
 - Getting started (installation, setting up the environment, simple examples)
 - How-To examples (demos, integrations, helper functions)
 - Reference (full API docs)
 - Resources (high-level explanation of core concepts)
 
 ## 🚀 What can this help with?
 
-There are six main areas that LangChain is designed to help with.
+There are five main areas that LangChain is designed to help with.
 These are, in increasing order of complexity:
 
-**📃 LLMs and Prompts:**
+**📃 Models and Prompts:**
 
-This includes prompt management, prompt optimization, a generic interface for all LLMs, and common utilities for working with LLMs.
+This includes prompt management, prompt optimization, a generic interface for all LLMs, and common utilities for working with chat models and LLMs.
 
 **🔗 Chains:**
 
 Chains go beyond a single LLM call and involve sequences of calls (whether to an LLM or a different utility). LangChain provides a standard interface for chains, lots of integrations with other tools, and end-to-end chains for common applications.
 
-**📚 Data Augmented Generation:**
+**📚 Retrieval Augmented Generation:**
 
-Data Augmented Generation involves specific types of chains that first interact with an external data source to fetch data for use in the generation step. Examples include summarization of long pieces of text and question/answering over specific data sources.
+Retrieval Augmented Generation involves specific types of chains that first interact with an external data source to fetch data for use in the generation step. Examples include summarization of long pieces of text and question/answering over specific data sources.
 
 **🤖 Agents:**
 
 Agents involve an LLM making decisions about which Actions to take, taking that Action, seeing an Observation, and repeating that until done. LangChain provides a standard interface for agents, a selection of agents to choose from, and examples of end-to-end agents.
 
-**🧠 Memory:**
-
-Memory refers to persisting state between calls of a chain/agent. LangChain provides a standard interface for memory, a collection of memory implementations, and examples of chains/agents that use memory.
-
 **🧐 Evaluation:**
 
 [BETA] Generative models are notoriously hard to evaluate with traditional metrics. One new way of evaluating them is using language models themselves to do the evaluation. LangChain provides some prompts/chains for assisting in this.
 
 For more information on these concepts, please see our [full documentation](https://python.langchain.com).
 
 ## 💁 Contributing
```

### Comparing `gigachain-0.1.9/langchain/__init__.py` & `gigachain-0.2.0/langchain/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 # ruff: noqa: E402
 """Main entrypoint into package."""
+
 import warnings
 from importlib import metadata
 from typing import Any, Optional
 
-from langchain_community.__gigachain_community import _check_gigachain_community_version
-
-# Check that we have gigachain_core package instead of langchain_core
 from langchain_core.__gigachain_core import _check_gigachain_core_version
 from langchain_core._api.deprecation import surface_langchain_deprecation_warnings
 
 # Убелимся, что мы используем именно gigachain_core и gigachain_community,
 # а не соответствующие langchain_... версии
 _check_gigachain_core_version()
-_check_gigachain_community_version()
 
 
 try:
-    __version__ = metadata.version(__package__)
+    __version__ = metadata.version("gigachain")
 except metadata.PackageNotFoundError:
     # Case where package metadata is not available.
     __version__ = ""
 del metadata  # optional, avoids polluting the results of dir(__package__)
 
 
 def _warn_on_import(name: str, replacement: Optional[str] = None) -> None:
     """Warn on import of deprecated module."""
-    from langchain.utils.interactive_env import is_interactive_env
+    from langchain._api.interactive_env import is_interactive_env
 
     if is_interactive_env():
         # No warnings for interactive environments.
         # This is done to avoid polluting the output of interactive environments
         # where users rely on auto-complete and may trigger this warning
         # even if they are not using any deprecated modules
         return
@@ -118,21 +115,21 @@
     elif name == "VectorDBQAWithSourcesChain":
         from langchain.chains import VectorDBQAWithSourcesChain
 
         _warn_on_import(name, replacement="langchain.chains.VectorDBQAWithSourcesChain")
 
         return VectorDBQAWithSourcesChain
     elif name == "InMemoryDocstore":
-        from langchain.docstore import InMemoryDocstore
+        from langchain_community.docstore import InMemoryDocstore
 
         _warn_on_import(name, replacement="langchain.docstore.InMemoryDocstore")
 
         return InMemoryDocstore
     elif name == "Wikipedia":
-        from langchain.docstore import Wikipedia
+        from langchain_community.docstore import Wikipedia
 
         _warn_on_import(name, replacement="langchain.docstore.Wikipedia")
 
         return Wikipedia
     elif name == "Anthropic":
         from langchain_community.llms import Anthropic
 
@@ -239,35 +236,37 @@
             replacement="langchain_community.llms.huggingface_pipeline.HuggingFacePipeline",
         )
 
         return HuggingFacePipeline
     elif name == "FewShotPromptTemplate":
         from langchain_core.prompts import FewShotPromptTemplate
 
-        _warn_on_import(name, replacement="langchain.prompts.FewShotPromptTemplate")
+        _warn_on_import(
+            name, replacement="langchain_core.prompts.FewShotPromptTemplate"
+        )
 
         return FewShotPromptTemplate
     elif name == "Prompt":
-        from langchain.prompts import Prompt
+        from langchain_core.prompts import PromptTemplate
 
-        _warn_on_import(name, replacement="langchain.prompts.Prompt")
+        _warn_on_import(name, replacement="langchain_core.prompts.PromptTemplate")
 
-        return Prompt
+        # it's renamed as prompt template anyways
+        # this is just for backwards compat
+        return PromptTemplate
     elif name == "PromptTemplate":
         from langchain_core.prompts import PromptTemplate
 
-        _warn_on_import(name, replacement="langchain.prompts.PromptTemplate")
+        _warn_on_import(name, replacement="langchain_core.prompts.PromptTemplate")
 
         return PromptTemplate
     elif name == "BasePromptTemplate":
         from langchain_core.prompts import BasePromptTemplate
 
-        _warn_on_import(
-            name, replacement="langchain.schema.prompt_template.BasePromptTemplate"
-        )
+        _warn_on_import(name, replacement="langchain_core.prompts.BasePromptTemplate")
 
         return BasePromptTemplate
     elif name == "ArxivAPIWrapper":
         from langchain_community.utilities import ArxivAPIWrapper
 
         _warn_on_import(
             name, replacement="langchain_community.utilities.ArxivAPIWrapper"
```

### Comparing `gigachain-0.1.9/langchain/_api/__init__.py` & `gigachain-0.2.0/langchain/_api/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 from .deprecation import (
     LangChainDeprecationWarning,
     deprecated,
     suppress_langchain_deprecation_warning,
     surface_langchain_deprecation_warnings,
     warn_deprecated,
 )
+from .module_import import create_importer
 
 __all__ = [
     "deprecated",
     "LangChainDeprecationWarning",
     "suppress_langchain_deprecation_warning",
     "surface_langchain_deprecation_warnings",
     "warn_deprecated",
+    "create_importer",
 ]
```

### Comparing `gigachain-0.1.9/langchain/agents/__init__.py` & `gigachain-0.2.0/langchain/agents/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,40 +11,35 @@
 
 .. code-block::
 
     BaseSingleActionAgent --> LLMSingleActionAgent
                               OpenAIFunctionsAgent
                               XMLAgent
                               Agent --> <name>Agent  # Examples: ZeroShotAgent, ChatAgent
-                                        
+
 
     BaseMultiActionAgent  --> OpenAIMultiFunctionsAgent
-    
-    
+
+
 **Main helpers:**
 
 .. code-block::
 
     AgentType, AgentExecutor, AgentOutputParser, AgentExecutorIterator,
     AgentAction, AgentFinish
-    
+
 """  # noqa: E501
+
 from pathlib import Path
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
-from langchain_community.agent_toolkits import (
-    create_json_agent,
-    create_openapi_agent,
-    create_pbi_agent,
-    create_pbi_chat_agent,
-    create_spark_sql_agent,
-    create_sql_agent,
-)
 from langchain_core._api.path import as_import_path
+from langchain_core.tools import Tool, tool
 
+from langchain._api import create_importer
 from langchain.agents.agent import (
     Agent,
     AgentExecutor,
     AgentOutputParser,
     BaseMultiActionAgent,
     BaseSingleActionAgent,
     LLMSingleActionAgent,
@@ -58,19 +53,14 @@
 from langchain.agents.conversational.base import ConversationalAgent
 from langchain.agents.conversational_chat.base import ConversationalChatAgent
 from langchain.agents.gigachat_functions_agent.base import (
     create_gigachat_functions_agent,
 )
 from langchain.agents.initialize import initialize_agent
 from langchain.agents.json_chat.base import create_json_chat_agent
-from langchain.agents.load_tools import (
-    get_all_tool_names,
-    load_huggingface_tool,
-    load_tools,
-)
 from langchain.agents.loading import load_agent
 from langchain.agents.mrkl.base import MRKLChain, ZeroShotAgent
 from langchain.agents.openai_functions_agent.base import (
     OpenAIFunctionsAgent,
     create_openai_functions_agent,
 )
 from langchain.agents.openai_functions_multi_agent.base import OpenAIMultiFunctionsAgent
@@ -81,24 +71,56 @@
     SelfAskWithSearchChain,
     create_self_ask_with_search_agent,
 )
 from langchain.agents.structured_chat.base import (
     StructuredChatAgent,
     create_structured_chat_agent,
 )
-from langchain.agents.tools import Tool, tool
+from langchain.agents.tool_calling_agent.base import create_tool_calling_agent
 from langchain.agents.xml.base import XMLAgent, create_xml_agent
 
+if TYPE_CHECKING:
+    from langchain_community.agent_toolkits.json.base import create_json_agent
+    from langchain_community.agent_toolkits.load_tools import (
+        get_all_tool_names,
+        load_huggingface_tool,
+        load_tools,
+    )
+    from langchain_community.agent_toolkits.openapi.base import create_openapi_agent
+    from langchain_community.agent_toolkits.powerbi.base import create_pbi_agent
+    from langchain_community.agent_toolkits.powerbi.chat_base import (
+        create_pbi_chat_agent,
+    )
+    from langchain_community.agent_toolkits.spark_sql.base import create_spark_sql_agent
+    from langchain_community.agent_toolkits.sql.base import create_sql_agent
+
 DEPRECATED_CODE = [
     "create_csv_agent",
     "create_pandas_dataframe_agent",
     "create_spark_dataframe_agent",
     "create_xorbits_agent",
 ]
 
+# Create a way to dynamically look up deprecated imports.
+# Used to consolidate logic for raising deprecation warnings and
+# handling optional imports.
+DEPRECATED_LOOKUP = {
+    "create_json_agent": "langchain_community.agent_toolkits.json.base",
+    "create_openapi_agent": "langchain_community.agent_toolkits.openapi.base",
+    "create_pbi_agent": "langchain_community.agent_toolkits.powerbi.base",
+    "create_pbi_chat_agent": "langchain_community.agent_toolkits.powerbi.chat_base",
+    "create_spark_sql_agent": "langchain_community.agent_toolkits.spark_sql.base",
+    "create_sql_agent": "langchain_community.agent_toolkits.sql.base",
+    "load_tools": "langchain_community.agent_toolkits.load_tools",
+    "load_huggingface_tool": "langchain_community.agent_toolkits.load_tools",
+    "get_all_tool_names": "langchain_community.agent_toolkits.load_tools",
+}
+
+_import_attribute = create_importer(__package__, deprecated_lookups=DEPRECATED_LOOKUP)
+
 
 def __getattr__(name: str) -> Any:
     """Get attr name."""
     if name in DEPRECATED_CODE:
         # Get directory of langchain package
         HERE = Path(__file__).parents[1]
         relative_path = as_import_path(
@@ -108,15 +130,15 @@
         new_path = "langchain_experimental." + relative_path
         raise ImportError(
             f"{name} has been moved to langchain experimental. "
             "See https://github.com/langchain-ai/langchain/discussions/11680"
             "for more information.\n"
             f"Please update your import statement from: `{old_path}` to `{new_path}`."
         )
-    raise AttributeError(f"{name} does not exist")
+    return _import_attribute(name)
 
 
 __all__ = [
     "Agent",
     "AgentExecutor",
     "AgentExecutorIterator",
     "AgentOutputParser",
@@ -154,8 +176,9 @@
     "create_gigachat_functions_agent",
     "create_xml_agent",
     "create_react_agent",
     "create_openai_tools_agent",
     "create_self_ask_with_search_agent",
     "create_json_chat_agent",
     "create_structured_chat_agent",
+    "create_tool_calling_agent",
 ]
```

### Comparing `gigachain-0.1.9/langchain/agents/agent.py` & `gigachain-0.2.0/langchain/agents/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Chain that takes in an input and produces an action and action input."""
+
 from __future__ import annotations
 
 import asyncio
 import json
 import logging
 import time
 from abc import abstractmethod
@@ -341,14 +342,22 @@
 class RunnableAgent(BaseSingleActionAgent):
     """Agent powered by runnables."""
 
     runnable: Runnable[dict, Union[AgentAction, AgentFinish]]
     """Runnable to call to get agent action."""
     input_keys_arg: List[str] = []
     return_keys_arg: List[str] = []
+    stream_runnable: bool = True
+    """Whether to stream from the runnable or not.
+
+    If True then underlying LLM is invoked in a streaming fashion to make it possible
+        to get access to the individual LLM tokens when using stream_log with the Agent
+        Executor. If False then LLM is invoked in a non-streaming fashion and
+        individual LLM tokens will not be available in stream_log.
+    """
 
     class Config:
         """Configuration for this pydantic object."""
 
         arbitrary_types_allowed = True
 
     @property
@@ -374,25 +383,29 @@
             callbacks: Callbacks to run.
             **kwargs: User inputs.
 
         Returns:
             Action specifying what tool to use.
         """
         inputs = {**kwargs, **{"intermediate_steps": intermediate_steps}}
-        # Use streaming to make sure that the underlying LLM is invoked in a streaming
-        # fashion to make it possible to get access to the individual LLM tokens
-        # when using stream_log with the Agent Executor.
-        # Because the response from the plan is not a generator, we need to
-        # accumulate the output into final output and return that.
         final_output: Any = None
-        for chunk in self.runnable.stream(inputs, config={"callbacks": callbacks}):
-            if final_output is None:
-                final_output = chunk
-            else:
-                final_output += chunk
+        if self.stream_runnable:
+            # Use streaming to make sure that the underlying LLM is invoked in a
+            # streaming
+            # fashion to make it possible to get access to the individual LLM tokens
+            # when using stream_log with the Agent Executor.
+            # Because the response from the plan is not a generator, we need to
+            # accumulate the output into final output and return that.
+            for chunk in self.runnable.stream(inputs, config={"callbacks": callbacks}):
+                if final_output is None:
+                    final_output = chunk
+                else:
+                    final_output += chunk
+        else:
+            final_output = self.runnable.invoke(inputs, config={"callbacks": callbacks})
 
         return final_output
 
     async def aplan(
         self,
         intermediate_steps: List[Tuple[AgentAction, str]],
         callbacks: Callbacks = None,
@@ -410,36 +423,50 @@
             **kwargs: User inputs
 
         Returns:
             Action specifying what tool to use.
         """
         inputs = {**kwargs, **{"intermediate_steps": intermediate_steps}}
         final_output: Any = None
-        # Use streaming to make sure that the underlying LLM is invoked in a streaming
-        # fashion to make it possible to get access to the individual LLM tokens
-        # when using stream_log with the Agent Executor.
-        # Because the response from the plan is not a generator, we need to
-        # accumulate the output into final output and return that.
-        async for chunk in self.runnable.astream(
-            inputs, config={"callbacks": callbacks}
-        ):
-            if final_output is None:
-                final_output = chunk
-            else:
-                final_output += chunk
+        if self.stream_runnable:
+            # Use streaming to make sure that the underlying LLM is invoked in a
+            # streaming
+            # fashion to make it possible to get access to the individual LLM tokens
+            # when using stream_log with the Agent Executor.
+            # Because the response from the plan is not a generator, we need to
+            # accumulate the output into final output and return that.
+            async for chunk in self.runnable.astream(
+                inputs, config={"callbacks": callbacks}
+            ):
+                if final_output is None:
+                    final_output = chunk
+                else:
+                    final_output += chunk
+        else:
+            final_output = await self.runnable.ainvoke(
+                inputs, config={"callbacks": callbacks}
+            )
         return final_output
 
 
 class RunnableMultiActionAgent(BaseMultiActionAgent):
     """Agent powered by runnables."""
 
     runnable: Runnable[dict, Union[List[AgentAction], AgentFinish]]
     """Runnable to call to get agent actions."""
     input_keys_arg: List[str] = []
     return_keys_arg: List[str] = []
+    stream_runnable: bool = True
+    """Whether to stream from the runnable or not.
+
+    If True then underlying LLM is invoked in a streaming fashion to make it possible
+        to get access to the individual LLM tokens when using stream_log with the Agent
+        Executor. If False then LLM is invoked in a non-streaming fashion and
+        individual LLM tokens will not be available in stream_log.
+    """
 
     class Config:
         """Configuration for this pydantic object."""
 
         arbitrary_types_allowed = True
 
     @property
@@ -473,25 +500,29 @@
             callbacks: Callbacks to run.
             **kwargs: User inputs.
 
         Returns:
             Action specifying what tool to use.
         """
         inputs = {**kwargs, **{"intermediate_steps": intermediate_steps}}
-        # Use streaming to make sure that the underlying LLM is invoked in a streaming
-        # fashion to make it possible to get access to the individual LLM tokens
-        # when using stream_log with the Agent Executor.
-        # Because the response from the plan is not a generator, we need to
-        # accumulate the output into final output and return that.
         final_output: Any = None
-        for chunk in self.runnable.stream(inputs, config={"callbacks": callbacks}):
-            if final_output is None:
-                final_output = chunk
-            else:
-                final_output += chunk
+        if self.stream_runnable:
+            # Use streaming to make sure that the underlying LLM is invoked in a
+            # streaming
+            # fashion to make it possible to get access to the individual LLM tokens
+            # when using stream_log with the Agent Executor.
+            # Because the response from the plan is not a generator, we need to
+            # accumulate the output into final output and return that.
+            for chunk in self.runnable.stream(inputs, config={"callbacks": callbacks}):
+                if final_output is None:
+                    final_output = chunk
+                else:
+                    final_output += chunk
+        else:
+            final_output = self.runnable.invoke(inputs, config={"callbacks": callbacks})
 
         return final_output
 
     async def aplan(
         self,
         intermediate_steps: List[Tuple[AgentAction, str]],
         callbacks: Callbacks = None,
@@ -508,38 +539,44 @@
             callbacks: Callbacks to run.
             **kwargs: User inputs.
 
         Returns:
             Action specifying what tool to use.
         """
         inputs = {**kwargs, **{"intermediate_steps": intermediate_steps}}
-        # Use streaming to make sure that the underlying LLM is invoked in a streaming
-        # fashion to make it possible to get access to the individual LLM tokens
-        # when using stream_log with the Agent Executor.
-        # Because the response from the plan is not a generator, we need to
-        # accumulate the output into final output and return that.
         final_output: Any = None
-        async for chunk in self.runnable.astream(
-            inputs, config={"callbacks": callbacks}
-        ):
-            if final_output is None:
-                final_output = chunk
-            else:
-                final_output += chunk
+        if self.stream_runnable:
+            # Use streaming to make sure that the underlying LLM is invoked in a
+            # streaming
+            # fashion to make it possible to get access to the individual LLM tokens
+            # when using stream_log with the Agent Executor.
+            # Because the response from the plan is not a generator, we need to
+            # accumulate the output into final output and return that.
+            async for chunk in self.runnable.astream(
+                inputs, config={"callbacks": callbacks}
+            ):
+                if final_output is None:
+                    final_output = chunk
+                else:
+                    final_output += chunk
+        else:
+            final_output = await self.runnable.ainvoke(
+                inputs, config={"callbacks": callbacks}
+            )
 
         return final_output
 
 
 @deprecated(
     "0.1.0",
     alternative=(
         "Use new agent constructor methods like create_react_agent, create_json_agent, "
         "create_structured_chat_agent, etc."
     ),
-    removal="0.2.0",
+    removal="0.3.0",
 )
 class LLMSingleActionAgent(BaseSingleActionAgent):
     """Base class for single action agents."""
 
     llm_chain: LLMChain
     """LLMChain to use for agent."""
     output_parser: AgentOutputParser
@@ -621,15 +658,15 @@
 
 @deprecated(
     "0.1.0",
     alternative=(
         "Use new agent constructor methods like create_react_agent, create_json_agent, "
         "create_structured_chat_agent, etc."
     ),
-    removal="0.2.0",
+    removal="0.3.0",
 )
 class Agent(BaseSingleActionAgent):
     """Agent that calls the language model and deciding the action.
 
     This is driven by an LLMChain. The prompt in the LLMChain MUST include
     a variable called "agent_scratchpad" where the agent can put its
     intermediary work.
@@ -886,27 +923,27 @@
     """The valid tools the agent can call."""
     return_intermediate_steps: bool = False
     """Whether to return the agent's trajectory of intermediate steps
     at the end in addition to the final output."""
     max_iterations: Optional[int] = 15
     """The maximum number of steps to take before ending the execution
     loop.
-    
+
     Setting to 'None' could lead to an infinite loop."""
     max_execution_time: Optional[float] = None
     """The maximum amount of wall clock time to spend in the execution
     loop.
     """
     early_stopping_method: str = "force"
     """The method to use for early stopping if the agent never
     returns `AgentFinish`. Either 'force' or 'generate'.
 
     `"force"` returns a string saying that it stopped because it met a
         time or iteration limit.
-    
+
     `"generate"` calls the agent's LLM Chain one final time to generate
         a final answer based on the previous steps.
     """
     handle_parsing_errors: Union[
         bool, str, Callable[[OutputParserException], str]
     ] = False
     """How to handle errors raised by the agent's output parser.
@@ -973,18 +1010,23 @@
             try:
                 output_type = agent.OutputType
             except Exception as _:
                 multi_action = False
             else:
                 multi_action = output_type == Union[List[AgentAction], AgentFinish]
 
+            stream_runnable = values.pop("stream_runnable", True)
             if multi_action:
-                values["agent"] = RunnableMultiActionAgent(runnable=agent)
+                values["agent"] = RunnableMultiActionAgent(
+                    runnable=agent, stream_runnable=stream_runnable
+                )
             else:
-                values["agent"] = RunnableAgent(runnable=agent)
+                values["agent"] = RunnableAgent(
+                    runnable=agent, stream_runnable=stream_runnable
+                )
         return values
 
     def save(self, file_path: Union[Path, str]) -> None:
         """Raise error - saving not supported for Agent Executors."""
         raise ValueError(
             "Saving not supported for agent executors. "
             "If you are trying to save the agent, please use the "
@@ -1520,14 +1562,15 @@
         iterator = AgentExecutorIterator(
             self,
             input,
             config.get("callbacks"),
             tags=config.get("tags"),
             metadata=config.get("metadata"),
             run_name=config.get("run_name"),
+            run_id=config.get("run_id"),
             yield_actions=True,
             **kwargs,
         )
         for step in iterator:
             yield step
 
     async def astream(
@@ -1541,12 +1584,13 @@
         iterator = AgentExecutorIterator(
             self,
             input,
             config.get("callbacks"),
             tags=config.get("tags"),
             metadata=config.get("metadata"),
             run_name=config.get("run_name"),
+            run_id=config.get("run_id"),
             yield_actions=True,
             **kwargs,
         )
         async for step in iterator:
             yield step
```

### Comparing `gigachain-0.1.9/langchain/agents/agent_iterator.py` & `gigachain-0.2.0/langchain/agents/agent_iterator.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     Dict,
     Iterator,
     List,
     Optional,
     Tuple,
     Union,
 )
+from uuid import UUID
 
 from langchain_core.agents import (
     AgentAction,
     AgentFinish,
     AgentStep,
 )
 from langchain_core.callbacks import (
@@ -50,36 +51,39 @@
         agent_executor: AgentExecutor,
         inputs: Any,
         callbacks: Callbacks = None,
         *,
         tags: Optional[list[str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         run_name: Optional[str] = None,
+        run_id: Optional[UUID] = None,
         include_run_info: bool = False,
         yield_actions: bool = False,
     ):
         """
         Initialize the AgentExecutorIterator with the given AgentExecutor,
         inputs, and optional callbacks.
         """
         self._agent_executor = agent_executor
         self.inputs = inputs
         self.callbacks = callbacks
         self.tags = tags
         self.metadata = metadata
         self.run_name = run_name
+        self.run_id = run_id
         self.include_run_info = include_run_info
         self.yield_actions = yield_actions
         self.reset()
 
     _inputs: Dict[str, str]
     callbacks: Callbacks
     tags: Optional[list[str]]
     metadata: Optional[Dict[str, Any]]
     run_name: Optional[str]
+    run_id: Optional[UUID]
     include_run_info: bool
     yield_actions: bool
 
     @property
     def inputs(self) -> Dict[str, str]:
         return self._inputs
 
@@ -158,14 +162,15 @@
             self.agent_executor.tags,
             self.metadata,
             self.agent_executor.metadata,
         )
         run_manager = callback_manager.on_chain_start(
             dumpd(self.agent_executor),
             self.inputs,
+            self.run_id,
             name=self.run_name,
         )
         try:
             while self.agent_executor._should_continue(
                 self.iterations, self.time_elapsed
             ):
                 # take the next step: this plans next action, executes it,
@@ -223,14 +228,15 @@
             self.agent_executor.tags,
             self.metadata,
             self.agent_executor.metadata,
         )
         run_manager = await callback_manager.on_chain_start(
             dumpd(self.agent_executor),
             self.inputs,
+            self.run_id,
             name=self.run_name,
         )
         try:
             async with asyncio_timeout(self.agent_executor.max_execution_time):
                 while self.agent_executor._should_continue(
                     self.iterations, self.time_elapsed
                 ):
```

### Comparing `gigachain-0.1.9/langchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py` & `gigachain-0.2.0/langchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import Any, List, Optional  # noqa: E501
 
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.memory import BaseMemory
 from langchain_core.messages import SystemMessage
 from langchain_core.prompts.chat import MessagesPlaceholder
+from langchain_core.tools import BaseTool
 
 from langchain.agents.agent import AgentExecutor
 from langchain.agents.openai_functions_agent.agent_token_buffer_memory import (
     AgentTokenBufferMemory,
 )
 from langchain.agents.openai_functions_agent.base import OpenAIFunctionsAgent
 from langchain.memory.token_buffer import ConversationTokenBufferMemory
-from langchain.tools.base import BaseTool
 
 
 def _get_default_system_message() -> SystemMessage:
     return SystemMessage(
         content=(
             "Do your best to answer the questions. "
             "Feel free to use any tools available to look up "
```

### Comparing `gigachain-0.1.9/langchain/agents/agent_toolkits/csv/__init__.py` & `gigachain-0.2.0/langchain/agents/agent_toolkits/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/agent_toolkits/pandas/__init__.py` & `gigachain-0.2.0/langchain/agents/agent_toolkits/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/agent_toolkits/python/__init__.py` & `gigachain-0.2.0/langchain/agents/agent_toolkits/python/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/agent_toolkits/spark/__init__.py` & `gigachain-0.2.0/langchain/agents/agent_toolkits/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/agent_toolkits/vectorstore/base.py` & `gigachain-0.2.0/langchain/agents/agent_toolkits/vectorstore/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """VectorStore agent."""
+
 from typing import Any, Dict, Optional
 
+from langchain_core.callbacks.base import BaseCallbackManager
 from langchain_core.language_models import BaseLanguageModel
 
 from langchain.agents.agent import AgentExecutor
 from langchain.agents.agent_toolkits.vectorstore.prompt import PREFIX, ROUTER_PREFIX
 from langchain.agents.agent_toolkits.vectorstore.toolkit import (
     VectorStoreRouterToolkit,
     VectorStoreToolkit,
 )
 from langchain.agents.mrkl.base import ZeroShotAgent
-from langchain.callbacks.base import BaseCallbackManager
 from langchain.chains.llm import LLMChain
 
 
 def create_vectorstore_agent(
     llm: BaseLanguageModel,
     toolkit: VectorStoreToolkit,
     callback_manager: Optional[BaseCallbackManager] = None,
```

### Comparing `gigachain-0.1.9/langchain/agents/agent_toolkits/vectorstore/prompt.py` & `gigachain-0.2.0/langchain/agents/agent_toolkits/vectorstore/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/agent_toolkits/vectorstore/toolkit.py` & `gigachain-0.2.0/langchain/agents/agent_toolkits/vectorstore/toolkit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 """Toolkit for interacting with a vector store."""
+
 from typing import List
 
-from langchain_community.agent_toolkits.base import BaseToolkit
-from langchain_community.llms.openai import OpenAI
-from langchain_community.tools.vectorstore.tool import (
-    VectorStoreQATool,
-    VectorStoreQAWithSourcesTool,
-)
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.pydantic_v1 import BaseModel, Field
+from langchain_core.tools import BaseTool, BaseToolkit
 from langchain_core.vectorstores import VectorStore
 
-from langchain.tools import BaseTool
-
 
 class VectorStoreInfo(BaseModel):
     """Information about a VectorStore."""
 
     vectorstore: VectorStore = Field(exclude=True)
     name: str
     description: str
@@ -27,23 +21,32 @@
         arbitrary_types_allowed = True
 
 
 class VectorStoreToolkit(BaseToolkit):
     """Toolkit for interacting with a Vector Store."""
 
     vectorstore_info: VectorStoreInfo = Field(exclude=True)
-    llm: BaseLanguageModel = Field(default_factory=lambda: OpenAI(temperature=0))
+    llm: BaseLanguageModel
 
     class Config:
         """Configuration for this pydantic object."""
 
         arbitrary_types_allowed = True
 
     def get_tools(self) -> List[BaseTool]:
         """Get the tools in the toolkit."""
+        try:
+            from langchain_community.tools.vectorstore.tool import (
+                VectorStoreQATool,
+                VectorStoreQAWithSourcesTool,
+            )
+        except ImportError:
+            raise ImportError(
+                "You need to install langchain-community to use this toolkit."
+            )
         description = VectorStoreQATool.get_description(
             self.vectorstore_info.name, self.vectorstore_info.description
         )
         qa_tool = VectorStoreQATool(
             name=self.vectorstore_info.name,
             description=description,
             vectorstore=self.vectorstore_info.vectorstore,
@@ -61,24 +64,32 @@
         return [qa_tool, qa_with_sources_tool]
 
 
 class VectorStoreRouterToolkit(BaseToolkit):
     """Toolkit for routing between Vector Stores."""
 
     vectorstores: List[VectorStoreInfo] = Field(exclude=True)
-    llm: BaseLanguageModel = Field(default_factory=lambda: OpenAI(temperature=0))
+    llm: BaseLanguageModel
 
     class Config:
         """Configuration for this pydantic object."""
 
         arbitrary_types_allowed = True
 
     def get_tools(self) -> List[BaseTool]:
         """Get the tools in the toolkit."""
         tools: List[BaseTool] = []
+        try:
+            from langchain_community.tools.vectorstore.tool import (
+                VectorStoreQATool,
+            )
+        except ImportError:
+            raise ImportError(
+                "You need to install langchain-community to use this toolkit."
+            )
         for vectorstore_info in self.vectorstores:
             description = VectorStoreQATool.get_description(
                 vectorstore_info.name, vectorstore_info.description
             )
             qa_tool = VectorStoreQATool(
                 name=vectorstore_info.name,
                 description=description,
```

### Comparing `gigachain-0.1.9/langchain/agents/agent_toolkits/xorbits/__init__.py` & `gigachain-0.2.0/langchain/agents/agent_toolkits/xorbits/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/agent_types.py` & `gigachain-0.2.0/langchain/agents/agent_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Module definitions of agent types together with corresponding agents."""
+
 from enum import Enum
 
 from langchain_core._api import deprecated
 
 
 @deprecated(
     "0.1.0",
     alternative=(
         "Use new agent constructor methods like create_react_agent, create_json_agent, "
         "create_structured_chat_agent, etc."
     ),
-    removal="0.2.0",
+    removal="0.3.0",
 )
 class AgentType(str, Enum):
     """An enum for agent types.
 
     See documentation: https://python.langchain.com/docs/modules/agents/agent_types/
     """
```

### Comparing `gigachain-0.1.9/langchain/agents/chat/base.py` & `gigachain-0.2.0/langchain/agents/chat/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     SYSTEM_MESSAGE_PREFIX,
     SYSTEM_MESSAGE_SUFFIX,
 )
 from langchain.agents.utils import validate_tools_single_input
 from langchain.chains.llm import LLMChain
 
 
-@deprecated("0.1.0", alternative="create_react_agent", removal="0.2.0")
+@deprecated("0.1.0", alternative="create_react_agent", removal="0.3.0")
 class ChatAgent(Agent):
     """Chat Agent."""
 
     output_parser: AgentOutputParser = Field(default_factory=ChatOutputParser)
     """Output parser for the agent."""
 
     @property
@@ -93,15 +93,15 @@
         )
         messages = [
             SystemMessagePromptTemplate.from_template(template),
             HumanMessagePromptTemplate.from_template(human_message),
         ]
         if input_variables is None:
             input_variables = ["input", "agent_scratchpad"]
-        return ChatPromptTemplate(input_variables=input_variables, messages=messages)
+        return ChatPromptTemplate(input_variables=input_variables, messages=messages)  # type: ignore[arg-type]
 
     @classmethod
     def from_llm_and_tools(
         cls,
         llm: BaseLanguageModel,
         tools: Sequence[BaseTool],
         callback_manager: Optional[BaseCallbackManager] = None,
```

### Comparing `gigachain-0.1.9/langchain/agents/chat/output_parser.py` & `gigachain-0.2.0/langchain/agents/chat/output_parser.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/chat/prompt.py` & `gigachain-0.2.0/langchain/agents/chat/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/conversational/base.py` & `gigachain-0.2.0/langchain/agents/conversational/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """An agent designed to hold a conversation in addition to using tools."""
+
 from __future__ import annotations
 
 from typing import Any, List, Optional, Sequence
 
 from langchain_core._api import deprecated
 from langchain_core.callbacks import BaseCallbackManager
 from langchain_core.language_models import BaseLanguageModel
@@ -14,15 +15,15 @@
 from langchain.agents.agent_types import AgentType
 from langchain.agents.conversational.output_parser import ConvoOutputParser
 from langchain.agents.conversational.prompt import FORMAT_INSTRUCTIONS, PREFIX, SUFFIX
 from langchain.agents.utils import validate_tools_single_input
 from langchain.chains import LLMChain
 
 
-@deprecated("0.1.0", alternative="create_react_agent", removal="0.2.0")
+@deprecated("0.1.0", alternative="create_react_agent", removal="0.3.0")
 class ConversationalAgent(Agent):
     """An agent that holds a conversation in addition to using tools."""
 
     ai_prefix: str = "AI"
     """Prefix to use before AI output."""
     output_parser: AgentOutputParser = Field(default_factory=ConvoOutputParser)
     """Output parser for the agent."""
@@ -112,15 +113,15 @@
             ai_prefix=ai_prefix,
             human_prefix=human_prefix,
             prefix=prefix,
             suffix=suffix,
             format_instructions=format_instructions,
             input_variables=input_variables,
         )
-        llm_chain = LLMChain(
+        llm_chain = LLMChain(  # type: ignore[misc]
             llm=llm,
             prompt=prompt,
             callback_manager=callback_manager,
         )
         tool_names = [tool.name for tool in tools]
         _output_parser = output_parser or cls._get_default_output_parser(
             ai_prefix=ai_prefix
```

### Comparing `gigachain-0.1.9/langchain/agents/conversational/output_parser.py` & `gigachain-0.2.0/langchain/agents/conversational/output_parser.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/conversational/prompt.py` & `gigachain-0.2.0/langchain/agents/conversational/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/conversational_chat/base.py` & `gigachain-0.2.0/langchain/agents/conversational_chat/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """An agent designed to hold a conversation in addition to using tools."""
+
 from __future__ import annotations
 
 from typing import Any, List, Optional, Sequence, Tuple
 
 from langchain_core._api import deprecated
 from langchain_core.agents import AgentAction
 from langchain_core.callbacks import BaseCallbackManager
@@ -26,15 +27,15 @@
     SUFFIX,
     TEMPLATE_TOOL_RESPONSE,
 )
 from langchain.agents.utils import validate_tools_single_input
 from langchain.chains import LLMChain
 
 
-@deprecated("0.1.0", alternative="create_json_chat_agent", removal="0.2.0")
+@deprecated("0.1.0", alternative="create_json_chat_agent", removal="0.3.0")
 class ConversationalChatAgent(Agent):
     """An agent designed to hold a conversation in addition to using tools."""
 
     output_parser: AgentOutputParser = Field(default_factory=ConvoOutputParser)
     template_tool_response: str = TEMPLATE_TOOL_RESPONSE
 
     @classmethod
@@ -87,15 +88,15 @@
             input_variables = ["input", "chat_history", "agent_scratchpad"]
         messages = [
             SystemMessagePromptTemplate.from_template(system_message),
             MessagesPlaceholder(variable_name="chat_history"),
             HumanMessagePromptTemplate.from_template(final_prompt),
             MessagesPlaceholder(variable_name="agent_scratchpad"),
         ]
-        return ChatPromptTemplate(input_variables=input_variables, messages=messages)
+        return ChatPromptTemplate(input_variables=input_variables, messages=messages)  # type: ignore[arg-type]
 
     def _construct_scratchpad(
         self, intermediate_steps: List[Tuple[AgentAction, str]]
     ) -> List[BaseMessage]:
         """Construct the scratchpad that lets the agent continue its thought process."""
         thoughts: List[BaseMessage] = []
         for action, observation in intermediate_steps:
@@ -124,15 +125,15 @@
         prompt = cls.create_prompt(
             tools,
             system_message=system_message,
             human_message=human_message,
             input_variables=input_variables,
             output_parser=_output_parser,
         )
-        llm_chain = LLMChain(
+        llm_chain = LLMChain(  # type: ignore[misc]
             llm=llm,
             prompt=prompt,
             callback_manager=callback_manager,
         )
         tool_names = [tool.name for tool in tools]
         return cls(
             llm_chain=llm_chain,
```

### Comparing `gigachain-0.1.9/langchain/agents/conversational_chat/output_parser.py` & `gigachain-0.2.0/langchain/agents/conversational_chat/output_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from typing import Union
 
 from langchain_core.agents import AgentAction, AgentFinish
 from langchain_core.exceptions import OutputParserException
+from langchain_core.utils.json import parse_json_markdown
 
 from langchain.agents import AgentOutputParser
 from langchain.agents.conversational_chat.prompt import FORMAT_INSTRUCTIONS
-from langchain.output_parsers.json import parse_json_markdown
 
 
 # Define a class that parses output for conversational agents
 class ConvoOutputParser(AgentOutputParser):
     """Output parser for the conversational agent."""
 
     format_instructions: str = FORMAT_INSTRUCTIONS
```

### Comparing `gigachain-0.1.9/langchain/agents/conversational_chat/prompt.py` & `gigachain-0.2.0/langchain/agents/conversational_chat/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/format_scratchpad/__init__.py` & `gigachain-0.2.0/langchain/agents/format_scratchpad/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """Logic for formatting intermediate steps into an agent scratchpad.
 
 Intermediate steps refers to the list of (AgentAction, observation) tuples
 that result from previous iterations of the agent.
 Depending on the prompting strategy you are using, you may want to format these
 differently before passing them into the LLM.
 """
+
 from langchain.agents.format_scratchpad.log import format_log_to_str
 from langchain.agents.format_scratchpad.log_to_messages import format_log_to_messages
 from langchain.agents.format_scratchpad.openai_functions import (
     format_to_openai_function_messages,
     format_to_openai_functions,
 )
+from langchain.agents.format_scratchpad.tools import format_to_tool_messages
 from langchain.agents.format_scratchpad.xml import format_xml
 
 __all__ = [
     "format_xml",
     "format_to_openai_function_messages",
     "format_to_openai_functions",
+    "format_to_tool_messages",
     "format_log_to_str",
     "format_log_to_messages",
 ]
```

### Comparing `gigachain-0.1.9/langchain/agents/format_scratchpad/gigachat_functions.py` & `gigachain-0.2.0/langchain/agents/format_scratchpad/gigachat_functions.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/format_scratchpad/gigachat_tools.py` & `gigachain-0.2.0/langchain/agents/format_scratchpad/gigachat_tools.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/format_scratchpad/log.py` & `gigachain-0.2.0/langchain/agents/format_scratchpad/log.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/format_scratchpad/log_to_messages.py` & `gigachain-0.2.0/langchain/agents/format_scratchpad/log_to_messages.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/format_scratchpad/openai_functions.py` & `gigachain-0.2.0/langchain/agents/format_scratchpad/openai_functions.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/format_scratchpad/openai_tools.py` & `gigachain-0.2.0/langchain/agents/format_scratchpad/tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from langchain_core.agents import AgentAction
 from langchain_core.messages import (
     AIMessage,
     BaseMessage,
     ToolMessage,
 )
 
-from langchain.agents.output_parsers.openai_tools import OpenAIToolAgentAction
+from langchain.agents.output_parsers.tools import ToolAgentAction
 
 
 def _create_tool_message(
-    agent_action: OpenAIToolAgentAction, observation: str
+    agent_action: ToolAgentAction, observation: str
 ) -> ToolMessage:
     """Convert agent action and observation into a function message.
     Args:
         agent_action: the tool invocation request from the agent
         observation: the result of the tool invocation
     Returns:
         FunctionMessage that corresponds to the original tool invocation
@@ -31,29 +31,29 @@
     return ToolMessage(
         tool_call_id=agent_action.tool_call_id,
         content=content,
         additional_kwargs={"name": agent_action.tool},
     )
 
 
-def format_to_openai_tool_messages(
+def format_to_tool_messages(
     intermediate_steps: Sequence[Tuple[AgentAction, str]],
 ) -> List[BaseMessage]:
     """Convert (AgentAction, tool output) tuples into FunctionMessages.
 
     Args:
         intermediate_steps: Steps the LLM has taken to date, along with observations
 
     Returns:
         list of messages to send to the LLM for the next prediction
 
     """
     messages = []
     for agent_action, observation in intermediate_steps:
-        if isinstance(agent_action, OpenAIToolAgentAction):
+        if isinstance(agent_action, ToolAgentAction):
             new_messages = list(agent_action.message_log) + [
                 _create_tool_message(agent_action, observation)
             ]
             messages.extend([new for new in new_messages if new not in messages])
         else:
             messages.append(AIMessage(content=agent_action.log))
     return messages
```

### Comparing `gigachain-0.1.9/langchain/agents/format_scratchpad/xml.py` & `gigachain-0.2.0/langchain/agents/format_scratchpad/xml.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/gigachat_functions_agent/agent_token_buffer_memory.py` & `gigachain-0.2.0/langchain/agents/gigachat_functions_agent/agent_token_buffer_memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Memory used to save agent output AND intermediate steps."""
+
 from typing import Any, Dict, List
 
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.messages import BaseMessage, get_buffer_string
 
 from langchain.agents.format_scratchpad.openai_functions import (
     format_to_openai_function_messages,
```

### Comparing `gigachain-0.1.9/langchain/agents/gigachat_functions_agent/base.py` & `gigachain-0.2.0/langchain/agents/gigachat_functions_agent/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Module implements an agent that uses GigaChat's APIs function enabled API."""
+
 from typing import Sequence
 
-from langchain_community.tools.render import format_tool_to_gigachat_function
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.prompts.chat import (
     ChatPromptTemplate,
     HumanMessagePromptTemplate,
     MessagesPlaceholder,
 )
 from langchain_core.runnables import Runnable, RunnablePassthrough
 from langchain_core.tools import BaseTool
+from langchain_core.utils.function_calling import format_tool_to_gigachat_function
 
 from langchain.agents.format_scratchpad.gigachat_functions import (
     format_to_gigachat_function_messages,
 )
 from langchain.agents.output_parsers.gigachat_functions import (
     GigaChatFunctionsAgentOutputParser,
 )
```

### Comparing `gigachain-0.1.9/langchain/agents/gigachat_tools/base.py` & `gigachain-0.2.0/langchain/agents/gigachat_tools/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Sequence
 
-from langchain_community.tools.convert_to_openai import format_tool_to_openai_tool
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.prompts.chat import ChatPromptTemplate
 from langchain_core.runnables import Runnable, RunnablePassthrough
 from langchain_core.tools import BaseTool
+from langchain_core.utils.function_calling import format_tool_to_openai_tool
 
 from langchain.agents.format_scratchpad.openai_tools import (
     format_to_openai_tool_messages,
 )
 from langchain.agents.output_parsers.openai_tools import OpenAIToolsAgentOutputParser
```

### Comparing `gigachain-0.1.9/langchain/agents/initialize.py` & `gigachain-0.2.0/langchain/agents/initialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Load agent."""
+
 from typing import Any, Optional, Sequence
 
 from langchain_core._api import deprecated
 from langchain_core.callbacks import BaseCallbackManager
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.tools import BaseTool
 
@@ -13,15 +14,15 @@
 
 @deprecated(
     "0.1.0",
     alternative=(
         "Use new agent constructor methods like create_react_agent, create_json_agent, "
         "create_structured_chat_agent, etc."
     ),
-    removal="0.2.0",
+    removal="0.3.0",
 )
 def initialize_agent(
     tools: Sequence[BaseTool],
     llm: BaseLanguageModel,
     agent: Optional[AgentType] = None,
     callback_manager: Optional[BaseCallbackManager] = None,
     agent_path: Optional[str] = None,
```

### Comparing `gigachain-0.1.9/langchain/agents/json_chat/base.py` & `gigachain-0.2.0/langchain/agents/json_chat/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,46 @@
-from typing import Sequence
+from typing import List, Sequence, Union
 
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.prompts.chat import ChatPromptTemplate
 from langchain_core.runnables import Runnable, RunnablePassthrough
 from langchain_core.tools import BaseTool
 
 from langchain.agents.format_scratchpad import format_log_to_messages
 from langchain.agents.json_chat.prompt import TEMPLATE_TOOL_RESPONSE
 from langchain.agents.output_parsers import JSONAgentOutputParser
-from langchain.tools.render import render_text_description
+from langchain.tools.render import ToolsRenderer, render_text_description
 
 
 def create_json_chat_agent(
     llm: BaseLanguageModel,
     tools: Sequence[BaseTool],
     prompt: ChatPromptTemplate,
-    stop_sequence: bool = True,
+    stop_sequence: Union[bool, List[str]] = True,
+    tools_renderer: ToolsRenderer = render_text_description,
+    template_tool_response: str = TEMPLATE_TOOL_RESPONSE,
 ) -> Runnable:
     """Create an agent that uses JSON to format its logic, build for Chat Models.
 
     Args:
         llm: LLM to use as the agent.
         tools: Tools this agent has access to.
         prompt: The prompt to use. See Prompt section below for more.
-        stop_sequence: Adds a stop token of "Observation:" to avoid hallucinates. 
+        stop_sequence: bool or list of str.
+            If True, adds a stop token of "Observation:" to avoid hallucinates. 
+            If False, does not add a stop token.
+            If a list of str, uses the provided list as the stop tokens.
+            
             Default is True. You may to set this to False if the LLM you are using
             does not support stop sequences.
+        tools_renderer: This controls how the tools are converted into a string and
+            then passed into the LLM. Default is `render_text_description`.
+        template_tool_response: Template prompt that uses the tool response (observation)
+            to make the LLM generate the next action to take.
+
     Returns:
         A Runnable sequence representing an agent. It takes as input all the same input
         variables as the prompt passed in does. It returns as output either an
         AgentAction or AgentFinish.
 
     Example:
 
@@ -140,32 +151,38 @@
                     MessagesPlaceholder("chat_history", optional=True),
                     ("human", human),
                     MessagesPlaceholder("agent_scratchpad"),
                 ]
             )
     """  # noqa: E501
     missing_vars = {"tools", "tool_names", "agent_scratchpad"}.difference(
-        prompt.input_variables
+        prompt.input_variables + list(prompt.partial_variables)
     )
     if missing_vars:
         raise ValueError(f"Prompt missing required variables: {missing_vars}")
 
+    if "{observation}" not in template_tool_response:
+        raise ValueError(
+            "Template tool response missing required variable 'observation'"
+        )
+
     prompt = prompt.partial(
-        tools=render_text_description(list(tools)),
+        tools=tools_renderer(list(tools)),
         tool_names=", ".join([t.name for t in tools]),
     )
     if stop_sequence:
-        llm_to_use = llm.bind(stop=["\nObservation"])
+        stop = ["\nObservation"] if stop_sequence is True else stop_sequence
+        llm_to_use = llm.bind(stop=stop)
     else:
         llm_to_use = llm
 
     agent = (
         RunnablePassthrough.assign(
             agent_scratchpad=lambda x: format_log_to_messages(
-                x["intermediate_steps"], template_tool_response=TEMPLATE_TOOL_RESPONSE
+                x["intermediate_steps"], template_tool_response=template_tool_response
             )
         )
         | prompt
         | llm_to_use
         | JSONAgentOutputParser()
     )
     return agent
```

### Comparing `gigachain-0.1.9/langchain/agents/json_chat/prompt.py` & `gigachain-0.2.0/langchain/agents/json_chat/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/loading.py` & `gigachain-0.2.0/langchain/agents/loading.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Functionality for loading agents."""
+
 import json
 import logging
 from pathlib import Path
 from typing import Any, List, Optional, Union
 
 import yaml
 from langchain_core._api import deprecated
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.tools import Tool
-from langchain_core.utils.loading import try_load_from_hub
 
 from langchain.agents.agent import BaseMultiActionAgent, BaseSingleActionAgent
 from langchain.agents.types import AGENT_TO_CLASS
 from langchain.chains.loading import load_chain, load_chain_from_config
 
 logger = logging.getLogger(__file__)
 
@@ -27,15 +27,15 @@
         raise ValueError(f"Loading {config_type} agent not supported")
 
     agent_cls = AGENT_TO_CLASS[config_type]
     combined_config = {**config, **kwargs}
     return agent_cls.from_llm_and_tools(llm, tools, **combined_config)
 
 
-@deprecated("0.1.0", removal="0.2.0")
+@deprecated("0.1.0", removal="0.3.0")
 def load_agent_from_config(
     config: dict,
     llm: Optional[BaseLanguageModel] = None,
     tools: Optional[List[Tool]] = None,
     **kwargs: Any,
 ) -> Union[BaseSingleActionAgent, BaseMultiActionAgent]:
     """Load agent from Config Dict.
@@ -83,34 +83,34 @@
         )
         del config["output_parser"]
 
     combined_config = {**config, **kwargs}
     return agent_cls(**combined_config)  # type: ignore
 
 
-@deprecated("0.1.0", removal="0.2.0")
+@deprecated("0.1.0", removal="0.3.0")
 def load_agent(
     path: Union[str, Path], **kwargs: Any
 ) -> Union[BaseSingleActionAgent, BaseMultiActionAgent]:
     """Unified method for loading an agent from LangChainHub or local fs.
 
     Args:
         path: Path to the agent file.
         **kwargs: Additional keyword arguments passed to the agent executor.
 
     Returns:
         An agent executor.
     """
-    valid_suffixes = {"json", "yaml"}
-    if hub_result := try_load_from_hub(
-        path, _load_agent_from_file, "agents", valid_suffixes
-    ):
-        return hub_result
-    else:
-        return _load_agent_from_file(path, **kwargs)
+    if isinstance(path, str) and path.startswith("lc://"):
+        raise RuntimeError(
+            "Loading from the deprecated github-based Hub is no longer supported. "
+            "Please use the new LangChain Hub at https://smith.langchain.com/hub "
+            "instead."
+        )
+    return _load_agent_from_file(path, **kwargs)
 
 
 def _load_agent_from_file(
     file: Union[str, Path], **kwargs: Any
 ) -> Union[BaseSingleActionAgent, BaseMultiActionAgent]:
     """Load agent from file."""
     valid_suffixes = {"json", "yaml"}
```

### Comparing `gigachain-0.1.9/langchain/agents/mrkl/base.py` & `gigachain-0.2.0/langchain/agents/mrkl/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """Attempt to implement MRKL systems as described in arxiv.org/pdf/2205.00445.pdf."""
+
 from __future__ import annotations
 
 from typing import Any, Callable, List, NamedTuple, Optional, Sequence
 
 from langchain_core._api import deprecated
 from langchain_core.callbacks import BaseCallbackManager
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.prompts import PromptTemplate
 from langchain_core.pydantic_v1 import Field
-from langchain_core.tools import BaseTool
+from langchain_core.tools import BaseTool, Tool
 
 from langchain.agents.agent import Agent, AgentExecutor, AgentOutputParser
 from langchain.agents.agent_types import AgentType
 from langchain.agents.mrkl.output_parser import MRKLOutputParser
 from langchain.agents.mrkl.prompt import FORMAT_INSTRUCTIONS, PREFIX, SUFFIX
-from langchain.agents.tools import Tool
 from langchain.agents.utils import validate_tools_single_input
 from langchain.chains import LLMChain
+from langchain.tools.render import render_text_description
 
 
 class ChainConfig(NamedTuple):
     """Configuration for chain to use in MRKL system.
 
     Args:
         action_name: Name of the action.
@@ -29,15 +30,15 @@
     """
 
     action_name: str
     action: Callable
     action_description: str
 
 
-@deprecated("0.1.0", alternative="create_react_agent", removal="0.2.0")
+@deprecated("0.1.0", alternative="create_react_agent", removal="0.3.0")
 class ZeroShotAgent(Agent):
     """Agent for the MRKL chain."""
 
     output_parser: AgentOutputParser = Field(default_factory=MRKLOutputParser)
 
     @classmethod
     def _get_default_output_parser(cls, **kwargs: Any) -> AgentOutputParser:
@@ -75,15 +76,15 @@
             prefix: String to put before the list of tools.
             suffix: String to put after the list of tools.
             input_variables: List of input variables the final prompt will expect.
 
         Returns:
             A PromptTemplate with the template assembled from the pieces here.
         """
-        tool_strings = "\n".join([f"{tool.name}: {tool.description}" for tool in tools])
+        tool_strings = render_text_description(list(tools))
         tool_names = ", ".join([tool.name for tool in tools])
         format_instructions = format_instructions.format(tool_names=tool_names)
         template = "\n\n".join([prefix, tool_strings, format_instructions, suffix])
         if input_variables:
             return PromptTemplate(template=template, input_variables=input_variables)
         return PromptTemplate.from_template(template)
 
@@ -105,15 +106,15 @@
         prompt = cls.create_prompt(
             tools,
             prefix=prefix,
             suffix=suffix,
             format_instructions=format_instructions,
             input_variables=input_variables,
         )
-        llm_chain = LLMChain(
+        llm_chain = LLMChain(  # type: ignore[misc]
             llm=llm,
             prompt=prompt,
             callback_manager=callback_manager,
         )
         tool_names = [tool.name for tool in tools]
         _output_parser = output_parser or cls._get_default_output_parser()
         return cls(
@@ -135,15 +136,15 @@
                 raise ValueError(
                     f"Got a tool {tool.name} without a description. For this agent, "
                     f"a description must always be provided."
                 )
         super()._validate_tools(tools)
 
 
-@deprecated("0.1.0", removal="0.2.0")
+@deprecated("0.1.0", removal="0.3.0")
 class MRKLChain(AgentExecutor):
     """[Deprecated] Chain that implements the MRKL system."""
 
     @classmethod
     def from_chains(
         cls, llm: BaseLanguageModel, chains: List[ChainConfig], **kwargs: Any
     ) -> AgentExecutor:
```

### Comparing `gigachain-0.1.9/langchain/agents/mrkl/output_parser.py` & `gigachain-0.2.0/langchain/agents/mrkl/output_parser.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/mrkl/prompt.py` & `gigachain-0.2.0/langchain/agents/mrkl/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/openai_assistant/base.py` & `gigachain-0.2.0/langchain/agents/openai_assistant/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 from __future__ import annotations
 
 import json
 from json import JSONDecodeError
 from time import sleep
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, Tuple, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
 
 from langchain_core.agents import AgentAction, AgentFinish
 from langchain_core.callbacks import CallbackManager
 from langchain_core.load import dumpd
-from langchain_core.pydantic_v1 import Field, root_validator
+from langchain_core.pydantic_v1 import BaseModel, Field, root_validator
 from langchain_core.runnables import RunnableConfig, RunnableSerializable, ensure_config
 from langchain_core.tools import BaseTool
 from langchain_core.utils.function_calling import convert_to_openai_tool
 
 if TYPE_CHECKING:
     import openai
     from openai.types.beta.threads import ThreadMessage
@@ -72,14 +83,40 @@
     except AttributeError as e:
         raise AttributeError(
             "Please make sure you are using a v1.1-compatible version of openai. You "
             'can install with `pip install "openai>=1.1"`.'
         ) from e
 
 
+def _is_assistants_builtin_tool(
+    tool: Union[Dict[str, Any], Type[BaseModel], Callable, BaseTool],
+) -> bool:
+    """Determine if tool corresponds to OpenAI Assistants built-in."""
+    assistants_builtin_tools = ("code_interpreter", "retrieval")
+    return (
+        isinstance(tool, dict)
+        and ("type" in tool)
+        and (tool["type"] in assistants_builtin_tools)
+    )
+
+
+def _get_assistants_tool(
+    tool: Union[Dict[str, Any], Type[BaseModel], Callable, BaseTool],
+) -> Dict[str, Any]:
+    """Convert a raw function/class to an OpenAI tool.
+
+    Note that OpenAI assistants supports several built-in tools,
+    such as "code_interpreter" and "retrieval."
+    """
+    if _is_assistants_builtin_tool(tool):
+        return tool  # type: ignore
+    else:
+        return convert_to_openai_tool(tool)
+
+
 OutputType = Union[
     List[OpenAIAssistantAction],
     OpenAIAssistantFinish,
     List["ThreadMessage"],
     List["RequiredActionFunctionToolCall"],
 ]
 
@@ -206,16 +243,17 @@
         Returns:
             OpenAIAssistantRunnable configured to run using the created assistant.
         """
         client = client or _get_openai_client()
         assistant = client.beta.assistants.create(
             name=name,
             instructions=instructions,
-            tools=[convert_to_openai_tool(tool) for tool in tools],  # type: ignore
+            tools=[_get_assistants_tool(tool) for tool in tools],  # type: ignore
             model=model,
+            file_ids=kwargs.get("file_ids"),
         )
         return cls(assistant_id=assistant.id, client=client, **kwargs)
 
     def invoke(
         self, input: dict, config: Optional[RunnableConfig] = None
     ) -> OutputType:
         """Invoke assistant.
@@ -323,20 +361,21 @@
             async_client: AsyncOpenAI client.
             Will create default async_client if not specified.
 
         Returns:
             AsyncOpenAIAssistantRunnable configured to run using the created assistant.
         """
         async_client = async_client or _get_openai_async_client()
-        openai_tools = [convert_to_openai_tool(tool) for tool in tools]
+        openai_tools = [_get_assistants_tool(tool) for tool in tools]
         assistant = await async_client.beta.assistants.create(
             name=name,
             instructions=instructions,
             tools=openai_tools,  # type: ignore
             model=model,
+            file_ids=kwargs.get("file_ids"),
         )
         return cls(assistant_id=assistant.id, async_client=async_client, **kwargs)
 
     async def ainvoke(
         self, input: dict, config: Optional[RunnableConfig] = None, **kwargs: Any
     ) -> OutputType:
         """Async invoke assistant.
@@ -391,32 +430,32 @@
                             "content": input["content"],
                             "file_ids": input.get("file_ids", []),
                             "metadata": input.get("message_metadata"),
                         }
                     ],
                     "metadata": input.get("thread_metadata"),
                 }
-                run = await self._create_thread_and_run(input, thread)
+                run = await self._acreate_thread_and_run(input, thread)
             # Starting a new run in an existing thread.
             elif "run_id" not in input:
                 _ = await self.async_client.beta.threads.messages.create(
                     input["thread_id"],
                     content=input["content"],
                     role="user",
                     file_ids=input.get("file_ids", []),
                     metadata=input.get("message_metadata"),
                 )
-                run = await self._create_run(input)
+                run = await self._acreate_run(input)
             # Submitting tool outputs to an existing run, outside the AgentExecutor
             # framework.
             else:
                 run = await self.async_client.beta.threads.runs.submit_tool_outputs(
                     **input
                 )
-            run = await self._wait_for_run(run.id, run.thread_id)
+            run = await self._await_for_run(run.id, run.thread_id)
         except BaseException as e:
             run_manager.on_chain_error(e)
             raise e
         try:
             response = self._get_response(run)
         except BaseException as e:
             run_manager.on_chain_error(e, metadata=run.dict())
@@ -472,25 +511,37 @@
 
     def _get_response(self, run: Any) -> Any:
         # TODO: Pagination
 
         if run.status == "completed":
             import openai
 
+            major_version = int(openai.version.VERSION.split(".")[0])
+            minor_version = int(openai.version.VERSION.split(".")[1])
+            version_gte_1_14 = (major_version > 1) or (
+                major_version == 1 and minor_version >= 14
+            )
+
             messages = self.client.beta.threads.messages.list(
                 run.thread_id, order="asc"
             )
             new_messages = [msg for msg in messages if msg.run_id == run.id]
             if not self.as_agent:
                 return new_messages
             answer: Any = [
                 msg_content for msg in new_messages for msg_content in msg.content
             ]
             if all(
-                isinstance(content, openai.types.beta.threads.MessageContentText)
+                (
+                    isinstance(content, openai.types.beta.threads.TextContentBlock)
+                    if version_gte_1_14
+                    else isinstance(
+                        content, openai.types.beta.threads.MessageContentText
+                    )
+                )
                 for content in answer
             ):
                 answer = "\n".join(content.text.value for content in answer)
             return OpenAIAssistantFinish(
                 return_values={
                     "output": answer,
                     "thread_id": run.thread_id,
@@ -588,25 +639,37 @@
 
     async def _aget_response(self, run: Any) -> Any:
         # TODO: Pagination
 
         if run.status == "completed":
             import openai
 
+            major_version = int(openai.version.VERSION.split(".")[0])
+            minor_version = int(openai.version.VERSION.split(".")[1])
+            version_gte_1_14 = (major_version > 1) or (
+                major_version == 1 and minor_version >= 14
+            )
+
             messages = await self.async_client.beta.threads.messages.list(
                 run.thread_id, order="asc"
             )
             new_messages = [msg for msg in messages if msg.run_id == run.id]
             if not self.as_agent:
                 return new_messages
             answer: Any = [
                 msg_content for msg in new_messages for msg_content in msg.content
             ]
             if all(
-                isinstance(content, openai.types.beta.threads.MessageContentText)
+                (
+                    isinstance(content, openai.types.beta.threads.TextContentBlock)
+                    if version_gte_1_14
+                    else isinstance(
+                        content, openai.types.beta.threads.MessageContentText
+                    )
+                )
                 for content in answer
             ):
                 answer = "\n".join(content.text.value for content in answer)
             return OpenAIAssistantFinish(
                 return_values={
                     "output": answer,
                     "thread_id": run.thread_id,
```

### Comparing `gigachain-0.1.9/langchain/agents/openai_functions_agent/agent_token_buffer_memory.py` & `gigachain-0.2.0/langchain/agents/openai_functions_agent/agent_token_buffer_memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 """Memory used to save agent output AND intermediate steps."""
+
 from typing import Any, Dict, List
 
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.messages import BaseMessage, get_buffer_string
 
-from langchain.agents.format_scratchpad.openai_functions import (
+from langchain.agents.format_scratchpad import (
     format_to_openai_function_messages,
+    format_to_tool_messages,
 )
 from langchain.memory.chat_memory import BaseChatMemory
 
 
 class AgentTokenBufferMemory(BaseChatMemory):
     """Memory used to save agent output AND intermediate steps."""
 
     human_prefix: str = "Human"
     ai_prefix: str = "AI"
     llm: BaseLanguageModel
     memory_key: str = "history"
     max_token_limit: int = 12000
-    """The max number of tokens to keep in the buffer. 
+    """The max number of tokens to keep in the buffer.
     Once the buffer exceeds this many tokens, the oldest messages will be pruned."""
     return_messages: bool = True
     output_key: str = "output"
     intermediate_steps_key: str = "intermediate_steps"
+    format_as_tools: bool = False
 
     @property
     def buffer(self) -> List[BaseMessage]:
         """String buffer of memory."""
         return self.chat_memory.messages
 
     @property
@@ -49,15 +52,20 @@
             )
         return {self.memory_key: final_buffer}
 
     def save_context(self, inputs: Dict[str, Any], outputs: Dict[str, Any]) -> None:
         """Save context from this conversation to buffer. Pruned."""
         input_str, output_str = self._get_input_output(inputs, outputs)
         self.chat_memory.add_user_message(input_str)
-        steps = format_to_openai_function_messages(outputs[self.intermediate_steps_key])
+        format_to_messages = (
+            format_to_tool_messages
+            if self.format_as_tools
+            else format_to_openai_function_messages
+        )
+        steps = format_to_messages(outputs[self.intermediate_steps_key])
         for msg in steps:
             self.chat_memory.add_message(msg)
         self.chat_memory.add_ai_message(output_str)
         # Prune buffer if it exceeds max token limit
         buffer = self.chat_memory.messages
         curr_buffer_length = self.llm.get_num_tokens_from_messages(buffer)
         if curr_buffer_length > self.max_token_limit:
```

### Comparing `gigachain-0.1.9/langchain/agents/openai_functions_agent/base.py` & `gigachain-0.2.0/langchain/agents/openai_functions_agent/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module implements an agent that uses OpenAI's APIs function enabled API."""
+
 from typing import Any, List, Optional, Sequence, Tuple, Type, Union
 
 from langchain_core._api import deprecated
 from langchain_core.agents import AgentAction, AgentFinish
 from langchain_core.callbacks import BaseCallbackManager, Callbacks
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.messages import (
@@ -26,15 +27,15 @@
     format_to_openai_function_messages,
 )
 from langchain.agents.output_parsers.openai_functions import (
     OpenAIFunctionsAgentOutputParser,
 )
 
 
-@deprecated("0.1.0", alternative="create_openai_functions_agent", removal="0.2.0")
+@deprecated("0.1.0", alternative="create_openai_functions_agent", removal="0.3.0")
 class OpenAIFunctionsAgent(BaseSingleActionAgent):
     """An Agent driven by OpenAIs function powered API.
 
     Args:
         llm: This should be an instance of ChatOpenAI, specifically a model
             that supports using `functions`.
         tools: The tools this agent has access to.
@@ -197,15 +198,15 @@
         messages.extend(
             [
                 *_prompts,
                 HumanMessagePromptTemplate.from_template("{input}"),
                 MessagesPlaceholder(variable_name="agent_scratchpad"),
             ]
         )
-        return ChatPromptTemplate(messages=messages)
+        return ChatPromptTemplate(messages=messages)  # type: ignore[arg-type, call-arg]
 
     @classmethod
     def from_llm_and_tools(
         cls,
         llm: BaseLanguageModel,
         tools: Sequence[BaseTool],
         callback_manager: Optional[BaseCallbackManager] = None,
@@ -216,15 +217,15 @@
         **kwargs: Any,
     ) -> BaseSingleActionAgent:
         """Construct an agent from an LLM and tools."""
         prompt = cls.create_prompt(
             extra_prompt_messages=extra_prompt_messages,
             system_message=system_message,
         )
-        return cls(
+        return cls(  # type: ignore[call-arg]
             llm=llm,
             prompt=prompt,
             tools=tools,
             callback_manager=callback_manager,
             **kwargs,
         )
 
@@ -294,15 +295,17 @@
                     ("system", "You are a helpful assistant"),
                     MessagesPlaceholder("chat_history", optional=True),
                     ("human", "{input}"),
                     MessagesPlaceholder("agent_scratchpad"),
                 ]
             )
     """
-    if "agent_scratchpad" not in prompt.input_variables:
+    if "agent_scratchpad" not in (
+        prompt.input_variables + list(prompt.partial_variables)
+    ):
         raise ValueError(
             "Prompt must have input variable `agent_scratchpad`, but wasn't found. "
             f"Found {prompt.input_variables} instead."
         )
     llm_with_tools = llm.bind(functions=[convert_to_openai_function(t) for t in tools])
     agent = (
         RunnablePassthrough.assign(
```

### Comparing `gigachain-0.1.9/langchain/agents/openai_functions_multi_agent/base.py` & `gigachain-0.2.0/langchain/agents/openai_functions_multi_agent/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module implements an agent that uses OpenAI's APIs function enabled API."""
+
 import json
 from json import JSONDecodeError
 from typing import Any, List, Optional, Sequence, Tuple, Union
 
 from langchain_core._api import deprecated
 from langchain_core.agents import AgentAction, AgentActionMessageLog, AgentFinish
 from langchain_core.callbacks import BaseCallbackManager, Callbacks
@@ -89,15 +90,15 @@
         return final_tools
 
     return AgentFinish(
         return_values={"output": message.content}, log=str(message.content)
     )
 
 
-@deprecated("0.1.0", alternative="create_openai_tools_agent", removal="0.2.0")
+@deprecated("0.1.0", alternative="create_openai_tools_agent", removal="0.3.0")
 class OpenAIMultiFunctionsAgent(BaseMultiActionAgent):
     """An Agent driven by OpenAIs function powered API.
 
     Args:
         llm: This should be an instance of ChatOpenAI, specifically a model
             that supports using `functions`.
         tools: The tools this agent has access to.
@@ -275,15 +276,15 @@
         messages.extend(
             [
                 *_prompts,
                 HumanMessagePromptTemplate.from_template("{input}"),
                 MessagesPlaceholder(variable_name="agent_scratchpad"),
             ]
         )
-        return ChatPromptTemplate(messages=messages)
+        return ChatPromptTemplate(messages=messages)  # type: ignore[arg-type, call-arg]
 
     @classmethod
     def from_llm_and_tools(
         cls,
         llm: BaseLanguageModel,
         tools: Sequence[BaseTool],
         callback_manager: Optional[BaseCallbackManager] = None,
@@ -294,14 +295,14 @@
         **kwargs: Any,
     ) -> BaseMultiActionAgent:
         """Construct an agent from an LLM and tools."""
         prompt = cls.create_prompt(
             extra_prompt_messages=extra_prompt_messages,
             system_message=system_message,
         )
-        return cls(
+        return cls(  # type: ignore[call-arg]
             llm=llm,
             prompt=prompt,
             tools=tools,
             callback_manager=callback_manager,
             **kwargs,
         )
```

### Comparing `gigachain-0.1.9/langchain/agents/openai_tools/base.py` & `gigachain-0.2.0/langchain/agents/openai_tools/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,15 +74,17 @@
                     ("system", "You are a helpful assistant"),
                     MessagesPlaceholder("chat_history", optional=True),
                     ("human", "{input}"),
                     MessagesPlaceholder("agent_scratchpad"),
                 ]
             )
     """
-    missing_vars = {"agent_scratchpad"}.difference(prompt.input_variables)
+    missing_vars = {"agent_scratchpad"}.difference(
+        prompt.input_variables + list(prompt.partial_variables)
+    )
     if missing_vars:
         raise ValueError(f"Prompt missing required variables: {missing_vars}")
 
     llm_with_tools = llm.bind(tools=[convert_to_openai_tool(tool) for tool in tools])
 
     agent = (
         RunnablePassthrough.assign(
```

### Comparing `gigachain-0.1.9/langchain/agents/output_parsers/__init__.py` & `gigachain-0.2.0/langchain/agents/output_parsers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,32 +5,35 @@
 and a `log` variable (which contains a log of the agent's thinking).
 
 AgentFinish means that a response should be given.
 This contains a `return_values` dictionary. This usually contains a
 single `output` key, but can be extended to contain more.
 This also contains a `log` variable (which contains a log of the agent's thinking).
 """
+
 from langchain.agents.output_parsers.gigachat_functions import (
     GigaChatFunctionsAgentOutputParser,
 )
 from langchain.agents.output_parsers.json import JSONAgentOutputParser
 from langchain.agents.output_parsers.openai_functions import (
     OpenAIFunctionsAgentOutputParser,
 )
 from langchain.agents.output_parsers.react_json_single_input import (
     ReActJsonSingleInputOutputParser,
 )
 from langchain.agents.output_parsers.react_single_input import (
     ReActSingleInputOutputParser,
 )
 from langchain.agents.output_parsers.self_ask import SelfAskOutputParser
+from langchain.agents.output_parsers.tools import ToolsAgentOutputParser
 from langchain.agents.output_parsers.xml import XMLAgentOutputParser
 
 __all__ = [
     "ReActSingleInputOutputParser",
     "SelfAskOutputParser",
+    "ToolsAgentOutputParser",
     "ReActJsonSingleInputOutputParser",
     "OpenAIFunctionsAgentOutputParser",
     "GigaChatFunctionsAgentOutputParser",
     "XMLAgentOutputParser",
     "JSONAgentOutputParser",
 ]
```

### Comparing `gigachain-0.1.9/langchain/agents/output_parsers/gigachat_functions.py` & `gigachain-0.2.0/langchain/agents/output_parsers/gigachat_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # TODO Don't know why it have linting error
 from typing import List, Union
 
 from langchain_core.agents import AgentAction, AgentActionMessageLog, AgentFinish
 from langchain_core.messages import AIMessage, BaseMessage
 from langchain_core.outputs import ChatGeneration, Generation
 
-from gigachat.models import FunctionCall
+from gigachat.models.function_call import FunctionCall
 from langchain.agents.agent import AgentOutputParser
 
 
 class GigaChatFunctionsAgentOutputParser(AgentOutputParser):
     """Parses a message into agent action/finish.
 
     Is meant to be used with GigaChat models, as it relies on the specific
```

### Comparing `gigachain-0.1.9/langchain/agents/output_parsers/json.py` & `gigachain-0.2.0/langchain/agents/output_parsers/json.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/output_parsers/openai_functions.py` & `gigachain-0.2.0/langchain/agents/output_parsers/openai_functions.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/output_parsers/openai_tools.py` & `gigachain-0.2.0/langchain/agents/output_parsers/tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,93 +3,100 @@
 from typing import List, Union
 
 from langchain_core.agents import AgentAction, AgentActionMessageLog, AgentFinish
 from langchain_core.exceptions import OutputParserException
 from langchain_core.messages import (
     AIMessage,
     BaseMessage,
+    ToolCall,
 )
 from langchain_core.outputs import ChatGeneration, Generation
 
 from langchain.agents.agent import MultiActionAgentOutputParser
 
 
-class OpenAIToolAgentAction(AgentActionMessageLog):
+class ToolAgentAction(AgentActionMessageLog):
     tool_call_id: str
     """Tool call that this message is responding to."""
 
 
-def parse_ai_message_to_openai_tool_action(
+def parse_ai_message_to_tool_action(
     message: BaseMessage,
 ) -> Union[List[AgentAction], AgentFinish]:
     """Parse an AI message potentially containing tool_calls."""
     if not isinstance(message, AIMessage):
         raise TypeError(f"Expected an AI message got {type(message)}")
 
-    if not message.additional_kwargs.get("tool_calls"):
-        return AgentFinish(
-            return_values={"output": message.content}, log=str(message.content)
-        )
-
     actions: List = []
-    for tool_call in message.additional_kwargs["tool_calls"]:
-        function = tool_call["function"]
-        function_name = function["name"]
-        try:
-            _tool_input = json.loads(function["arguments"] or "{}")
-        except JSONDecodeError:
-            raise OutputParserException(
-                f"Could not parse tool input: {function} because "
-                f"the `arguments` is not valid JSON."
+    if message.tool_calls:
+        tool_calls = message.tool_calls
+    else:
+        if not message.additional_kwargs.get("tool_calls"):
+            return AgentFinish(
+                return_values={"output": message.content}, log=str(message.content)
             )
-
+        # Best-effort parsing
+        tool_calls = []
+        for tool_call in message.additional_kwargs["tool_calls"]:
+            function = tool_call["function"]
+            function_name = function["name"]
+            try:
+                args = json.loads(function["arguments"] or "{}")
+                tool_calls.append(
+                    ToolCall(name=function_name, args=args, id=tool_call["id"])
+                )
+            except JSONDecodeError:
+                raise OutputParserException(
+                    f"Could not parse tool input: {function} because "
+                    f"the `arguments` is not valid JSON."
+                )
+    for tool_call in tool_calls:
         # HACK HACK HACK:
         # The code that encodes tool input into Open AI uses a special variable
         # name called `__arg1` to handle old style tools that do not expose a
         # schema and expect a single string argument as an input.
         # We unpack the argument here if it exists.
         # Open AI does not support passing in a JSON array as an argument.
+        function_name = tool_call["name"]
+        _tool_input = tool_call["args"]
         if "__arg1" in _tool_input:
             tool_input = _tool_input["__arg1"]
         else:
             tool_input = _tool_input
 
         content_msg = f"responded: {message.content}\n" if message.content else "\n"
         log = f"\nInvoking: `{function_name}` with `{tool_input}`\n{content_msg}\n"
         actions.append(
-            OpenAIToolAgentAction(
+            ToolAgentAction(
                 tool=function_name,
                 tool_input=tool_input,
                 log=log,
                 message_log=[message],
                 tool_call_id=tool_call["id"],
             )
         )
     return actions
 
 
-class OpenAIToolsAgentOutputParser(MultiActionAgentOutputParser):
+class ToolsAgentOutputParser(MultiActionAgentOutputParser):
     """Parses a message into agent actions/finish.
 
-    Is meant to be used with OpenAI models, as it relies on the specific
-    tool_calls parameter from OpenAI to convey what tools to use.
-
     If a tool_calls parameter is passed, then that is used to get
     the tool names and tool inputs.
 
     If one is not passed, then the AIMessage is assumed to be the final output.
     """
 
     @property
     def _type(self) -> str:
-        return "openai-tools-agent-output-parser"
+        return "tools-agent-output-parser"
 
     def parse_result(
         self, result: List[Generation], *, partial: bool = False
     ) -> Union[List[AgentAction], AgentFinish]:
         if not isinstance(result[0], ChatGeneration):
             raise ValueError("This output parser only works on ChatGeneration output")
         message = result[0].message
-        return parse_ai_message_to_openai_tool_action(message)
+        return parse_ai_message_to_tool_action(message)
 
     def parse(self, text: str) -> Union[List[AgentAction], AgentFinish]:
         raise ValueError("Can only parse messages")
```

### Comparing `gigachain-0.1.9/langchain/agents/output_parsers/react_json_single_input.py` & `gigachain-0.2.0/langchain/agents/output_parsers/react_json_single_input.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/output_parsers/react_single_input.py` & `gigachain-0.2.0/langchain/agents/output_parsers/react_single_input.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/output_parsers/self_ask.py` & `gigachain-0.2.0/langchain/agents/output_parsers/self_ask.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/output_parsers/xml.py` & `gigachain-0.2.0/langchain/agents/output_parsers/xml.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/react/agent.py` & `gigachain-0.2.0/langchain/agents/react/agent.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,47 @@
 from __future__ import annotations
 
-from typing import Sequence
+from typing import List, Optional, Sequence, Union
 
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.prompts import BasePromptTemplate
 from langchain_core.runnables import Runnable, RunnablePassthrough
 from langchain_core.tools import BaseTool
 
+from langchain.agents import AgentOutputParser
 from langchain.agents.format_scratchpad import format_log_to_str
 from langchain.agents.output_parsers import ReActSingleInputOutputParser
-from langchain.tools.render import render_text_description
+from langchain.tools.render import ToolsRenderer, render_text_description
 
 
 def create_react_agent(
-    llm: BaseLanguageModel, tools: Sequence[BaseTool], prompt: BasePromptTemplate
+    llm: BaseLanguageModel,
+    tools: Sequence[BaseTool],
+    prompt: BasePromptTemplate,
+    output_parser: Optional[AgentOutputParser] = None,
+    tools_renderer: ToolsRenderer = render_text_description,
+    *,
+    stop_sequence: Union[bool, List[str]] = True,
 ) -> Runnable:
     """Create an agent that uses ReAct prompting.
 
     Args:
         llm: LLM to use as the agent.
         tools: Tools this agent has access to.
         prompt: The prompt to use. See Prompt section below for more.
+        output_parser: AgentOutputParser for parse the LLM output.
+        tools_renderer: This controls how the tools are converted into a string and
+            then passed into the LLM. Default is `render_text_description`.
+        stop_sequence: bool or list of str.
+            If True, adds a stop token of "Observation:" to avoid hallucinates.
+            If False, does not add a stop token.
+            If a list of str, uses the provided list as the stop tokens.
+
+            Default is True. You may to set this to False if the LLM you are using
+            does not support stop sequences.
 
     Returns:
         A Runnable sequence representing an agent. It takes as input all the same input
         variables as the prompt passed in does. It returns as output either an
         AgentAction or AgentFinish.
 
     Examples:
@@ -87,26 +104,31 @@
 
             Question: {input}
             Thought:{agent_scratchpad}'''
 
             prompt = PromptTemplate.from_template(template)
     """  # noqa: E501
     missing_vars = {"tools", "tool_names", "agent_scratchpad"}.difference(
-        prompt.input_variables
+        prompt.input_variables + list(prompt.partial_variables)
     )
     if missing_vars:
         raise ValueError(f"Prompt missing required variables: {missing_vars}")
 
     prompt = prompt.partial(
-        tools=render_text_description(list(tools)),
+        tools=tools_renderer(list(tools)),
         tool_names=", ".join([t.name for t in tools]),
     )
-    llm_with_stop = llm.bind(stop=["\nObservation"])
+    if stop_sequence:
+        stop = ["\nObservation"] if stop_sequence is True else stop_sequence
+        llm_with_stop = llm.bind(stop=stop)
+    else:
+        llm_with_stop = llm
+    output_parser = output_parser or ReActSingleInputOutputParser()
     agent = (
         RunnablePassthrough.assign(
             agent_scratchpad=lambda x: format_log_to_str(x["intermediate_steps"]),
         )
         | prompt
         | llm_with_stop
-        | ReActSingleInputOutputParser()
+        | output_parser
     )
     return agent
```

### Comparing `gigachain-0.1.9/langchain/agents/react/base.py` & `gigachain-0.2.0/langchain/agents/react/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 """Chain that implements the ReAct paper from https://arxiv.org/pdf/2210.03629.pdf."""
-from typing import Any, List, Optional, Sequence
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Any, List, Optional, Sequence
 
 from langchain_core._api import deprecated
 from langchain_core.documents import Document
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.prompts import BasePromptTemplate
 from langchain_core.pydantic_v1 import Field
 from langchain_core.tools import BaseTool, Tool
 
 from langchain.agents.agent import Agent, AgentExecutor, AgentOutputParser
 from langchain.agents.agent_types import AgentType
 from langchain.agents.react.output_parser import ReActOutputParser
 from langchain.agents.react.textworld_prompt import TEXTWORLD_PROMPT
 from langchain.agents.react.wiki_prompt import WIKI_PROMPT
 from langchain.agents.utils import validate_tools_single_input
-from langchain.docstore.base import Docstore
+
+if TYPE_CHECKING:
+    from langchain_community.docstore.base import Docstore
 
 
-@deprecated("0.1.0", removal="0.2.0")
+@deprecated("0.1.0", removal="0.3.0")
 class ReActDocstoreAgent(Agent):
     """Agent for the ReAct chain."""
 
     output_parser: AgentOutputParser = Field(default_factory=ReActOutputParser)
 
     @classmethod
     def _get_default_output_parser(cls, **kwargs: Any) -> AgentOutputParser:
@@ -60,15 +64,15 @@
 
     @property
     def llm_prefix(self) -> str:
         """Prefix to append the LLM call with."""
         return "Thought:"
 
 
-@deprecated("0.1.0", removal="0.2.0")
+@deprecated("0.1.0", removal="0.3.0")
 class DocstoreExplorer:
     """Class to assist with exploration of a document store."""
 
     def __init__(self, docstore: Docstore):
         """Initialize with a docstore, and set initial document to None."""
         self.docstore = docstore
         self.document: Optional[Document] = None
@@ -110,15 +114,15 @@
     @property
     def _paragraphs(self) -> List[str]:
         if self.document is None:
             raise ValueError("Cannot get paragraphs without a document")
         return self.document.page_content.split("\n\n")
 
 
-@deprecated("0.1.0", removal="0.2.0")
+@deprecated("0.1.0", removal="0.3.0")
 class ReActTextWorldAgent(ReActDocstoreAgent):
     """Agent for the ReAct TextWorld chain."""
 
     @classmethod
     def create_prompt(cls, tools: Sequence[BaseTool]) -> BasePromptTemplate:
         """Return default prompt."""
         return TEXTWORLD_PROMPT
@@ -130,15 +134,15 @@
         if len(tools) != 1:
             raise ValueError(f"Exactly one tool must be specified, but got {tools}")
         tool_names = {tool.name for tool in tools}
         if tool_names != {"Play"}:
             raise ValueError(f"Tool name should be Play, got {tool_names}")
 
 
-@deprecated("0.1.0", removal="0.2.0")
+@deprecated("0.1.0", removal="0.3.0")
 class ReActChain(AgentExecutor):
     """[Deprecated] Chain that implements the ReAct paper."""
 
     def __init__(self, llm: BaseLanguageModel, docstore: Docstore, **kwargs: Any):
         """Initialize with the LLM and a docstore."""
         docstore_explorer = DocstoreExplorer(docstore)
         tools = [
```

### Comparing `gigachain-0.1.9/langchain/agents/react/output_parser.py` & `gigachain-0.2.0/langchain/agents/react/output_parser.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/react/textworld_prompt.py` & `gigachain-0.2.0/langchain/agents/react/textworld_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/react/wiki_prompt.py` & `gigachain-0.2.0/langchain/agents/react/wiki_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/schema.py` & `gigachain-0.2.0/langchain/agents/schema.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/self_ask_with_search/base.py` & `gigachain-0.2.0/langchain/agents/self_ask_with_search/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 """Chain that does self-ask with search."""
-from typing import Any, Sequence, Union
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Any, Sequence, Union
 
-from langchain_community.utilities.google_serper import GoogleSerperAPIWrapper
-from langchain_community.utilities.searchapi import SearchApiAPIWrapper
-from langchain_community.utilities.serpapi import SerpAPIWrapper
 from langchain_core._api import deprecated
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.prompts import BasePromptTemplate
 from langchain_core.pydantic_v1 import Field
 from langchain_core.runnables import Runnable, RunnablePassthrough
 from langchain_core.tools import BaseTool, Tool
 
 from langchain.agents.agent import Agent, AgentExecutor, AgentOutputParser
 from langchain.agents.agent_types import AgentType
 from langchain.agents.format_scratchpad import format_log_to_str
 from langchain.agents.self_ask_with_search.output_parser import SelfAskOutputParser
 from langchain.agents.self_ask_with_search.prompt import PROMPT
 from langchain.agents.utils import validate_tools_single_input
 
+if TYPE_CHECKING:
+    from langchain_community.utilities.google_serper import GoogleSerperAPIWrapper
+    from langchain_community.utilities.searchapi import SearchApiAPIWrapper
+    from langchain_community.utilities.serpapi import SerpAPIWrapper
+
 
-@deprecated("0.1.0", alternative="create_self_ask_with_search", removal="0.2.0")
+@deprecated("0.1.0", alternative="create_self_ask_with_search", removal="0.3.0")
 class SelfAskWithSearchAgent(Agent):
     """Agent for the self-ask-with-search paper."""
 
     output_parser: AgentOutputParser = Field(default_factory=SelfAskOutputParser)
 
     @classmethod
     def _get_default_output_parser(cls, **kwargs: Any) -> AgentOutputParser:
@@ -58,15 +62,15 @@
 
     @property
     def llm_prefix(self) -> str:
         """Prefix to append the LLM call with."""
         return ""
 
 
-@deprecated("0.1.0", removal="0.2.0")
+@deprecated("0.1.0", removal="0.3.0")
 class SelfAskWithSearchChain(AgentExecutor):
     """[Deprecated] Chain that does self-ask with search."""
 
     def __init__(
         self,
         llm: BaseLanguageModel,
         search_chain: Union[
@@ -169,15 +173,17 @@
             So the final answer is: No
 
             Question: {input}
             Are followup questions needed here:{agent_scratchpad}'''
 
             prompt = PromptTemplate.from_template(template)
     """  # noqa: E501
-    missing_vars = {"agent_scratchpad"}.difference(prompt.input_variables)
+    missing_vars = {"agent_scratchpad"}.difference(
+        prompt.input_variables + list(prompt.partial_variables)
+    )
     if missing_vars:
         raise ValueError(f"Prompt missing required variables: {missing_vars}")
 
     if len(tools) != 1:
         raise ValueError("This agent expects exactly one tool")
     tool = list(tools)[0]
     if tool.name != "Intermediate Answer":
```

### Comparing `gigachain-0.1.9/langchain/agents/self_ask_with_search/prompt.py` & `gigachain-0.2.0/langchain/agents/self_ask_with_search/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/structured_chat/base.py` & `gigachain-0.2.0/langchain/agents/structured_chat/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from typing import Any, List, Optional, Sequence, Tuple
+from typing import Any, List, Optional, Sequence, Tuple, Union
 
 from langchain_core._api import deprecated
 from langchain_core.agents import AgentAction
 from langchain_core.callbacks import BaseCallbackManager
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.prompts import BasePromptTemplate
 from langchain_core.prompts.chat import (
@@ -19,20 +19,20 @@
 from langchain.agents.format_scratchpad import format_log_to_str
 from langchain.agents.output_parsers import JSONAgentOutputParser
 from langchain.agents.structured_chat.output_parser import (
     StructuredChatOutputParserWithRetries,
 )
 from langchain.agents.structured_chat.prompt import FORMAT_INSTRUCTIONS, PREFIX, SUFFIX
 from langchain.chains.llm import LLMChain
-from langchain.tools.render import render_text_description_and_args
+from langchain.tools.render import ToolsRenderer, render_text_description_and_args
 
 HUMAN_MESSAGE_TEMPLATE = "{input}\n\n{agent_scratchpad}"
 
 
-@deprecated("0.1.0", alternative="create_structured_chat_agent", removal="0.2.0")
+@deprecated("0.1.0", alternative="create_structured_chat_agent", removal="0.3.0")
 class StructuredChatAgent(Agent):
     """Structured Chat Agent."""
 
     output_parser: AgentOutputParser = Field(
         default_factory=StructuredChatOutputParserWithRetries
     )
     """Output parser for the agent."""
@@ -99,15 +99,15 @@
             input_variables = ["input", "agent_scratchpad"]
         _memory_prompts = memory_prompts or []
         messages = [
             SystemMessagePromptTemplate.from_template(template),
             *_memory_prompts,
             HumanMessagePromptTemplate.from_template(human_message_template),
         ]
-        return ChatPromptTemplate(input_variables=input_variables, messages=messages)
+        return ChatPromptTemplate(input_variables=input_variables, messages=messages)  # type: ignore[arg-type]
 
     @classmethod
     def from_llm_and_tools(
         cls,
         llm: BaseLanguageModel,
         tools: Sequence[BaseTool],
         callback_manager: Optional[BaseCallbackManager] = None,
@@ -147,22 +147,36 @@
 
     @property
     def _agent_type(self) -> str:
         raise ValueError
 
 
 def create_structured_chat_agent(
-    llm: BaseLanguageModel, tools: Sequence[BaseTool], prompt: ChatPromptTemplate
+    llm: BaseLanguageModel,
+    tools: Sequence[BaseTool],
+    prompt: ChatPromptTemplate,
+    tools_renderer: ToolsRenderer = render_text_description_and_args,
+    *,
+    stop_sequence: Union[bool, List[str]] = True,
 ) -> Runnable:
     """Create an agent aimed at supporting tools with multiple inputs.
 
     Args:
         llm: LLM to use as the agent.
         tools: Tools this agent has access to.
         prompt: The prompt to use. See Prompt section below for more.
+        stop_sequence: bool or list of str.
+            If True, adds a stop token of "Observation:" to avoid hallucinates.
+            If False, does not add a stop token.
+            If a list of str, uses the provided list as the stop tokens.
+
+            Default is True. You may to set this to False if the LLM you are using
+            does not support stop sequences.
+        tools_renderer: This controls how the tools are converted into a string and
+            then passed into the LLM. Default is `render_text_description`.
 
     Returns:
         A Runnable sequence representing an agent. It takes as input all the same input
         variables as the prompt passed in does. It returns as output either an
         AgentAction or AgentFinish.
 
     Examples:
@@ -255,24 +269,28 @@
                     ("system", system),
                     MessagesPlaceholder("chat_history", optional=True),
                     ("human", human),
                 ]
             )
     """  # noqa: E501
     missing_vars = {"tools", "tool_names", "agent_scratchpad"}.difference(
-        prompt.input_variables
+        prompt.input_variables + list(prompt.partial_variables)
     )
     if missing_vars:
         raise ValueError(f"Prompt missing required variables: {missing_vars}")
 
     prompt = prompt.partial(
-        tools=render_text_description_and_args(list(tools)),
+        tools=tools_renderer(list(tools)),
         tool_names=", ".join([t.name for t in tools]),
     )
-    llm_with_stop = llm.bind(stop=["Observation"])
+    if stop_sequence:
+        stop = ["\nObservation"] if stop_sequence is True else stop_sequence
+        llm_with_stop = llm.bind(stop=stop)
+    else:
+        llm_with_stop = llm
 
     agent = (
         RunnablePassthrough.assign(
             agent_scratchpad=lambda x: format_log_to_str(x["intermediate_steps"]),
         )
         | prompt
         | llm_with_stop
```

### Comparing `gigachain-0.1.9/langchain/agents/structured_chat/output_parser.py` & `gigachain-0.2.0/langchain/agents/structured_chat/output_parser.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/structured_chat/prompt.py` & `gigachain-0.2.0/langchain/agents/structured_chat/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/tools.py` & `gigachain-0.2.0/langchain/agents/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Interface for tools."""
+
 from typing import List, Optional
 
 from langchain_core.callbacks import (
     AsyncCallbackManagerForToolRun,
     CallbackManagerForToolRun,
 )
 from langchain_core.tools import BaseTool, Tool, tool
```

### Comparing `gigachain-0.1.9/langchain/agents/types.py` & `gigachain-0.2.0/langchain/agents/types.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/agents/xml/base.py` & `gigachain-0.2.0/langchain/agents/xml/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from langchain_core.tools import BaseTool
 
 from langchain.agents.agent import BaseSingleActionAgent
 from langchain.agents.format_scratchpad import format_xml
 from langchain.agents.output_parsers import XMLAgentOutputParser
 from langchain.agents.xml.prompt import agent_instructions
 from langchain.chains.llm import LLMChain
-from langchain.tools.render import render_text_description
+from langchain.tools.render import ToolsRenderer, render_text_description
 
 
-@deprecated("0.1.0", alternative="create_xml_agent", removal="0.2.0")
+@deprecated("0.1.0", alternative="create_xml_agent", removal="0.3.0")
 class XMLAgent(BaseSingleActionAgent):
     """Agent that uses XML tags.
 
     Args:
         tools: list of tools the agent can choose from
         llm_chain: The LLMChain to call to predict the next action
 
@@ -104,24 +104,38 @@
             "stop": ["</tool_input>", "</final_answer>"],
         }
         response = await self.llm_chain.acall(inputs, callbacks=callbacks)
         return response[self.llm_chain.output_key]
 
 
 def create_xml_agent(
-    llm: BaseLanguageModel, tools: Sequence[BaseTool], prompt: BasePromptTemplate
+    llm: BaseLanguageModel,
+    tools: Sequence[BaseTool],
+    prompt: BasePromptTemplate,
+    tools_renderer: ToolsRenderer = render_text_description,
+    *,
+    stop_sequence: Union[bool, List[str]] = True,
 ) -> Runnable:
     """Create an agent that uses XML to format its logic.
 
     Args:
         llm: LLM to use as the agent.
         tools: Tools this agent has access to.
         prompt: The prompt to use, must have input keys
             `tools`: contains descriptions for each tool.
             `agent_scratchpad`: contains previous agent actions and tool outputs.
+        tools_renderer: This controls how the tools are converted into a string and
+            then passed into the LLM. Default is `render_text_description`.
+        stop_sequence: bool or list of str.
+            If True, adds a stop token of "</tool_input>" to avoid hallucinates.
+            If False, does not add a stop token.
+            If a list of str, uses the provided list as the stop tokens.
+
+            Default is True. You may to set this to False if the LLM you are using
+            does not support stop sequences.
 
     Returns:
         A Runnable sequence representing an agent. It takes as input all the same input
         variables as the prompt passed in does. It returns as output either an
         AgentAction or AgentFinish.
 
     Example:
@@ -185,22 +199,29 @@
             Previous Conversation:
             {chat_history}
 
             Question: {input}
             {agent_scratchpad}'''
             prompt = PromptTemplate.from_template(template)
     """  # noqa: E501
-    missing_vars = {"tools", "agent_scratchpad"}.difference(prompt.input_variables)
+    missing_vars = {"tools", "agent_scratchpad"}.difference(
+        prompt.input_variables + list(prompt.partial_variables)
+    )
     if missing_vars:
         raise ValueError(f"Prompt missing required variables: {missing_vars}")
 
     prompt = prompt.partial(
-        tools=render_text_description(list(tools)),
+        tools=tools_renderer(list(tools)),
     )
-    llm_with_stop = llm.bind(stop=["</tool_input>"])
+
+    if stop_sequence:
+        stop = ["</tool_input>"] if stop_sequence is True else stop_sequence
+        llm_with_stop = llm.bind(stop=stop)
+    else:
+        llm_with_stop = llm
 
     agent = (
         RunnablePassthrough.assign(
             agent_scratchpad=lambda x: format_xml(x["intermediate_steps"]),
         )
         | prompt
         | llm_with_stop
```

### Comparing `gigachain-0.1.9/langchain/agents/xml/prompt.py` & `gigachain-0.2.0/langchain/agents/xml/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/callbacks/base.py` & `gigachain-0.2.0/langchain/callbacks/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base callback handler that can be used to handle callbacks in langchain."""
+
 from __future__ import annotations
 
 from langchain_core.callbacks import (
     AsyncCallbackHandler,
     BaseCallbackHandler,
     BaseCallbackManager,
     CallbackManagerMixin,
```

### Comparing `gigachain-0.1.9/langchain/callbacks/manager.py` & `gigachain-0.2.0/langchain/schema/callbacks/manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-from __future__ import annotations
-
-from langchain_community.callbacks.manager import (
-    get_openai_callback,
-    wandb_tracing_enabled,
-)
 from langchain_core.callbacks.manager import (
     AsyncCallbackManager,
     AsyncCallbackManagerForChainGroup,
     AsyncCallbackManagerForChainRun,
     AsyncCallbackManagerForLLMRun,
     AsyncCallbackManagerForRetrieverRun,
     AsyncCallbackManagerForToolRun,
@@ -16,30 +10,33 @@
     BaseRunManager,
     CallbackManager,
     CallbackManagerForChainGroup,
     CallbackManagerForChainRun,
     CallbackManagerForLLMRun,
     CallbackManagerForRetrieverRun,
     CallbackManagerForToolRun,
-    Callbacks,
     ParentRunManager,
     RunManager,
-    ahandle_event,
-    atrace_as_chain_group,
     handle_event,
     trace_as_chain_group,
 )
 from langchain_core.tracers.context import (
     collect_runs,
+    register_configure_hook,
     tracing_enabled,
     tracing_v2_enabled,
 )
 from langchain_core.utils.env import env_var_is_set
 
 __all__ = [
+    "tracing_enabled",
+    "tracing_v2_enabled",
+    "collect_runs",
+    "trace_as_chain_group",
+    "handle_event",
     "BaseRunManager",
     "RunManager",
     "ParentRunManager",
     "AsyncRunManager",
     "AsyncParentRunManager",
     "CallbackManagerForLLMRun",
     "AsyncCallbackManagerForLLMRun",
@@ -49,19 +46,10 @@
     "AsyncCallbackManagerForToolRun",
     "CallbackManagerForRetrieverRun",
     "AsyncCallbackManagerForRetrieverRun",
     "CallbackManager",
     "CallbackManagerForChainGroup",
     "AsyncCallbackManager",
     "AsyncCallbackManagerForChainGroup",
-    "tracing_enabled",
-    "tracing_v2_enabled",
-    "collect_runs",
-    "atrace_as_chain_group",
-    "trace_as_chain_group",
-    "handle_event",
-    "ahandle_event",
-    "Callbacks",
+    "register_configure_hook",
     "env_var_is_set",
-    "get_openai_callback",
-    "wandb_tracing_enabled",
 ]
```

### Comparing `gigachain-0.1.9/langchain/callbacks/streaming_aiter.py` & `gigachain-0.2.0/langchain/callbacks/streaming_aiter.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/callbacks/streaming_aiter_final_only.py` & `gigachain-0.2.0/langchain/callbacks/streaming_aiter_final_only.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/callbacks/streaming_stdout_final_only.py` & `gigachain-0.2.0/langchain/callbacks/streaming_stdout_final_only.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Callback Handler streams to stdout on new llm token."""
+
 import sys
 from typing import Any, Dict, List, Optional
 
 from langchain_core.callbacks import StreamingStdOutCallbackHandler
 
 DEFAULT_ANSWER_PREFIX_TOKENS = ["Final", "Answer", ":"]
```

### Comparing `gigachain-0.1.9/langchain/callbacks/streamlit/__init__.py` & `gigachain-0.2.0/langchain/callbacks/streamlit/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Optional
 
-from langchain.callbacks.base import BaseCallbackHandler
-from langchain.callbacks.streamlit.streamlit_callback_handler import (
-    LLMThoughtLabeler as LLMThoughtLabeler,
-)
-from langchain.callbacks.streamlit.streamlit_callback_handler import (
-    StreamlitCallbackHandler as _InternalStreamlitCallbackHandler,
-)
+from langchain_core.callbacks.base import BaseCallbackHandler
 
 if TYPE_CHECKING:
+    from langchain_community.callbacks import LLMThoughtLabeler
     from streamlit.delta_generator import DeltaGenerator
 
 
 def StreamlitCallbackHandler(
     parent_container: DeltaGenerator,
     *,
     max_thought_containers: int = 4,
@@ -56,26 +51,35 @@
     will be used.
 
     """
     # If we're using a version of Streamlit that implements StreamlitCallbackHandler,
     # delegate to it instead of using our built-in handler. The official handler is
     # guaranteed to support the same set of kwargs.
     try:
-        from streamlit.external.langchain import (
-            StreamlitCallbackHandler as OfficialStreamlitCallbackHandler,  # type: ignore # noqa: 501
-        )
+        from streamlit.external.langchain import StreamlitCallbackHandler
 
-        return OfficialStreamlitCallbackHandler(
+        # This is the official handler, so we can just return it.
+        return StreamlitCallbackHandler(
             parent_container,
             max_thought_containers=max_thought_containers,
             expand_new_thoughts=expand_new_thoughts,
             collapse_completed_thoughts=collapse_completed_thoughts,
             thought_labeler=thought_labeler,
         )
     except ImportError:
+        try:
+            from langchain_community.callbacks.streamlit.streamlit_callback_handler import (  # noqa: E501
+                StreamlitCallbackHandler as _InternalStreamlitCallbackHandler,
+            )
+        except ImportError:
+            raise ImportError(
+                "To use the StreamlitCallbackHandler, please install "
+                "langchain-community with `pip install langchain-community`."
+            )
+
         return _InternalStreamlitCallbackHandler(
             parent_container,
             max_thought_containers=max_thought_containers,
             expand_new_thoughts=expand_new_thoughts,
             collapse_completed_thoughts=collapse_completed_thoughts,
             thought_labeler=thought_labeler,
         )
```

### Comparing `gigachain-0.1.9/langchain/callbacks/tracers/logging.py` & `gigachain-0.2.0/langchain/callbacks/tracers/logging.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/api/base.py` & `gigachain-0.2.0/langchain/chains/api/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Chain that makes API calls and summarizes the responses to answer a question."""
+
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Sequence, Tuple
 from urllib.parse import urlparse
 
-from langchain_community.utilities.requests import TextRequestsWrapper
 from langchain_core.callbacks import (
     AsyncCallbackManagerForChainRun,
     CallbackManagerForChainRun,
 )
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.prompts import BasePromptTemplate
 from langchain_core.pydantic_v1 import Field, root_validator
@@ -46,193 +46,209 @@
     for allowed_domain in limit_to_domains:
         allowed_scheme, allowed_domain = _extract_scheme_and_domain(allowed_domain)
         if scheme == allowed_scheme and domain == allowed_domain:
             return True
     return False
 
 
-class APIChain(Chain):
-    """Chain that makes API calls and summarizes the responses to answer a question.
-
-    *Security Note*: This API chain uses the requests toolkit
-        to make GET, POST, PATCH, PUT, and DELETE requests to an API.
+try:
+    from langchain_community.utilities.requests import TextRequestsWrapper
 
-        Exercise care in who is allowed to use this chain. If exposing
-        to end users, consider that users will be able to make arbitrary
-        requests on behalf of the server hosting the code. For example,
-        users could ask the server to make a request to a private API
-        that is only accessible from the server.
+    class APIChain(Chain):
+        """Chain that makes API calls and summarizes the responses to answer a question.
 
-        Control access to who can submit issue requests using this toolkit and
-        what network access it has.
+        *Security Note*: This API chain uses the requests toolkit
+            to make GET, POST, PATCH, PUT, and DELETE requests to an API.
 
-        See https://python.langchain.com/docs/security for more information.
-    """
+            Exercise care in who is allowed to use this chain. If exposing
+            to end users, consider that users will be able to make arbitrary
+            requests on behalf of the server hosting the code. For example,
+            users could ask the server to make a request to a private API
+            that is only accessible from the server.
 
-    api_request_chain: LLMChain
-    api_answer_chain: LLMChain
-    requests_wrapper: TextRequestsWrapper = Field(exclude=True)
-    api_docs: str
-    question_key: str = "question"  #: :meta private:
-    output_key: str = "output"  #: :meta private:
-    limit_to_domains: Optional[Sequence[str]]
-    """Use to limit the domains that can be accessed by the API chain.
-    
-    * For example, to limit to just the domain `https://www.example.com`, set
-        `limit_to_domains=["https://www.example.com"]`.
-        
-    * The default value is an empty tuple, which means that no domains are
-      allowed by default. By design this will raise an error on instantiation.
-    * Use a None if you want to allow all domains by default -- this is not
-      recommended for security reasons, as it would allow malicious users to
-      make requests to arbitrary URLS including internal APIs accessible from
-      the server.
-    """
+            Control access to who can submit issue requests using this toolkit and
+            what network access it has.
 
-    @property
-    def input_keys(self) -> List[str]:
-        """Expect input key.
-
-        :meta private:
+            See https://python.langchain.com/docs/security for more information.
         """
-        return [self.question_key]
-
-    @property
-    def output_keys(self) -> List[str]:
-        """Expect output key.
 
-        :meta private:
+        api_request_chain: LLMChain
+        api_answer_chain: LLMChain
+        requests_wrapper: TextRequestsWrapper = Field(exclude=True)
+        api_docs: str
+        question_key: str = "question"  #: :meta private:
+        output_key: str = "output"  #: :meta private:
+        limit_to_domains: Optional[Sequence[str]]
+        """Use to limit the domains that can be accessed by the API chain.
+        
+        * For example, to limit to just the domain `https://www.example.com`, set
+            `limit_to_domains=["https://www.example.com"]`.
+            
+        * The default value is an empty tuple, which means that no domains are
+          allowed by default. By design this will raise an error on instantiation.
+        * Use a None if you want to allow all domains by default -- this is not
+          recommended for security reasons, as it would allow malicious users to
+          make requests to arbitrary URLS including internal APIs accessible from
+          the server.
         """
-        return [self.output_key]
 
-    @root_validator(pre=True)
-    def validate_api_request_prompt(cls, values: Dict) -> Dict:
-        """Check that api request prompt expects the right variables."""
-        input_vars = values["api_request_chain"].prompt.input_variables
-        expected_vars = {"question", "api_docs"}
-        if set(input_vars) != expected_vars:
-            raise ValueError(
-                f"Input variables should be {expected_vars}, got {input_vars}"
-            )
-        return values
-
-    @root_validator(pre=True)
-    def validate_limit_to_domains(cls, values: Dict) -> Dict:
-        """Check that allowed domains are valid."""
-        if "limit_to_domains" not in values:
-            raise ValueError(
-                "You must specify a list of domains to limit access using "
-                "`limit_to_domains`"
-            )
-        if not values["limit_to_domains"] and values["limit_to_domains"] is not None:
-            raise ValueError(
-                "Please provide a list of domains to limit access using "
-                "`limit_to_domains`."
-            )
-        return values
-
-    @root_validator(pre=True)
-    def validate_api_answer_prompt(cls, values: Dict) -> Dict:
-        """Check that api answer prompt expects the right variables."""
-        input_vars = values["api_answer_chain"].prompt.input_variables
-        expected_vars = {"question", "api_docs", "api_url", "api_response"}
-        if set(input_vars) != expected_vars:
-            raise ValueError(
-                f"Input variables should be {expected_vars}, got {input_vars}"
-            )
-        return values
-
-    def _call(
-        self,
-        inputs: Dict[str, Any],
-        run_manager: Optional[CallbackManagerForChainRun] = None,
-    ) -> Dict[str, str]:
-        _run_manager = run_manager or CallbackManagerForChainRun.get_noop_manager()
-        question = inputs[self.question_key]
-        api_url = self.api_request_chain.predict(
-            question=question,
-            api_docs=self.api_docs,
-            callbacks=_run_manager.get_child(),
-        )
-        _run_manager.on_text(api_url, color="green", end="\n", verbose=self.verbose)
-        api_url = api_url.strip()
-        if self.limit_to_domains and not _check_in_allowed_domain(
-            api_url, self.limit_to_domains
-        ):
-            raise ValueError(
-                f"{api_url} is not in the allowed domains: {self.limit_to_domains}"
-            )
-        api_response = self.requests_wrapper.get(api_url)
-        _run_manager.on_text(
-            str(api_response), color="yellow", end="\n", verbose=self.verbose
-        )
-        answer = self.api_answer_chain.predict(
-            question=question,
-            api_docs=self.api_docs,
-            api_url=api_url,
-            api_response=api_response,
-            callbacks=_run_manager.get_child(),
-        )
-        return {self.output_key: answer}
-
-    async def _acall(
-        self,
-        inputs: Dict[str, Any],
-        run_manager: Optional[AsyncCallbackManagerForChainRun] = None,
-    ) -> Dict[str, str]:
-        _run_manager = run_manager or AsyncCallbackManagerForChainRun.get_noop_manager()
-        question = inputs[self.question_key]
-        api_url = await self.api_request_chain.apredict(
-            question=question,
-            api_docs=self.api_docs,
-            callbacks=_run_manager.get_child(),
-        )
-        await _run_manager.on_text(
-            api_url, color="green", end="\n", verbose=self.verbose
-        )
-        api_url = api_url.strip()
-        if self.limit_to_domains and not _check_in_allowed_domain(
-            api_url, self.limit_to_domains
-        ):
-            raise ValueError(
-                f"{api_url} is not in the allowed domains: {self.limit_to_domains}"
-            )
-        api_response = await self.requests_wrapper.aget(api_url)
-        await _run_manager.on_text(
-            str(api_response), color="yellow", end="\n", verbose=self.verbose
-        )
-        answer = await self.api_answer_chain.apredict(
-            question=question,
-            api_docs=self.api_docs,
-            api_url=api_url,
-            api_response=api_response,
-            callbacks=_run_manager.get_child(),
-        )
-        return {self.output_key: answer}
-
-    @classmethod
-    def from_llm_and_api_docs(
-        cls,
-        llm: BaseLanguageModel,
-        api_docs: str,
-        headers: Optional[dict] = None,
-        api_url_prompt: BasePromptTemplate = API_URL_PROMPT,
-        api_response_prompt: BasePromptTemplate = API_RESPONSE_PROMPT,
-        limit_to_domains: Optional[Sequence[str]] = tuple(),
-        **kwargs: Any,
-    ) -> APIChain:
-        """Load chain from just an LLM and the api docs."""
-        get_request_chain = LLMChain(llm=llm, prompt=api_url_prompt)
-        requests_wrapper = TextRequestsWrapper(headers=headers)
-        get_answer_chain = LLMChain(llm=llm, prompt=api_response_prompt)
-        return cls(
-            api_request_chain=get_request_chain,
-            api_answer_chain=get_answer_chain,
-            requests_wrapper=requests_wrapper,
-            api_docs=api_docs,
-            limit_to_domains=limit_to_domains,
-            **kwargs,
-        )
-
-    @property
-    def _chain_type(self) -> str:
-        return "api_chain"
+        @property
+        def input_keys(self) -> List[str]:
+            """Expect input key.
+
+            :meta private:
+            """
+            return [self.question_key]
+
+        @property
+        def output_keys(self) -> List[str]:
+            """Expect output key.
+
+            :meta private:
+            """
+            return [self.output_key]
+
+        @root_validator(pre=True)
+        def validate_api_request_prompt(cls, values: Dict) -> Dict:
+            """Check that api request prompt expects the right variables."""
+            input_vars = values["api_request_chain"].prompt.input_variables
+            expected_vars = {"question", "api_docs"}
+            if set(input_vars) != expected_vars:
+                raise ValueError(
+                    f"Input variables should be {expected_vars}, got {input_vars}"
+                )
+            return values
+
+        @root_validator(pre=True)
+        def validate_limit_to_domains(cls, values: Dict) -> Dict:
+            """Check that allowed domains are valid."""
+            if "limit_to_domains" not in values:
+                raise ValueError(
+                    "You must specify a list of domains to limit access using "
+                    "`limit_to_domains`"
+                )
+            if (
+                not values["limit_to_domains"]
+                and values["limit_to_domains"] is not None
+            ):
+                raise ValueError(
+                    "Please provide a list of domains to limit access using "
+                    "`limit_to_domains`."
+                )
+            return values
+
+        @root_validator(pre=True)
+        def validate_api_answer_prompt(cls, values: Dict) -> Dict:
+            """Check that api answer prompt expects the right variables."""
+            input_vars = values["api_answer_chain"].prompt.input_variables
+            expected_vars = {"question", "api_docs", "api_url", "api_response"}
+            if set(input_vars) != expected_vars:
+                raise ValueError(
+                    f"Input variables should be {expected_vars}, got {input_vars}"
+                )
+            return values
+
+        def _call(
+            self,
+            inputs: Dict[str, Any],
+            run_manager: Optional[CallbackManagerForChainRun] = None,
+        ) -> Dict[str, str]:
+            _run_manager = run_manager or CallbackManagerForChainRun.get_noop_manager()
+            question = inputs[self.question_key]
+            api_url = self.api_request_chain.predict(
+                question=question,
+                api_docs=self.api_docs,
+                callbacks=_run_manager.get_child(),
+            )
+            _run_manager.on_text(api_url, color="green", end="\n", verbose=self.verbose)
+            api_url = api_url.strip()
+            if self.limit_to_domains and not _check_in_allowed_domain(
+                api_url, self.limit_to_domains
+            ):
+                raise ValueError(
+                    f"{api_url} is not in the allowed domains: {self.limit_to_domains}"
+                )
+            api_response = self.requests_wrapper.get(api_url)
+            _run_manager.on_text(
+                str(api_response), color="yellow", end="\n", verbose=self.verbose
+            )
+            answer = self.api_answer_chain.predict(
+                question=question,
+                api_docs=self.api_docs,
+                api_url=api_url,
+                api_response=api_response,
+                callbacks=_run_manager.get_child(),
+            )
+            return {self.output_key: answer}
+
+        async def _acall(
+            self,
+            inputs: Dict[str, Any],
+            run_manager: Optional[AsyncCallbackManagerForChainRun] = None,
+        ) -> Dict[str, str]:
+            _run_manager = (
+                run_manager or AsyncCallbackManagerForChainRun.get_noop_manager()
+            )
+            question = inputs[self.question_key]
+            api_url = await self.api_request_chain.apredict(
+                question=question,
+                api_docs=self.api_docs,
+                callbacks=_run_manager.get_child(),
+            )
+            await _run_manager.on_text(
+                api_url, color="green", end="\n", verbose=self.verbose
+            )
+            api_url = api_url.strip()
+            if self.limit_to_domains and not _check_in_allowed_domain(
+                api_url, self.limit_to_domains
+            ):
+                raise ValueError(
+                    f"{api_url} is not in the allowed domains: {self.limit_to_domains}"
+                )
+            api_response = await self.requests_wrapper.aget(api_url)
+            await _run_manager.on_text(
+                str(api_response), color="yellow", end="\n", verbose=self.verbose
+            )
+            answer = await self.api_answer_chain.apredict(
+                question=question,
+                api_docs=self.api_docs,
+                api_url=api_url,
+                api_response=api_response,
+                callbacks=_run_manager.get_child(),
+            )
+            return {self.output_key: answer}
+
+        @classmethod
+        def from_llm_and_api_docs(
+            cls,
+            llm: BaseLanguageModel,
+            api_docs: str,
+            headers: Optional[dict] = None,
+            api_url_prompt: BasePromptTemplate = API_URL_PROMPT,
+            api_response_prompt: BasePromptTemplate = API_RESPONSE_PROMPT,
+            limit_to_domains: Optional[Sequence[str]] = tuple(),
+            **kwargs: Any,
+        ) -> APIChain:
+            """Load chain from just an LLM and the api docs."""
+            get_request_chain = LLMChain(llm=llm, prompt=api_url_prompt)
+            requests_wrapper = TextRequestsWrapper(headers=headers)
+            get_answer_chain = LLMChain(llm=llm, prompt=api_response_prompt)
+            return cls(
+                api_request_chain=get_request_chain,
+                api_answer_chain=get_answer_chain,
+                requests_wrapper=requests_wrapper,
+                api_docs=api_docs,
+                limit_to_domains=limit_to_domains,
+                **kwargs,
+            )
+
+        @property
+        def _chain_type(self) -> str:
+            return "api_chain"
+except ImportError:
+
+    class APIChain:  # type: ignore[no-redef]
+        def __init__(self, *args: Any, **kwargs: Any) -> None:
+            raise ImportError(
+                "To use the APIChain, you must install the langchain_community package."
+                "pip install langchain_community"
+            )
```

### Comparing `gigachain-0.1.9/langchain/chains/api/news_docs.py` & `gigachain-0.2.0/langchain/chains/api/news_docs.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/api/open_meteo_docs.py` & `gigachain-0.2.0/langchain/chains/api/open_meteo_docs.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/api/openapi/chain.py` & `gigachain-0.2.0/langchain/chains/flare/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,229 +1,270 @@
-"""Chain that makes API calls and summarizes the responses to answer a question."""
 from __future__ import annotations
 
-import json
-from typing import Any, Dict, List, NamedTuple, Optional, cast
-
-from langchain_community.tools.openapi.utils.api_models import APIOperation
-from langchain_community.utilities.requests import Requests
-from langchain_core.callbacks import CallbackManagerForChainRun, Callbacks
+import re
+from abc import abstractmethod
+from typing import Any, Dict, List, Optional, Sequence, Tuple
+
+import numpy as np
+from langchain_core.callbacks import (
+    CallbackManagerForChainRun,
+)
 from langchain_core.language_models import BaseLanguageModel
-from langchain_core.pydantic_v1 import BaseModel, Field
-from requests import Response
+from langchain_core.outputs import Generation
+from langchain_core.prompts import BasePromptTemplate
+from langchain_core.pydantic_v1 import Field
+from langchain_core.retrievers import BaseRetriever
 
-from langchain.chains.api.openapi.requests_chain import APIRequesterChain
-from langchain.chains.api.openapi.response_chain import APIResponderChain
 from langchain.chains.base import Chain
+from langchain.chains.flare.prompts import (
+    PROMPT,
+    QUESTION_GENERATOR_PROMPT,
+    FinishedOutputParser,
+)
 from langchain.chains.llm import LLMChain
 
 
-class _ParamMapping(NamedTuple):
-    """Mapping from parameter name to parameter value."""
+class _ResponseChain(LLMChain):
+    """Base class for chains that generate responses."""
+
+    prompt: BasePromptTemplate = PROMPT
 
-    query_params: List[str]
-    body_params: List[str]
-    path_params: List[str]
-
-
-class OpenAPIEndpointChain(Chain, BaseModel):
-    """Chain interacts with an OpenAPI endpoint using natural language."""
-
-    api_request_chain: LLMChain
-    api_response_chain: Optional[LLMChain]
-    api_operation: APIOperation
-    requests: Requests = Field(exclude=True, default_factory=Requests)
-    param_mapping: _ParamMapping = Field(alias="param_mapping")
-    return_intermediate_steps: bool = False
-    instructions_key: str = "instructions"  #: :meta private:
-    output_key: str = "output"  #: :meta private:
-    max_text_length: Optional[int] = Field(ge=0)  #: :meta private:
+    @classmethod
+    def is_lc_serializable(cls) -> bool:
+        return False
 
     @property
     def input_keys(self) -> List[str]:
-        """Expect input key.
+        return self.prompt.input_variables
+
+    def generate_tokens_and_log_probs(
+        self,
+        _input: Dict[str, Any],
+        *,
+        run_manager: Optional[CallbackManagerForChainRun] = None,
+    ) -> Tuple[Sequence[str], Sequence[float]]:
+        llm_result = self.generate([_input], run_manager=run_manager)
+        return self._extract_tokens_and_log_probs(llm_result.generations[0])
+
+    @abstractmethod
+    def _extract_tokens_and_log_probs(
+        self, generations: List[Generation]
+    ) -> Tuple[Sequence[str], Sequence[float]]:
+        """Extract tokens and log probs from response."""
+
+
+class _OpenAIResponseChain(_ResponseChain):
+    """Chain that generates responses from user input and context."""
+
+    llm: BaseLanguageModel
+
+    def _extract_tokens_and_log_probs(
+        self, generations: List[Generation]
+    ) -> Tuple[Sequence[str], Sequence[float]]:
+        tokens = []
+        log_probs = []
+        for gen in generations:
+            if gen.generation_info is None:
+                raise ValueError
+            tokens.extend(gen.generation_info["logprobs"]["tokens"])
+            log_probs.extend(gen.generation_info["logprobs"]["token_logprobs"])
+        return tokens, log_probs
 
-        :meta private:
-        """
-        return [self.instructions_key]
+
+class QuestionGeneratorChain(LLMChain):
+    """Chain that generates questions from uncertain spans."""
+
+    prompt: BasePromptTemplate = QUESTION_GENERATOR_PROMPT
+    """Prompt template for the chain."""
+
+    @classmethod
+    def is_lc_serializable(cls) -> bool:
+        return False
 
     @property
-    def output_keys(self) -> List[str]:
-        """Expect output key.
+    def input_keys(self) -> List[str]:
+        """Input keys for the chain."""
+        return ["user_input", "context", "response"]
 
-        :meta private:
-        """
-        if not self.return_intermediate_steps:
-            return [self.output_key]
+
+def _low_confidence_spans(
+    tokens: Sequence[str],
+    log_probs: Sequence[float],
+    min_prob: float,
+    min_token_gap: int,
+    num_pad_tokens: int,
+) -> List[str]:
+    _low_idx = np.where(np.exp(log_probs) < min_prob)[0]
+    low_idx = [i for i in _low_idx if re.search(r"\w", tokens[i])]
+    if len(low_idx) == 0:
+        return []
+    spans = [[low_idx[0], low_idx[0] + num_pad_tokens + 1]]
+    for i, idx in enumerate(low_idx[1:]):
+        end = idx + num_pad_tokens + 1
+        if idx - low_idx[i] < min_token_gap:
+            spans[-1][1] = end
         else:
-            return [self.output_key, "intermediate_steps"]
+            spans.append([idx, end])
+    return ["".join(tokens[start:end]) for start, end in spans]
 
-    def _construct_path(self, args: Dict[str, str]) -> str:
-        """Construct the path from the deserialized input."""
-        path = self.api_operation.base_url + self.api_operation.path
-        for param in self.param_mapping.path_params:
-            path = path.replace(f"{{{param}}}", str(args.pop(param, "")))
-        return path
-
-    def _extract_query_params(self, args: Dict[str, str]) -> Dict[str, str]:
-        """Extract the query params from the deserialized input."""
-        query_params = {}
-        for param in self.param_mapping.query_params:
-            if param in args:
-                query_params[param] = args.pop(param)
-        return query_params
-
-    def _extract_body_params(self, args: Dict[str, str]) -> Optional[Dict[str, str]]:
-        """Extract the request body params from the deserialized input."""
-        body_params = None
-        if self.param_mapping.body_params:
-            body_params = {}
-            for param in self.param_mapping.body_params:
-                if param in args:
-                    body_params[param] = args.pop(param)
-        return body_params
 
-    def deserialize_json_input(self, serialized_args: str) -> dict:
-        """Use the serialized typescript dictionary.
+class FlareChain(Chain):
+    """Chain that combines a retriever, a question generator,
+    and a response generator."""
+
+    question_generator_chain: QuestionGeneratorChain
+    """Chain that generates questions from uncertain spans."""
+    response_chain: _ResponseChain
+    """Chain that generates responses from user input and context."""
+    output_parser: FinishedOutputParser = Field(default_factory=FinishedOutputParser)
+    """Parser that determines whether the chain is finished."""
+    retriever: BaseRetriever
+    """Retriever that retrieves relevant documents from a user input."""
+    min_prob: float = 0.2
+    """Minimum probability for a token to be considered low confidence."""
+    min_token_gap: int = 5
+    """Minimum number of tokens between two low confidence spans."""
+    num_pad_tokens: int = 2
+    """Number of tokens to pad around a low confidence span."""
+    max_iter: int = 10
+    """Maximum number of iterations."""
+    start_with_retrieval: bool = True
+    """Whether to start with retrieval."""
 
-        Resolve the path, query params dict, and optional requestBody dict.
-        """
-        args: dict = json.loads(serialized_args)
-        path = self._construct_path(args)
-        body_params = self._extract_body_params(args)
-        query_params = self._extract_query_params(args)
-        return {
-            "url": path,
-            "data": body_params,
-            "params": query_params,
-        }
-
-    def _get_output(self, output: str, intermediate_steps: dict) -> dict:
-        """Return the output from the API call."""
-        if self.return_intermediate_steps:
-            return {
-                self.output_key: output,
-                "intermediate_steps": intermediate_steps,
+    @property
+    def input_keys(self) -> List[str]:
+        """Input keys for the chain."""
+        return ["user_input"]
+
+    @property
+    def output_keys(self) -> List[str]:
+        """Output keys for the chain."""
+        return ["response"]
+
+    def _do_generation(
+        self,
+        questions: List[str],
+        user_input: str,
+        response: str,
+        _run_manager: CallbackManagerForChainRun,
+    ) -> Tuple[str, bool]:
+        callbacks = _run_manager.get_child()
+        docs = []
+        for question in questions:
+            docs.extend(self.retriever.invoke(question))
+        context = "\n\n".join(d.page_content for d in docs)
+        result = self.response_chain.predict(
+            user_input=user_input,
+            context=context,
+            response=response,
+            callbacks=callbacks,
+        )
+        marginal, finished = self.output_parser.parse(result)
+        return marginal, finished
+
+    def _do_retrieval(
+        self,
+        low_confidence_spans: List[str],
+        _run_manager: CallbackManagerForChainRun,
+        user_input: str,
+        response: str,
+        initial_response: str,
+    ) -> Tuple[str, bool]:
+        question_gen_inputs = [
+            {
+                "user_input": user_input,
+                "current_response": initial_response,
+                "uncertain_span": span,
             }
-        else:
-            return {self.output_key: output}
+            for span in low_confidence_spans
+        ]
+        callbacks = _run_manager.get_child()
+        question_gen_outputs = self.question_generator_chain.apply(
+            question_gen_inputs, callbacks=callbacks
+        )
+        questions = [
+            output[self.question_generator_chain.output_keys[0]]
+            for output in question_gen_outputs
+        ]
+        _run_manager.on_text(
+            f"Generated Questions: {questions}", color="yellow", end="\n"
+        )
+        return self._do_generation(questions, user_input, response, _run_manager)
 
     def _call(
         self,
         inputs: Dict[str, Any],
         run_manager: Optional[CallbackManagerForChainRun] = None,
-    ) -> Dict[str, str]:
+    ) -> Dict[str, Any]:
         _run_manager = run_manager or CallbackManagerForChainRun.get_noop_manager()
-        intermediate_steps = {}
-        instructions = inputs[self.instructions_key]
-        instructions = instructions[: self.max_text_length]
-        _api_arguments = self.api_request_chain.predict_and_parse(
-            instructions=instructions, callbacks=_run_manager.get_child()
-        )
-        api_arguments = cast(str, _api_arguments)
-        intermediate_steps["request_args"] = api_arguments
-        _run_manager.on_text(
-            api_arguments, color="green", end="\n", verbose=self.verbose
-        )
-        if api_arguments.startswith("ERROR"):
-            return self._get_output(api_arguments, intermediate_steps)
-        elif api_arguments.startswith("MESSAGE:"):
-            return self._get_output(
-                api_arguments[len("MESSAGE:") :], intermediate_steps
+
+        user_input = inputs[self.input_keys[0]]
+
+        response = ""
+
+        for i in range(self.max_iter):
+            _run_manager.on_text(
+                f"Current Response: {response}", color="blue", end="\n"
             )
-        try:
-            request_args = self.deserialize_json_input(api_arguments)
-            method = getattr(self.requests, self.api_operation.method.value)
-            api_response: Response = method(**request_args)
-            if api_response.status_code != 200:
-                method_str = str(self.api_operation.method.value)
-                response_text = (
-                    f"{api_response.status_code}: {api_response.reason}"
-                    + f"\nFor {method_str.upper()}  {request_args['url']}\n"
-                    + f"Called with args: {request_args['params']}"
-                )
-            else:
-                response_text = api_response.text
-        except Exception as e:
-            response_text = f"Error with message {str(e)}"
-        response_text = response_text[: self.max_text_length]
-        intermediate_steps["response_text"] = response_text
-        _run_manager.on_text(
-            response_text, color="blue", end="\n", verbose=self.verbose
-        )
-        if self.api_response_chain is not None:
-            _answer = self.api_response_chain.predict_and_parse(
-                response=response_text,
-                instructions=instructions,
-                callbacks=_run_manager.get_child(),
+            _input = {"user_input": user_input, "context": "", "response": response}
+            tokens, log_probs = self.response_chain.generate_tokens_and_log_probs(
+                _input, run_manager=_run_manager
             )
-            answer = cast(str, _answer)
-            _run_manager.on_text(answer, color="yellow", end="\n", verbose=self.verbose)
-            return self._get_output(answer, intermediate_steps)
-        else:
-            return self._get_output(response_text, intermediate_steps)
+            low_confidence_spans = _low_confidence_spans(
+                tokens,
+                log_probs,
+                self.min_prob,
+                self.min_token_gap,
+                self.num_pad_tokens,
+            )
+            initial_response = response.strip() + " " + "".join(tokens)
+            if not low_confidence_spans:
+                response = initial_response
+                final_response, finished = self.output_parser.parse(response)
+                if finished:
+                    return {self.output_keys[0]: final_response}
+                continue
+
+            marginal, finished = self._do_retrieval(
+                low_confidence_spans,
+                _run_manager,
+                user_input,
+                response,
+                initial_response,
+            )
+            response = response.strip() + " " + marginal
+            if finished:
+                break
+        return {self.output_keys[0]: response}
 
     @classmethod
-    def from_url_and_method(
-        cls,
-        spec_url: str,
-        path: str,
-        method: str,
-        llm: BaseLanguageModel,
-        requests: Optional[Requests] = None,
-        return_intermediate_steps: bool = False,
-        **kwargs: Any,
-        # TODO: Handle async
-    ) -> "OpenAPIEndpointChain":
-        """Create an OpenAPIEndpoint from a spec at the specified url."""
-        operation = APIOperation.from_openapi_url(spec_url, path, method)
-        return cls.from_api_operation(
-            operation,
-            requests=requests,
-            llm=llm,
-            return_intermediate_steps=return_intermediate_steps,
-            **kwargs,
-        )
+    def from_llm(
+        cls, llm: BaseLanguageModel, max_generation_len: int = 32, **kwargs: Any
+    ) -> FlareChain:
+        """Creates a FlareChain from a language model.
+
+        Args:
+            llm: Language model to use.
+            max_generation_len: Maximum length of the generated response.
+            **kwargs: Additional arguments to pass to the constructor.
 
-    @classmethod
-    def from_api_operation(
-        cls,
-        operation: APIOperation,
-        llm: BaseLanguageModel,
-        requests: Optional[Requests] = None,
-        verbose: bool = False,
-        return_intermediate_steps: bool = False,
-        raw_response: bool = False,
-        callbacks: Callbacks = None,
-        **kwargs: Any,
-        # TODO: Handle async
-    ) -> "OpenAPIEndpointChain":
-        """Create an OpenAPIEndpointChain from an operation and a spec."""
-        param_mapping = _ParamMapping(
-            query_params=operation.query_params,
-            body_params=operation.body_params,
-            path_params=operation.path_params,
-        )
-        requests_chain = APIRequesterChain.from_llm_and_typescript(
-            llm,
-            typescript_definition=operation.to_typescript(),
-            verbose=verbose,
-            callbacks=callbacks,
-        )
-        if raw_response:
-            response_chain = None
-        else:
-            response_chain = APIResponderChain.from_llm(
-                llm, verbose=verbose, callbacks=callbacks
+        Returns:
+            FlareChain class with the given language model.
+        """
+        try:
+            from langchain_openai import OpenAI
+        except ImportError:
+            raise ImportError(
+                "OpenAI is required for FlareChain. "
+                "Please install langchain-openai."
+                "pip install langchain-openai"
             )
-        _requests = requests or Requests()
+        question_gen_chain = QuestionGeneratorChain(llm=llm)
+        response_llm = OpenAI(
+            max_tokens=max_generation_len, model_kwargs={"logprobs": 1}, temperature=0
+        )
+        response_chain = _OpenAIResponseChain(llm=response_llm)
         return cls(
-            api_request_chain=requests_chain,
-            api_response_chain=response_chain,
-            api_operation=operation,
-            requests=_requests,
-            param_mapping=param_mapping,
-            verbose=verbose,
-            return_intermediate_steps=return_intermediate_steps,
-            callbacks=callbacks,
+            question_generator_chain=question_gen_chain,
+            response_chain=response_chain,
             **kwargs,
         )
```

### Comparing `gigachain-0.1.9/langchain/chains/api/podcast_docs.py` & `gigachain-0.2.0/langchain/chains/api/podcast_docs.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/api/prompt.py` & `gigachain-0.2.0/langchain/chains/api/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/api/tmdb_docs.py` & `gigachain-0.2.0/langchain/chains/api/tmdb_docs.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/base.py` & `gigachain-0.2.0/langchain/chains/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base interface that all chains should implement."""
+
 import inspect
 import json
 import logging
 import warnings
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Type, Union, cast
@@ -123,14 +124,15 @@
         **kwargs: Any,
     ) -> Dict[str, Any]:
         config = ensure_config(config)
         callbacks = config.get("callbacks")
         tags = config.get("tags")
         metadata = config.get("metadata")
         run_name = config.get("run_name") or self.get_name()
+        run_id = config.get("run_id")
         include_run_info = kwargs.get("include_run_info", False)
         return_only_outputs = kwargs.get("return_only_outputs", False)
 
         inputs = self.prep_inputs(input)
         callback_manager = CallbackManager.configure(
             callbacks,
             self.callbacks,
@@ -141,14 +143,15 @@
             self.metadata,
         )
         new_arg_supported = inspect.signature(self._call).parameters.get("run_manager")
 
         run_manager = callback_manager.on_chain_start(
             dumpd(self),
             inputs,
+            run_id,
             name=run_name,
         )
         try:
             self._validate_inputs(inputs)
             outputs = (
                 self._call(inputs, run_manager=run_manager)
                 if new_arg_supported
@@ -174,41 +177,43 @@
         **kwargs: Any,
     ) -> Dict[str, Any]:
         config = ensure_config(config)
         callbacks = config.get("callbacks")
         tags = config.get("tags")
         metadata = config.get("metadata")
         run_name = config.get("run_name") or self.get_name()
+        run_id = config.get("run_id")
         include_run_info = kwargs.get("include_run_info", False)
         return_only_outputs = kwargs.get("return_only_outputs", False)
 
-        inputs = self.prep_inputs(input)
+        inputs = await self.aprep_inputs(input)
         callback_manager = AsyncCallbackManager.configure(
             callbacks,
             self.callbacks,
             self.verbose,
             tags,
             self.tags,
             metadata,
             self.metadata,
         )
         new_arg_supported = inspect.signature(self._acall).parameters.get("run_manager")
         run_manager = await callback_manager.on_chain_start(
             dumpd(self),
             inputs,
+            run_id,
             name=run_name,
         )
         try:
             self._validate_inputs(inputs)
             outputs = (
                 await self._acall(inputs, run_manager=run_manager)
                 if new_arg_supported
                 else await self._acall(inputs)
             )
-            final_outputs: Dict[str, Any] = self.prep_outputs(
+            final_outputs: Dict[str, Any] = await self.aprep_outputs(
                 inputs, outputs, return_only_outputs
             )
         except BaseException as e:
             await run_manager.on_chain_error(e)
             raise e
         await run_manager.on_chain_end(outputs)
 
@@ -327,15 +332,15 @@
             A dict of named outputs. Should contain all outputs specified in
                 `Chain.output_keys`.
         """
         return await run_in_executor(
             None, self._call, inputs, run_manager.get_sync() if run_manager else None
         )
 
-    @deprecated("0.1.0", alternative="invoke", removal="0.2.0")
+    @deprecated("0.1.0", alternative="invoke", removal="0.3.0")
     def __call__(
         self,
         inputs: Union[Dict[str, Any], Any],
         return_only_outputs: bool = False,
         callbacks: Callbacks = None,
         *,
         tags: Optional[List[str]] = None,
@@ -378,15 +383,15 @@
         return self.invoke(
             inputs,
             cast(RunnableConfig, {k: v for k, v in config.items() if v is not None}),
             return_only_outputs=return_only_outputs,
             include_run_info=include_run_info,
         )
 
-    @deprecated("0.1.0", alternative="ainvoke", removal="0.2.0")
+    @deprecated("0.1.0", alternative="ainvoke", removal="0.3.0")
     async def acall(
         self,
         inputs: Union[Dict[str, Any], Any],
         return_only_outputs: bool = False,
         callbacks: Callbacks = None,
         *,
         tags: Optional[List[str]] = None,
@@ -454,14 +459,40 @@
         if self.memory is not None:
             self.memory.save_context(inputs, outputs)
         if return_only_outputs:
             return outputs
         else:
             return {**inputs, **outputs}
 
+    async def aprep_outputs(
+        self,
+        inputs: Dict[str, str],
+        outputs: Dict[str, str],
+        return_only_outputs: bool = False,
+    ) -> Dict[str, str]:
+        """Validate and prepare chain outputs, and save info about this run to memory.
+
+        Args:
+            inputs: Dictionary of chain inputs, including any inputs added by chain
+                memory.
+            outputs: Dictionary of initial chain outputs.
+            return_only_outputs: Whether to only return the chain outputs. If False,
+                inputs are also added to the final outputs.
+
+        Returns:
+            A dict of the final chain outputs.
+        """
+        self._validate_outputs(outputs)
+        if self.memory is not None:
+            await self.memory.asave_context(inputs, outputs)
+        if return_only_outputs:
+            return outputs
+        else:
+            return {**inputs, **outputs}
+
     def prep_inputs(self, inputs: Union[Dict[str, Any], Any]) -> Dict[str, str]:
         """Prepare chain inputs, including adding inputs from memory.
 
         Args:
             inputs: Dictionary of raw inputs, or single input if chain expects
                 only one param. Should contain all inputs specified in
                 `Chain.input_keys` except for inputs that will be set by the chain's
@@ -478,24 +509,48 @@
                 _input_keys = _input_keys.difference(self.memory.memory_variables)
             inputs = {list(_input_keys)[0]: inputs}
         if self.memory is not None:
             external_context = self.memory.load_memory_variables(inputs)
             inputs = dict(inputs, **external_context)
         return inputs
 
+    async def aprep_inputs(self, inputs: Union[Dict[str, Any], Any]) -> Dict[str, str]:
+        """Prepare chain inputs, including adding inputs from memory.
+
+        Args:
+            inputs: Dictionary of raw inputs, or single input if chain expects
+                only one param. Should contain all inputs specified in
+                `Chain.input_keys` except for inputs that will be set by the chain's
+                memory.
+
+        Returns:
+            A dictionary of all inputs, including those added by the chain's memory.
+        """
+        if not isinstance(inputs, dict):
+            _input_keys = set(self.input_keys)
+            if self.memory is not None:
+                # If there are multiple input keys, but some get set by memory so that
+                # only one is not set, we can still figure out which key it is.
+                _input_keys = _input_keys.difference(self.memory.memory_variables)
+            inputs = {list(_input_keys)[0]: inputs}
+        if self.memory is not None:
+            external_context = await self.memory.aload_memory_variables(inputs)
+            inputs = dict(inputs, **external_context)
+        return inputs
+
     @property
     def _run_output_key(self) -> str:
         if len(self.output_keys) != 1:
             raise ValueError(
                 f"`run` not supported when there is not exactly "
                 f"one output key. Got {self.output_keys}."
             )
         return self.output_keys[0]
 
-    @deprecated("0.1.0", alternative="invoke", removal="0.2.0")
+    @deprecated("0.1.0", alternative="invoke", removal="0.3.0")
     def run(
         self,
         *args: Any,
         callbacks: Callbacks = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
@@ -558,15 +613,15 @@
             )
         else:
             raise ValueError(
                 f"`run` supported with either positional arguments or keyword arguments"
                 f" but not both. Got args: {args} and kwargs: {kwargs}."
             )
 
-    @deprecated("0.1.0", alternative="ainvoke", removal="0.2.0")
+    @deprecated("0.1.0", alternative="ainvoke", removal="0.3.0")
     async def arun(
         self,
         *args: Any,
         callbacks: Callbacks = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
@@ -696,13 +751,13 @@
                 json.dump(chain_dict, f, indent=4)
         elif save_path.suffix.endswith((".yaml", ".yml")):
             with open(file_path, "w", encoding="utf-8") as f:
                 yaml.dump(chain_dict, f, default_flow_style=False)
         else:
             raise ValueError(f"{save_path} must be json or yaml")
 
-    @deprecated("0.1.0", alternative="batch", removal="0.2.0")
+    @deprecated("0.1.0", alternative="batch", removal="0.3.0")
     def apply(
         self, input_list: List[Dict[str, Any]], callbacks: Callbacks = None
     ) -> List[Dict[str, str]]:
         """Call the chain on all inputs in the list."""
         return [self(inputs, callbacks=callbacks) for inputs in input_list]
```

### Comparing `gigachain-0.1.9/langchain/chains/chat_vector_db/prompts.py` & `gigachain-0.2.0/langchain/chains/chat_vector_db/prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/combine_documents/base.py` & `gigachain-0.2.0/langchain/chains/combine_documents/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     CallbackManagerForChainRun,
 )
 from langchain_core.documents import Document
 from langchain_core.prompts import BasePromptTemplate, PromptTemplate
 from langchain_core.pydantic_v1 import BaseModel, Field
 from langchain_core.runnables.config import RunnableConfig
 from langchain_core.runnables.utils import create_model
+from langchain_text_splitters import RecursiveCharacterTextSplitter, TextSplitter
 
 from langchain.chains.base import Chain
-from langchain.text_splitter import RecursiveCharacterTextSplitter, TextSplitter
 
 DEFAULT_DOCUMENT_SEPARATOR = "\n\n"
 DOCUMENTS_KEY = "context"
 DEFAULT_DOCUMENT_PROMPT = PromptTemplate.from_template("{page_content}")
 
 
 def _validate_prompt(prompt: BasePromptTemplate) -> None:
```

### Comparing `gigachain-0.1.9/langchain/chains/combine_documents/conditional.py` & `gigachain-0.2.0/langchain/chains/combine_documents/conditional.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/combine_documents/map_reduce.py` & `gigachain-0.2.0/langchain/chains/combine_documents/map_reduce.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/combine_documents/map_rerank.py` & `gigachain-0.2.0/langchain/chains/combine_documents/map_rerank.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/combine_documents/reduce.py` & `gigachain-0.2.0/langchain/chains/combine_documents/reduce.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/combine_documents/refine.py` & `gigachain-0.2.0/langchain/chains/combine_documents/refine.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/combine_documents/stuff.py` & `gigachain-0.2.0/langchain/chains/combine_documents/stuff.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Chain that combines documents by stuffing into context."""
+
 from typing import Any, Dict, List, Optional, Tuple
 
 from langchain_core.callbacks import Callbacks
 from langchain_core.documents import Document
 from langchain_core.language_models import LanguageModelLike
 from langchain_core.output_parsers import BaseOutputParser, StrOutputParser
 from langchain_core.prompts import BasePromptTemplate, format_document
@@ -56,15 +57,15 @@
             from langchain_core.documents import Document
             from langchain_core.prompts import ChatPromptTemplate
             from langchain.chains.combine_documents import create_stuff_documents_chain
 
             prompt = ChatPromptTemplate.from_messages(
                 [("system", "What are everyone's favorite colors:\\n\\n{context}")]
             )
-            llm = ChatOpenAI(model_name="gpt-3.5-turbo")
+            llm = ChatOpenAI(model="gpt-3.5-turbo")
             chain = create_stuff_documents_chain(llm, prompt)
 
             docs = [
                 Document(page_content="Jesse loves red but not yellow"),
                 Document(page_content = "Jamal loves green but not as much as he loves orange")
             ]
```

### Comparing `gigachain-0.1.9/langchain/chains/constitutional_ai/base.py` & `gigachain-0.2.0/langchain/chains/constitutional_ai/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Chain for applying constitutional principles to the outputs of another chain."""
+
 from typing import Any, Dict, List, Optional
 
 from langchain_core.callbacks import CallbackManagerForChainRun
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.prompts import BasePromptTemplate
 
 from langchain.chains.base import Chain
```

### Comparing `gigachain-0.1.9/langchain/chains/constitutional_ai/principles.py` & `gigachain-0.2.0/langchain/chains/constitutional_ai/principles.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Constitutional principles from https://arxiv.org/pdf/2212.08073.pdf (Bai et al. 2022)
 UnifiedObjectives v0.2 principles ("uo-*") adapted from https://examine.dev/docs/Unified_objectives.pdf (Samwald et al. 2023)
 """
+
 # flake8: noqa
 from typing import Dict
 
 from langchain.chains.constitutional_ai.models import ConstitutionalPrinciple
 
 PRINCIPLES: Dict[str, ConstitutionalPrinciple] = {
     "harmful1": ConstitutionalPrinciple(
```

### Comparing `gigachain-0.1.9/langchain/chains/constitutional_ai/prompts.py` & `gigachain-0.2.0/langchain/chains/constitutional_ai/prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/conversation/base.py` & `gigachain-0.2.0/langchain/chains/conversation/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Chain that carries on a conversation and calls an LLM."""
+
 from typing import Dict, List
 
 from langchain_core.memory import BaseMemory
 from langchain_core.prompts import BasePromptTemplate
 from langchain_core.pydantic_v1 import Extra, Field, root_validator
 
 from langchain.chains.conversation.prompt import PROMPT
```

### Comparing `gigachain-0.1.9/langchain/chains/conversation/memory.py` & `gigachain-0.2.0/langchain/chains/conversation/memory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,40 @@
 """Memory modules for conversation prompts."""
 
+from typing import TYPE_CHECKING, Any
+
+from langchain._api import create_importer
 from langchain.memory.buffer import (
     ConversationBufferMemory,
     ConversationStringBufferMemory,
 )
 from langchain.memory.buffer_window import ConversationBufferWindowMemory
 from langchain.memory.combined import CombinedMemory
 from langchain.memory.entity import ConversationEntityMemory
-from langchain.memory.kg import ConversationKGMemory
 from langchain.memory.summary import ConversationSummaryMemory
 from langchain.memory.summary_buffer import ConversationSummaryBufferMemory
 
+if TYPE_CHECKING:
+    from langchain_community.memory.kg import ConversationKGMemory
+
+# Create a way to dynamically look up deprecated imports.
+# Used to consolidate logic for raising deprecation warnings and
+# handling optional imports.
+DEPRECATED_LOOKUP = {
+    "ConversationKGMemory": "langchain_community.memory.kg",
+}
+
+_importer = create_importer(__package__, deprecated_lookups=DEPRECATED_LOOKUP)
+
+
+def __getattr__(name: str) -> Any:
+    """Look up attributes dynamically."""
+    return _importer(name)
+
+
 # This is only for backwards compatibility.
 
 __all__ = [
     "ConversationSummaryBufferMemory",
     "ConversationSummaryMemory",
     "ConversationKGMemory",
     "ConversationBufferWindowMemory",
```

### Comparing `gigachain-0.1.9/langchain/chains/conversation/prompt.py` & `gigachain-0.2.0/langchain/chains/conversation/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/conversational_retrieval/base.py` & `gigachain-0.2.0/langchain/chains/conversational_retrieval/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Chain for chatting with a vector database."""
+
 from __future__ import annotations
 
 import inspect
 import warnings
 from abc import abstractmethod
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
 
+from langchain_core._api import deprecated
 from langchain_core.callbacks import (
     AsyncCallbackManagerForChainRun,
     CallbackManagerForChainRun,
     Callbacks,
 )
 from langchain_core.documents import Document
 from langchain_core.language_models import BaseLanguageModel
@@ -231,17 +233,92 @@
 
     def save(self, file_path: Union[Path, str]) -> None:
         if self.get_chat_history:
             raise ValueError("Chain not saveable when `get_chat_history` is not None.")
         super().save(file_path)
 
 
+@deprecated(
+    since="0.1.17",
+    alternative=(
+        "create_history_aware_retriever together with create_retrieval_chain "
+        "(see example in docstring)"
+    ),
+    removal="0.3.0",
+)
 class ConversationalRetrievalChain(BaseConversationalRetrievalChain):
     """Chain for having a conversation based on retrieved documents.
 
+    This class is deprecated. See below for an example implementation using
+    `create_retrieval_chain`. Additional walkthroughs can be found at
+    https://python.langchain.com/docs/use_cases/question_answering/chat_history
+
+        .. code-block:: python
+
+            from langchain.chains import (
+                create_history_aware_retriever,
+                create_retrieval_chain,
+            )
+            from langchain.chains.combine_documents import create_stuff_documents_chain
+            from langchain_core.prompts import ChatPromptTemplate, MessagesPlaceholder
+            from langchain_openai import ChatOpenAI
+
+
+            retriever = ...  # Your retriever
+
+            llm = ChatOpenAI()
+
+            # Contextualize question
+            contextualize_q_system_prompt = (
+                "Given a chat history and the latest user question "
+                "which might reference context in the chat history, "
+                "formulate a standalone question which can be understood "
+                "without the chat history. Do NOT answer the question, just "
+                "reformulate it if needed and otherwise return it as is."
+            )
+            contextualize_q_prompt = ChatPromptTemplate.from_messages(
+                [
+                    ("system", contextualize_q_system_prompt),
+                    MessagesPlaceholder("chat_history"),
+                    ("human", "{input}"),
+                ]
+            )
+            history_aware_retriever = create_history_aware_retriever(
+                llm, retriever, contextualize_q_prompt
+            )
+
+            # Answer question
+            qa_system_prompt = (
+                "You are an assistant for question-answering tasks. Use "
+                "the following pieces of retrieved context to answer the "
+                "question. If you don't know the answer, just say that you "
+                "don't know. Use three sentences maximum and keep the answer "
+                "concise."
+                "\n\n"
+                "{context}"
+            )
+            qa_prompt = ChatPromptTemplate.from_messages(
+                [
+                    ("system", qa_system_prompt),
+                    MessagesPlaceholder("chat_history"),
+                    ("human", "{input}"),
+                ]
+            )
+            # Below we use create_stuff_documents_chain to feed all retrieved context
+            # into the LLM. Note that we can also use StuffDocumentsChain and other
+            # instances of BaseCombineDocumentsChain.
+            question_answer_chain = create_stuff_documents_chain(llm, qa_prompt)
+            rag_chain = create_retrieval_chain(
+                history_aware_retriever, question_answer_chain
+            )
+
+            # Usage:
+            chat_history = []  # Collect chat history here (a sequence of messages)
+            rag_chain.invoke({"input": query, "chat_history": chat_history})
+
     This chain takes in chat history (a list of messages) and new questions,
     and then returns an answer to that question.
     The algorithm for this chain consists of three parts:
 
     1. Use the chat history and the new question to create a "standalone question".
     This is done so that this question can be passed into the retrieval step to fetch
     relevant documents. If only the new question was passed in, then relevant context
@@ -312,29 +389,29 @@
         self,
         question: str,
         inputs: Dict[str, Any],
         *,
         run_manager: CallbackManagerForChainRun,
     ) -> List[Document]:
         """Get docs."""
-        docs = self.retriever.get_relevant_documents(
-            question, callbacks=run_manager.get_child()
+        docs = self.retriever.invoke(
+            question, config={"callbacks": run_manager.get_child()}
         )
         return self._reduce_tokens_below_limit(docs)
 
     async def _aget_docs(
         self,
         question: str,
         inputs: Dict[str, Any],
         *,
         run_manager: AsyncCallbackManagerForChainRun,
     ) -> List[Document]:
         """Get docs."""
-        docs = await self.retriever.aget_relevant_documents(
-            question, callbacks=run_manager.get_child()
+        docs = await self.retriever.ainvoke(
+            question, config={"callbacks": run_manager.get_child()}
         )
         return self._reduce_tokens_below_limit(docs)
 
     @classmethod
     def from_llm(
         cls,
         llm: BaseLanguageModel,
```

### Comparing `gigachain-0.1.9/langchain/chains/conversational_retrieval/prompts.py` & `gigachain-0.2.0/langchain/chains/conversational_retrieval/prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/elasticsearch_database/base.py` & `gigachain-0.2.0/langchain/chains/elasticsearch_database/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Chain for interacting with Elasticsearch Database."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 from langchain_core.callbacks import CallbackManagerForChainRun
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.output_parsers import BaseLLMOutputParser
```

### Comparing `gigachain-0.1.9/langchain/chains/elasticsearch_database/prompts.py` & `gigachain-0.2.0/langchain/chains/elasticsearch_database/prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/encoder.py` & `gigachain-0.2.0/langchain/chains/encoder.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/example_generator.py` & `gigachain-0.2.0/langchain/chains/example_generator.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/flare/base.py` & `gigachain-0.2.0/langchain/chains/retrieval_qa/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,267 +1,336 @@
+"""Chain for question-answering against a vector database."""
+
 from __future__ import annotations
 
-import re
+import inspect
+import warnings
 from abc import abstractmethod
-from typing import Any, Dict, List, Optional, Sequence, Tuple
+from typing import Any, Dict, List, Optional
 
-import numpy as np
-from langchain_community.llms.openai import OpenAI
+from langchain_core._api import deprecated
 from langchain_core.callbacks import (
+    AsyncCallbackManagerForChainRun,
     CallbackManagerForChainRun,
+    Callbacks,
 )
+from langchain_core.documents import Document
 from langchain_core.language_models import BaseLanguageModel
-from langchain_core.outputs import Generation
-from langchain_core.prompts import BasePromptTemplate
-from langchain_core.pydantic_v1 import Field
+from langchain_core.prompts import PromptTemplate
+from langchain_core.pydantic_v1 import Extra, Field, root_validator
 from langchain_core.retrievers import BaseRetriever
+from langchain_core.vectorstores import VectorStore
 
 from langchain.chains.base import Chain
-from langchain.chains.flare.prompts import (
-    PROMPT,
-    QUESTION_GENERATOR_PROMPT,
-    FinishedOutputParser,
-)
+from langchain.chains.combine_documents.base import BaseCombineDocumentsChain
+from langchain.chains.combine_documents.stuff import StuffDocumentsChain
 from langchain.chains.llm import LLMChain
+from langchain.chains.question_answering import load_qa_chain
+from langchain.chains.question_answering.stuff_prompt import PROMPT_SELECTOR
 
 
-class _ResponseChain(LLMChain):
-    """Base class for chains that generate responses."""
-
-    prompt: BasePromptTemplate = PROMPT
+class BaseRetrievalQA(Chain):
+    """Base class for question-answering chains."""
 
-    @classmethod
-    def is_lc_serializable(cls) -> bool:
-        return False
+    combine_documents_chain: BaseCombineDocumentsChain
+    """Chain to use to combine the documents."""
+    input_key: str = "query"  #: :meta private:
+    output_key: str = "result"  #: :meta private:
+    return_source_documents: bool = False
+    """Return the source documents or not."""
+
+    class Config:
+        """Configuration for this pydantic object."""
+
+        extra = Extra.forbid
+        arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def input_keys(self) -> List[str]:
-        return self.prompt.input_variables
+        """Input keys.
+
+        :meta private:
+        """
+        return [self.input_key]
+
+    @property
+    def output_keys(self) -> List[str]:
+        """Output keys.
+
+        :meta private:
+        """
+        _output_keys = [self.output_key]
+        if self.return_source_documents:
+            _output_keys = _output_keys + ["source_documents"]
+        return _output_keys
+
+    @classmethod
+    def from_llm(
+        cls,
+        llm: BaseLanguageModel,
+        prompt: Optional[PromptTemplate] = None,
+        callbacks: Callbacks = None,
+        llm_chain_kwargs: Optional[dict] = None,
+        **kwargs: Any,
+    ) -> BaseRetrievalQA:
+        """Initialize from LLM."""
+        _prompt = prompt or PROMPT_SELECTOR.get_prompt(llm)
+        llm_chain = LLMChain(
+            llm=llm, prompt=_prompt, callbacks=callbacks, **(llm_chain_kwargs or {})
+        )
+        document_prompt = PromptTemplate(
+            input_variables=["page_content"], template="Context:\n{page_content}"
+        )
+        combine_documents_chain = StuffDocumentsChain(
+            llm_chain=llm_chain,
+            document_variable_name="context",
+            document_prompt=document_prompt,
+            callbacks=callbacks,
+        )
+
+        return cls(
+            combine_documents_chain=combine_documents_chain,
+            callbacks=callbacks,
+            **kwargs,
+        )
+
+    @classmethod
+    def from_chain_type(
+        cls,
+        llm: BaseLanguageModel,
+        chain_type: str = "stuff",
+        chain_type_kwargs: Optional[dict] = None,
+        **kwargs: Any,
+    ) -> BaseRetrievalQA:
+        """Load chain from chain type."""
+        _chain_type_kwargs = chain_type_kwargs or {}
+        combine_documents_chain = load_qa_chain(
+            llm, chain_type=chain_type, **_chain_type_kwargs
+        )
+        return cls(combine_documents_chain=combine_documents_chain, **kwargs)
 
-    def generate_tokens_and_log_probs(
+    @abstractmethod
+    def _get_docs(
         self,
-        _input: Dict[str, Any],
+        question: str,
         *,
+        run_manager: CallbackManagerForChainRun,
+    ) -> List[Document]:
+        """Get documents to do question answering over."""
+
+    def _call(
+        self,
+        inputs: Dict[str, Any],
         run_manager: Optional[CallbackManagerForChainRun] = None,
-    ) -> Tuple[Sequence[str], Sequence[float]]:
-        llm_result = self.generate([_input], run_manager=run_manager)
-        return self._extract_tokens_and_log_probs(llm_result.generations[0])
+    ) -> Dict[str, Any]:
+        """Run get_relevant_text and llm on input query.
 
-    @abstractmethod
-    def _extract_tokens_and_log_probs(
-        self, generations: List[Generation]
-    ) -> Tuple[Sequence[str], Sequence[float]]:
-        """Extract tokens and log probs from response."""
-
-
-class _OpenAIResponseChain(_ResponseChain):
-    """Chain that generates responses from user input and context."""
-
-    llm: OpenAI = Field(
-        default_factory=lambda: OpenAI(
-            max_tokens=32, model_kwargs={"logprobs": 1}, temperature=0
-        )
-    )
-
-    def _extract_tokens_and_log_probs(
-        self, generations: List[Generation]
-    ) -> Tuple[Sequence[str], Sequence[float]]:
-        tokens = []
-        log_probs = []
-        for gen in generations:
-            if gen.generation_info is None:
-                raise ValueError
-            tokens.extend(gen.generation_info["logprobs"]["tokens"])
-            log_probs.extend(gen.generation_info["logprobs"]["token_logprobs"])
-        return tokens, log_probs
+        If chain has 'return_source_documents' as 'True', returns
+        the retrieved documents as well under the key 'source_documents'.
 
+        Example:
+        .. code-block:: python
 
-class QuestionGeneratorChain(LLMChain):
-    """Chain that generates questions from uncertain spans."""
+        res = indexqa({'query': 'This is my query'})
+        answer, docs = res['result'], res['source_documents']
+        """
+        _run_manager = run_manager or CallbackManagerForChainRun.get_noop_manager()
+        question = inputs[self.input_key]
+        accepts_run_manager = (
+            "run_manager" in inspect.signature(self._get_docs).parameters
+        )
+        if accepts_run_manager:
+            docs = self._get_docs(question, run_manager=_run_manager)
+        else:
+            docs = self._get_docs(question)  # type: ignore[call-arg]
+        answer = self.combine_documents_chain.run(
+            input_documents=docs, question=question, callbacks=_run_manager.get_child()
+        )
 
-    prompt: BasePromptTemplate = QUESTION_GENERATOR_PROMPT
-    """Prompt template for the chain."""
+        if self.return_source_documents:
+            return {self.output_key: answer, "source_documents": docs}
+        else:
+            return {self.output_key: answer}
 
-    @classmethod
-    def is_lc_serializable(cls) -> bool:
-        return False
+    @abstractmethod
+    async def _aget_docs(
+        self,
+        question: str,
+        *,
+        run_manager: AsyncCallbackManagerForChainRun,
+    ) -> List[Document]:
+        """Get documents to do question answering over."""
 
-    @property
-    def input_keys(self) -> List[str]:
-        """Input keys for the chain."""
-        return ["user_input", "context", "response"]
+    async def _acall(
+        self,
+        inputs: Dict[str, Any],
+        run_manager: Optional[AsyncCallbackManagerForChainRun] = None,
+    ) -> Dict[str, Any]:
+        """Run get_relevant_text and llm on input query.
 
+        If chain has 'return_source_documents' as 'True', returns
+        the retrieved documents as well under the key 'source_documents'.
 
-def _low_confidence_spans(
-    tokens: Sequence[str],
-    log_probs: Sequence[float],
-    min_prob: float,
-    min_token_gap: int,
-    num_pad_tokens: int,
-) -> List[str]:
-    _low_idx = np.where(np.exp(log_probs) < min_prob)[0]
-    low_idx = [i for i in _low_idx if re.search(r"\w", tokens[i])]
-    if len(low_idx) == 0:
-        return []
-    spans = [[low_idx[0], low_idx[0] + num_pad_tokens + 1]]
-    for i, idx in enumerate(low_idx[1:]):
-        end = idx + num_pad_tokens + 1
-        if idx - low_idx[i] < min_token_gap:
-            spans[-1][1] = end
+        Example:
+        .. code-block:: python
+
+        res = indexqa({'query': 'This is my query'})
+        answer, docs = res['result'], res['source_documents']
+        """
+        _run_manager = run_manager or AsyncCallbackManagerForChainRun.get_noop_manager()
+        question = inputs[self.input_key]
+        accepts_run_manager = (
+            "run_manager" in inspect.signature(self._aget_docs).parameters
+        )
+        if accepts_run_manager:
+            docs = await self._aget_docs(question, run_manager=_run_manager)
         else:
-            spans.append([idx, end])
-    return ["".join(tokens[start:end]) for start, end in spans]
+            docs = await self._aget_docs(question)  # type: ignore[call-arg]
+        answer = await self.combine_documents_chain.arun(
+            input_documents=docs, question=question, callbacks=_run_manager.get_child()
+        )
 
+        if self.return_source_documents:
+            return {self.output_key: answer, "source_documents": docs}
+        else:
+            return {self.output_key: answer}
 
-class FlareChain(Chain):
-    """Chain that combines a retriever, a question generator,
-    and a response generator."""
-
-    question_generator_chain: QuestionGeneratorChain
-    """Chain that generates questions from uncertain spans."""
-    response_chain: _ResponseChain = Field(default_factory=_OpenAIResponseChain)
-    """Chain that generates responses from user input and context."""
-    output_parser: FinishedOutputParser = Field(default_factory=FinishedOutputParser)
-    """Parser that determines whether the chain is finished."""
-    retriever: BaseRetriever
-    """Retriever that retrieves relevant documents from a user input."""
-    min_prob: float = 0.2
-    """Minimum probability for a token to be considered low confidence."""
-    min_token_gap: int = 5
-    """Minimum number of tokens between two low confidence spans."""
-    num_pad_tokens: int = 2
-    """Number of tokens to pad around a low confidence span."""
-    max_iter: int = 10
-    """Maximum number of iterations."""
-    start_with_retrieval: bool = True
-    """Whether to start with retrieval."""
 
-    @property
-    def input_keys(self) -> List[str]:
-        """Input keys for the chain."""
-        return ["user_input"]
+@deprecated(since="0.1.17", alternative="create_retrieval_chain", removal="0.3.0")
+class RetrievalQA(BaseRetrievalQA):
+    """Chain for question-answering against an index.
 
-    @property
-    def output_keys(self) -> List[str]:
-        """Output keys for the chain."""
-        return ["response"]
+    This class is deprecated. See below for an example implementation using
+    `create_retrieval_chain`:
 
-    def _do_generation(
-        self,
-        questions: List[str],
-        user_input: str,
-        response: str,
-        _run_manager: CallbackManagerForChainRun,
-    ) -> Tuple[str, bool]:
-        callbacks = _run_manager.get_child()
-        docs = []
-        for question in questions:
-            docs.extend(self.retriever.get_relevant_documents(question))
-        context = "\n\n".join(d.page_content for d in docs)
-        result = self.response_chain.predict(
-            user_input=user_input,
-            context=context,
-            response=response,
-            callbacks=callbacks,
-        )
-        marginal, finished = self.output_parser.parse(result)
-        return marginal, finished
+        .. code-block:: python
 
-    def _do_retrieval(
+            from langchain.chains import create_retrieval_chain
+            from langchain.chains.combine_documents import create_stuff_documents_chain
+            from langchain_core.prompts import ChatPromptTemplate
+            from langchain_openai import ChatOpenAI
+
+
+            retriever = ...  # Your retriever
+            llm = ChatOpenAI()
+
+            system_prompt = (
+                "Use the given context to answer the question. "
+                "If you don't know the answer, say you don't know. "
+                "Use three sentence maximum and keep the answer concise. "
+                "Context: {context}"
+            )
+            prompt = ChatPromptTemplate.from_messages(
+                [
+                    ("system", system_prompt),
+                    ("human", "{input}"),
+                ]
+            )
+            question_answer_chain = create_stuff_documents_chain(llm, prompt)
+            chain = create_retrieval_chain(retriever, question_answer_chain)
+
+            chain.invoke({"input": query})
+
+    Example:
+        .. code-block:: python
+
+            from langchain_community.llms import OpenAI
+            from langchain.chains import RetrievalQA
+            from langchain_community.vectorstores import FAISS
+            from langchain_core.vectorstores import VectorStoreRetriever
+            retriever = VectorStoreRetriever(vectorstore=FAISS(...))
+            retrievalQA = RetrievalQA.from_llm(llm=OpenAI(), retriever=retriever)
+
+    """
+
+    retriever: BaseRetriever = Field(exclude=True)
+
+    def _get_docs(
         self,
-        low_confidence_spans: List[str],
-        _run_manager: CallbackManagerForChainRun,
-        user_input: str,
-        response: str,
-        initial_response: str,
-    ) -> Tuple[str, bool]:
-        question_gen_inputs = [
-            {
-                "user_input": user_input,
-                "current_response": initial_response,
-                "uncertain_span": span,
-            }
-            for span in low_confidence_spans
-        ]
-        callbacks = _run_manager.get_child()
-        question_gen_outputs = self.question_generator_chain.apply(
-            question_gen_inputs, callbacks=callbacks
-        )
-        questions = [
-            output[self.question_generator_chain.output_keys[0]]
-            for output in question_gen_outputs
-        ]
-        _run_manager.on_text(
-            f"Generated Questions: {questions}", color="yellow", end="\n"
+        question: str,
+        *,
+        run_manager: CallbackManagerForChainRun,
+    ) -> List[Document]:
+        """Get docs."""
+        return self.retriever.invoke(
+            question, config={"callbacks": run_manager.get_child()}
         )
-        return self._do_generation(questions, user_input, response, _run_manager)
 
-    def _call(
+    async def _aget_docs(
         self,
-        inputs: Dict[str, Any],
-        run_manager: Optional[CallbackManagerForChainRun] = None,
-    ) -> Dict[str, Any]:
-        _run_manager = run_manager or CallbackManagerForChainRun.get_noop_manager()
+        question: str,
+        *,
+        run_manager: AsyncCallbackManagerForChainRun,
+    ) -> List[Document]:
+        """Get docs."""
+        return await self.retriever.ainvoke(
+            question, config={"callbacks": run_manager.get_child()}
+        )
 
-        user_input = inputs[self.input_keys[0]]
+    @property
+    def _chain_type(self) -> str:
+        """Return the chain type."""
+        return "retrieval_qa"
+
+
+class VectorDBQA(BaseRetrievalQA):
+    """Chain for question-answering against a vector database."""
+
+    vectorstore: VectorStore = Field(exclude=True, alias="vectorstore")
+    """Vector Database to connect to."""
+    k: int = 4
+    """Number of documents to query for."""
+    search_type: str = "similarity"
+    """Search type to use over vectorstore. `similarity` or `mmr`."""
+    search_kwargs: Dict[str, Any] = Field(default_factory=dict)
+    """Extra search args."""
+
+    @root_validator()
+    def raise_deprecation(cls, values: Dict) -> Dict:
+        warnings.warn(
+            "`VectorDBQA` is deprecated - "
+            "please use `from langchain.chains import RetrievalQA`"
+        )
+        return values
 
-        response = ""
+    @root_validator()
+    def validate_search_type(cls, values: Dict) -> Dict:
+        """Validate search type."""
+        if "search_type" in values:
+            search_type = values["search_type"]
+            if search_type not in ("similarity", "mmr"):
+                raise ValueError(f"search_type of {search_type} not allowed.")
+        return values
 
-        for i in range(self.max_iter):
-            _run_manager.on_text(
-                f"Current Response: {response}", color="blue", end="\n"
-            )
-            _input = {"user_input": user_input, "context": "", "response": response}
-            tokens, log_probs = self.response_chain.generate_tokens_and_log_probs(
-                _input, run_manager=_run_manager
-            )
-            low_confidence_spans = _low_confidence_spans(
-                tokens,
-                log_probs,
-                self.min_prob,
-                self.min_token_gap,
-                self.num_pad_tokens,
+    def _get_docs(
+        self,
+        question: str,
+        *,
+        run_manager: CallbackManagerForChainRun,
+    ) -> List[Document]:
+        """Get docs."""
+        if self.search_type == "similarity":
+            docs = self.vectorstore.similarity_search(
+                question, k=self.k, **self.search_kwargs
             )
-            initial_response = response.strip() + " " + "".join(tokens)
-            if not low_confidence_spans:
-                response = initial_response
-                final_response, finished = self.output_parser.parse(response)
-                if finished:
-                    return {self.output_keys[0]: final_response}
-                continue
-
-            marginal, finished = self._do_retrieval(
-                low_confidence_spans,
-                _run_manager,
-                user_input,
-                response,
-                initial_response,
+        elif self.search_type == "mmr":
+            docs = self.vectorstore.max_marginal_relevance_search(
+                question, k=self.k, **self.search_kwargs
             )
-            response = response.strip() + " " + marginal
-            if finished:
-                break
-        return {self.output_keys[0]: response}
+        else:
+            raise ValueError(f"search_type of {self.search_type} not allowed.")
+        return docs
 
-    @classmethod
-    def from_llm(
-        cls, llm: BaseLanguageModel, max_generation_len: int = 32, **kwargs: Any
-    ) -> FlareChain:
-        """Creates a FlareChain from a language model.
-
-        Args:
-            llm: Language model to use.
-            max_generation_len: Maximum length of the generated response.
-            **kwargs: Additional arguments to pass to the constructor.
+    async def _aget_docs(
+        self,
+        question: str,
+        *,
+        run_manager: AsyncCallbackManagerForChainRun,
+    ) -> List[Document]:
+        """Get docs."""
+        raise NotImplementedError("VectorDBQA does not support async")
 
-        Returns:
-            FlareChain class with the given language model.
-        """
-        question_gen_chain = QuestionGeneratorChain(llm=llm)
-        response_llm = OpenAI(
-            max_tokens=max_generation_len, model_kwargs={"logprobs": 1}, temperature=0
-        )
-        response_chain = _OpenAIResponseChain(llm=response_llm)
-        return cls(
-            question_generator_chain=question_gen_chain,
-            response_chain=response_chain,
-            **kwargs,
-        )
+    @property
+    def _chain_type(self) -> str:
+        """Return the chain type."""
+        return "vector_db_qa"
```

### Comparing `gigachain-0.1.9/langchain/chains/flare/prompts.py` & `gigachain-0.2.0/langchain/chains/flare/prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/graph_qa/kuzu.py` & `gigachain-0.2.0/langchain/chains/openai_functions/citation_fuzzy_match.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,103 +1,106 @@
-"""Question answering over a graph."""
-from __future__ import annotations
+from typing import Iterator, List
 
-from typing import Any, Dict, List, Optional
-
-from langchain_community.graphs.kuzu_graph import KuzuGraph
-from langchain_core.callbacks import CallbackManagerForChainRun
 from langchain_core.language_models import BaseLanguageModel
-from langchain_core.prompts import BasePromptTemplate
-from langchain_core.pydantic_v1 import Field
+from langchain_core.messages import HumanMessage, SystemMessage
+from langchain_core.output_parsers.openai_functions import PydanticOutputFunctionsParser
+from langchain_core.prompts.chat import ChatPromptTemplate, HumanMessagePromptTemplate
+from langchain_core.pydantic_v1 import BaseModel, Field
 
-from langchain.chains.base import Chain
-from langchain.chains.graph_qa.prompts import CYPHER_QA_PROMPT, KUZU_GENERATION_PROMPT
 from langchain.chains.llm import LLMChain
+from langchain.chains.openai_functions.utils import get_llm_kwargs
 
 
-class KuzuQAChain(Chain):
-    """Question-answering against a graph by generating Cypher statements for Kùzu.
-
-    *Security note*: Make sure that the database connection uses credentials
-        that are narrowly-scoped to only include necessary permissions.
-        Failure to do so may result in data corruption or loss, since the calling
-        code may attempt commands that would result in deletion, mutation
-        of data if appropriately prompted or reading sensitive data if such
-        data is present in the database.
-        The best way to guard against such negative outcomes is to (as appropriate)
-        limit the permissions granted to the credentials used with this tool.
+class FactWithEvidence(BaseModel):
+    """Class representing a single statement.
 
-        See https://python.langchain.com/docs/security for more information.
+    Each fact has a body and a list of sources.
+    If there are multiple facts make sure to break them apart
+    such that each one only uses a set of sources that are relevant to it.
     """
 
-    graph: KuzuGraph = Field(exclude=True)
-    cypher_generation_chain: LLMChain
-    qa_chain: LLMChain
-    input_key: str = "query"  #: :meta private:
-    output_key: str = "result"  #: :meta private:
-
-    @property
-    def input_keys(self) -> List[str]:
-        """Return the input keys.
-
-        :meta private:
-        """
-        return [self.input_key]
-
-    @property
-    def output_keys(self) -> List[str]:
-        """Return the output keys.
-
-        :meta private:
-        """
-        _output_keys = [self.output_key]
-        return _output_keys
-
-    @classmethod
-    def from_llm(
-        cls,
-        llm: BaseLanguageModel,
-        *,
-        qa_prompt: BasePromptTemplate = CYPHER_QA_PROMPT,
-        cypher_prompt: BasePromptTemplate = KUZU_GENERATION_PROMPT,
-        **kwargs: Any,
-    ) -> KuzuQAChain:
-        """Initialize from LLM."""
-        qa_chain = LLMChain(llm=llm, prompt=qa_prompt)
-        cypher_generation_chain = LLMChain(llm=llm, prompt=cypher_prompt)
-
-        return cls(
-            qa_chain=qa_chain,
-            cypher_generation_chain=cypher_generation_chain,
-            **kwargs,
-        )
-
-    def _call(
-        self,
-        inputs: Dict[str, Any],
-        run_manager: Optional[CallbackManagerForChainRun] = None,
-    ) -> Dict[str, str]:
-        """Generate Cypher statement, use it to look up in db and answer question."""
-        _run_manager = run_manager or CallbackManagerForChainRun.get_noop_manager()
-        callbacks = _run_manager.get_child()
-        question = inputs[self.input_key]
-
-        generated_cypher = self.cypher_generation_chain.run(
-            {"question": question, "schema": self.graph.get_schema}, callbacks=callbacks
-        )
-
-        _run_manager.on_text("Generated Cypher:", end="\n", verbose=self.verbose)
-        _run_manager.on_text(
-            generated_cypher, color="green", end="\n", verbose=self.verbose
-        )
-        context = self.graph.query(generated_cypher)
-
-        _run_manager.on_text("Full Context:", end="\n", verbose=self.verbose)
-        _run_manager.on_text(
-            str(context), color="green", end="\n", verbose=self.verbose
-        )
-
-        result = self.qa_chain(
-            {"question": question, "context": context},
-            callbacks=callbacks,
-        )
-        return {self.output_key: result[self.qa_chain.output_key]}
+    fact: str = Field(..., description="Body of the sentence, as part of a response")
+    substring_quote: List[str] = Field(
+        ...,
+        description=(
+            "Each source should be a direct quote from the context, "
+            "as a substring of the original content"
+        ),
+    )
+
+    def _get_span(self, quote: str, context: str, errs: int = 100) -> Iterator[str]:
+        import regex
+
+        minor = quote
+        major = context
+
+        errs_ = 0
+        s = regex.search(f"({minor}){{e<={errs_}}}", major)
+        while s is None and errs_ <= errs:
+            errs_ += 1
+            s = regex.search(f"({minor}){{e<={errs_}}}", major)
+
+        if s is not None:
+            yield from s.spans()
+
+    def get_spans(self, context: str) -> Iterator[str]:
+        for quote in self.substring_quote:
+            yield from self._get_span(quote, context)
+
+
+class QuestionAnswer(BaseModel):
+    """A question and its answer as a list of facts each one should have a source.
+    each sentence contains a body and a list of sources."""
+
+    question: str = Field(..., description="Question that was asked")
+    answer: List[FactWithEvidence] = Field(
+        ...,
+        description=(
+            "Body of the answer, each fact should be "
+            "its separate object with a body and a list of sources"
+        ),
+    )
+
+
+def create_citation_fuzzy_match_chain(llm: BaseLanguageModel) -> LLMChain:
+    """Create a citation fuzzy match chain.
+
+    Args:
+        llm: Language model to use for the chain.
+
+    Returns:
+        Chain (LLMChain) that can be used to answer questions with citations.
+    """
+    output_parser = PydanticOutputFunctionsParser(pydantic_schema=QuestionAnswer)
+    schema = QuestionAnswer.schema()
+    function = {
+        "name": schema["title"],
+        "description": schema["description"],
+        "parameters": schema,
+    }
+    llm_kwargs = get_llm_kwargs(function)
+    messages = [
+        SystemMessage(
+            content=(
+                "You are a world class algorithm to answer "
+                "questions with correct and exact citations."
+            )
+        ),
+        HumanMessage(content="Answer question using the following context"),
+        HumanMessagePromptTemplate.from_template("{context}"),
+        HumanMessagePromptTemplate.from_template("Question: {question}"),
+        HumanMessage(
+            content=(
+                "Tips: Make sure to cite your sources, "
+                "and use the exact words from the context."
+            )
+        ),
+    ]
+    prompt = ChatPromptTemplate(messages=messages)  # type: ignore[arg-type, call-arg]
+
+    chain = LLMChain(
+        llm=llm,
+        prompt=prompt,
+        llm_kwargs=llm_kwargs,
+        output_parser=output_parser,
+    )
+    return chain
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gigachain-0.1.9/langchain/chains/history_aware_retriever.py` & `gigachain-0.2.0/langchain/chains/history_aware_retriever.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/hyde/base.py` & `gigachain-0.2.0/langchain/chains/hyde/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Hypothetical Document Embeddings.
 
 https://arxiv.org/abs/2212.10496
 """
+
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional
 
 import numpy as np
 from langchain_core.callbacks import CallbackManagerForChainRun
 from langchain_core.embeddings import Embeddings
```

### Comparing `gigachain-0.1.9/langchain/chains/hyde/prompts.py` & `gigachain-0.2.0/langchain/chains/hyde/prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/llm.py` & `gigachain-0.2.0/langchain/chains/llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Chain that just formats a prompt and calls an LLM."""
+
 from __future__ import annotations
 
 import warnings
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union, cast
 
+from langchain_core._api import deprecated
 from langchain_core.callbacks import (
     AsyncCallbackManager,
     AsyncCallbackManagerForChainRun,
     CallbackManager,
     CallbackManagerForChainRun,
     Callbacks,
 )
@@ -30,17 +32,39 @@
 )
 from langchain_core.runnables.configurable import DynamicRunnable
 from langchain_core.utils.input import get_colored_text
 
 from langchain.chains.base import Chain
 
 
+@deprecated(
+    since="0.1.17",
+    alternative="RunnableSequence, e.g., `prompt | llm`",
+    removal="0.3.0",
+)
 class LLMChain(Chain):
     """Chain to run queries against LLMs.
 
+    This class is deprecated. See below for an example implementation using
+    LangChain runnables:
+
+        .. code-block:: python
+
+            from langchain_core.prompts import PromptTemplate
+            from langchain_openai import OpenAI
+
+            prompt_template = "Tell me a {adjective} joke"
+            prompt = PromptTemplate(
+                input_variables=["adjective"], template=prompt_template
+            )
+            llm = OpenAI()
+            chain = prompt | llm
+
+            chain.invoke("your adjective here")
+
     Example:
         .. code-block:: python
 
             from langchain.chains import LLMChain
             from langchain_community.llms import OpenAI
             from langchain_core.prompts import PromptTemplate
             prompt_template = "Tell me a {adjective} joke"
```

### Comparing `gigachain-0.1.9/langchain/chains/llm_checker/base.py` & `gigachain-0.2.0/langchain/chains/llm_checker/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Chain for question-answering with self-verification."""
+
 from __future__ import annotations
 
 import warnings
 from typing import Any, Dict, List, Optional
 
 from langchain_core.callbacks import CallbackManagerForChainRun
 from langchain_core.language_models import BaseLanguageModel
@@ -50,15 +51,15 @@
     chains = [
         create_draft_answer_chain,
         list_assertions_chain,
         check_assertions_chain,
         revised_answer_chain,
     ]
     question_to_checked_assertions_chain = SequentialChain(
-        chains=chains,
+        chains=chains,  # type: ignore[arg-type]
         input_variables=["question"],
         output_variables=["revised_statement"],
         verbose=True,
     )
     return question_to_checked_assertions_chain
```

### Comparing `gigachain-0.1.9/langchain/chains/llm_checker/prompt.py` & `gigachain-0.2.0/langchain/chains/llm_checker/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/llm_math/base.py` & `gigachain-0.2.0/langchain/chains/llm_math/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Chain that interprets a prompt and executes python code to do math."""
+
 from __future__ import annotations
 
 import math
 import re
 import warnings
 from typing import Any, Dict, List, Optional
 
@@ -77,15 +78,15 @@
         """Expect output key.
 
         :meta private:
         """
         return [self.output_key]
 
     def _evaluate_expression(self, expression: str) -> str:
-        import numexpr  # noqa: F401
+        import numexpr
 
         try:
             local_dict = {"pi": math.pi, "e": math.e}
             output = str(
                 numexpr.evaluate(
                     expression.strip(),
                     global_dict={},  # restrict access to globals
```

### Comparing `gigachain-0.1.9/langchain/chains/llm_math/prompt.py` & `gigachain-0.2.0/langchain/chains/llm_math/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/llm_summarization_checker/base.py` & `gigachain-0.2.0/langchain/chains/llm_summarization_checker/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt` & `gigachain-0.2.0/langchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/llm_summarization_checker/prompts/check_facts.txt` & `gigachain-0.2.0/langchain/chains/llm_summarization_checker/prompts/check_facts.txt`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/llm_summarization_checker/prompts/revise_summary.txt` & `gigachain-0.2.0/langchain/chains/llm_summarization_checker/prompts/revise_summary.txt`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/loading.py` & `gigachain-0.2.0/langchain/chains/loading.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,73 @@
 """Functionality for loading chains."""
+from __future__ import annotations
+
 import json
 from pathlib import Path
-from typing import Any, Union
+from typing import TYPE_CHECKING, Any, Union
 
 import yaml
-from langchain_community.llms.loading import load_llm, load_llm_from_config
 from langchain_core.prompts.loading import (
     _load_output_parser,
     load_prompt,
     load_prompt_from_config,
 )
-from langchain_core.utils.loading import try_load_from_hub
 
 from langchain.chains import ReduceDocumentsChain
 from langchain.chains.api.base import APIChain
 from langchain.chains.base import Chain
 from langchain.chains.combine_documents.map_reduce import MapReduceDocumentsChain
 from langchain.chains.combine_documents.map_rerank import MapRerankDocumentsChain
 from langchain.chains.combine_documents.refine import RefineDocumentsChain
 from langchain.chains.combine_documents.stuff import StuffDocumentsChain
-from langchain.chains.graph_qa.cypher import GraphCypherQAChain
 from langchain.chains.hyde.base import HypotheticalDocumentEmbedder
 from langchain.chains.llm import LLMChain
 from langchain.chains.llm_checker.base import LLMCheckerChain
 from langchain.chains.llm_math.base import LLMMathChain
-from langchain.chains.llm_requests import LLMRequestsChain
 from langchain.chains.qa_with_sources.base import QAWithSourcesChain
 from langchain.chains.qa_with_sources.retrieval import RetrievalQAWithSourcesChain
 from langchain.chains.qa_with_sources.vector_db import VectorDBQAWithSourcesChain
 from langchain.chains.retrieval_qa.base import RetrievalQA, VectorDBQA
 
+if TYPE_CHECKING:
+    from langchain_community.chains.graph_qa.cypher import GraphCypherQAChain
+
+    from langchain.chains.llm_requests import LLMRequestsChain
+
+try:
+    from langchain_community.llms.loading import load_llm, load_llm_from_config
+except ImportError:
+
+    def load_llm(*args: Any, **kwargs: Any) -> None:  # type: ignore
+        raise ImportError(
+            "To use this load_llm functionality you must install the "
+            "langchain_community package. "
+            "You can install it with `pip install langchain_community`"
+        )
+
+    def load_llm_from_config(  # type: ignore
+        *args: Any, **kwargs: Any
+    ) -> None:
+        raise ImportError(
+            "To use this load_llm_from_config functionality you must install the "
+            "langchain_community package. "
+            "You can install it with `pip install langchain_community`"
+        )
+
+
 URL_BASE = "https://raw.githubusercontent.com/hwchase17/langchain-hub/master/chains/"
 
 
 def _load_llm_chain(config: dict, **kwargs: Any) -> LLMChain:
     """Load LLM chain from config dict."""
     if "llm" in config:
         llm_config = config.pop("llm")
-        llm = load_llm_from_config(llm_config)
+        llm = load_llm_from_config(llm_config, **kwargs)
     elif "llm_path" in config:
-        llm = load_llm(config.pop("llm_path"))
+        llm = load_llm(config.pop("llm_path"), **kwargs)
     else:
         raise ValueError("One of `llm` or `llm_path` must be present.")
 
     if "prompt" in config:
         prompt_config = config.pop("prompt")
         prompt = load_prompt_from_config(prompt_config)
     elif "prompt_path" in config:
@@ -55,34 +79,36 @@
     return LLMChain(llm=llm, prompt=prompt, **config)
 
 
 def _load_hyde_chain(config: dict, **kwargs: Any) -> HypotheticalDocumentEmbedder:
     """Load hypothetical document embedder chain from config dict."""
     if "llm_chain" in config:
         llm_chain_config = config.pop("llm_chain")
-        llm_chain = load_chain_from_config(llm_chain_config)
+        llm_chain = load_chain_from_config(llm_chain_config, **kwargs)
     elif "llm_chain_path" in config:
-        llm_chain = load_chain(config.pop("llm_chain_path"))
+        llm_chain = load_chain(config.pop("llm_chain_path"), **kwargs)
     else:
         raise ValueError("One of `llm_chain` or `llm_chain_path` must be present.")
     if "embeddings" in kwargs:
         embeddings = kwargs.pop("embeddings")
     else:
         raise ValueError("`embeddings` must be present.")
     return HypotheticalDocumentEmbedder(
-        llm_chain=llm_chain, base_embeddings=embeddings, **config
+        llm_chain=llm_chain,  # type: ignore[arg-type]
+        base_embeddings=embeddings,
+        **config,  # type: ignore[arg-type]
     )
 
 
 def _load_stuff_documents_chain(config: dict, **kwargs: Any) -> StuffDocumentsChain:
     if "llm_chain" in config:
         llm_chain_config = config.pop("llm_chain")
-        llm_chain = load_chain_from_config(llm_chain_config)
+        llm_chain = load_chain_from_config(llm_chain_config, **kwargs)
     elif "llm_chain_path" in config:
-        llm_chain = load_chain(config.pop("llm_chain_path"))
+        llm_chain = load_chain(config.pop("llm_chain_path"), **kwargs)
     else:
         raise ValueError("One of `llm_chain` or `llm_chain_path` must be present.")
 
     if not isinstance(llm_chain, LLMChain):
         raise ValueError(f"Expected LLMChain, got {llm_chain}")
 
     if "document_prompt" in config:
@@ -101,127 +127,137 @@
 
 
 def _load_map_reduce_documents_chain(
     config: dict, **kwargs: Any
 ) -> MapReduceDocumentsChain:
     if "llm_chain" in config:
         llm_chain_config = config.pop("llm_chain")
-        llm_chain = load_chain_from_config(llm_chain_config)
+        llm_chain = load_chain_from_config(llm_chain_config, **kwargs)
     elif "llm_chain_path" in config:
-        llm_chain = load_chain(config.pop("llm_chain_path"))
+        llm_chain = load_chain(config.pop("llm_chain_path"), **kwargs)
     else:
         raise ValueError("One of `llm_chain` or `llm_chain_path` must be present.")
 
     if not isinstance(llm_chain, LLMChain):
         raise ValueError(f"Expected LLMChain, got {llm_chain}")
 
     if "reduce_documents_chain" in config:
         reduce_documents_chain = load_chain_from_config(
-            config.pop("reduce_documents_chain")
+            config.pop("reduce_documents_chain"), **kwargs
         )
     elif "reduce_documents_chain_path" in config:
-        reduce_documents_chain = load_chain(config.pop("reduce_documents_chain_path"))
+        reduce_documents_chain = load_chain(
+            config.pop("reduce_documents_chain_path"), **kwargs
+        )
     else:
-        reduce_documents_chain = _load_reduce_documents_chain(config)
+        reduce_documents_chain = _load_reduce_documents_chain(config, **kwargs)
 
     return MapReduceDocumentsChain(
         llm_chain=llm_chain,
-        reduce_documents_chain=reduce_documents_chain,
+        reduce_documents_chain=reduce_documents_chain,  # type: ignore[arg-type]
         **config,
     )
 
 
-def _load_reduce_documents_chain(config: dict, **kwargs: Any) -> ReduceDocumentsChain:
+def _load_reduce_documents_chain(config: dict, **kwargs: Any) -> ReduceDocumentsChain:  # type: ignore[valid-type]
     combine_documents_chain = None
     collapse_documents_chain = None
 
     if "combine_documents_chain" in config:
         combine_document_chain_config = config.pop("combine_documents_chain")
-        combine_documents_chain = load_chain_from_config(combine_document_chain_config)
+        combine_documents_chain = load_chain_from_config(
+            combine_document_chain_config, **kwargs
+        )
     elif "combine_document_chain" in config:
         combine_document_chain_config = config.pop("combine_document_chain")
-        combine_documents_chain = load_chain_from_config(combine_document_chain_config)
+        combine_documents_chain = load_chain_from_config(
+            combine_document_chain_config, **kwargs
+        )
     elif "combine_documents_chain_path" in config:
-        combine_documents_chain = load_chain(config.pop("combine_documents_chain_path"))
+        combine_documents_chain = load_chain(
+            config.pop("combine_documents_chain_path"), **kwargs
+        )
     elif "combine_document_chain_path" in config:
-        combine_documents_chain = load_chain(config.pop("combine_document_chain_path"))
+        combine_documents_chain = load_chain(
+            config.pop("combine_document_chain_path"), **kwargs
+        )
     else:
         raise ValueError(
             "One of `combine_documents_chain` or "
             "`combine_documents_chain_path` must be present."
         )
 
     if "collapse_documents_chain" in config:
         collapse_document_chain_config = config.pop("collapse_documents_chain")
         if collapse_document_chain_config is None:
             collapse_documents_chain = None
         else:
             collapse_documents_chain = load_chain_from_config(
-                collapse_document_chain_config
+                collapse_document_chain_config, **kwargs
             )
     elif "collapse_documents_chain_path" in config:
         collapse_documents_chain = load_chain(
-            config.pop("collapse_documents_chain_path")
+            config.pop("collapse_documents_chain_path"), **kwargs
         )
     elif "collapse_document_chain" in config:
         collapse_document_chain_config = config.pop("collapse_document_chain")
         if collapse_document_chain_config is None:
             collapse_documents_chain = None
         else:
             collapse_documents_chain = load_chain_from_config(
-                collapse_document_chain_config
+                collapse_document_chain_config, **kwargs
             )
     elif "collapse_document_chain_path" in config:
         collapse_documents_chain = load_chain(
-            config.pop("collapse_document_chain_path")
+            config.pop("collapse_document_chain_path"), **kwargs
         )
 
-    return ReduceDocumentsChain(
+    return ReduceDocumentsChain(  # type: ignore[misc]
         combine_documents_chain=combine_documents_chain,
         collapse_documents_chain=collapse_documents_chain,
         **config,
     )
 
 
 def _load_llm_bash_chain(config: dict, **kwargs: Any) -> Any:
     from langchain_experimental.llm_bash.base import LLMBashChain
 
     llm_chain = None
     if "llm_chain" in config:
         llm_chain_config = config.pop("llm_chain")
-        llm_chain = load_chain_from_config(llm_chain_config)
+        llm_chain = load_chain_from_config(llm_chain_config, **kwargs)
     elif "llm_chain_path" in config:
-        llm_chain = load_chain(config.pop("llm_chain_path"))
+        llm_chain = load_chain(config.pop("llm_chain_path"), **kwargs)
     # llm attribute is deprecated in favor of llm_chain, here to support old configs
     elif "llm" in config:
         llm_config = config.pop("llm")
-        llm = load_llm_from_config(llm_config)
+        llm = load_llm_from_config(llm_config, **kwargs)
     # llm_path attribute is deprecated in favor of llm_chain_path,
     # its to support old configs
     elif "llm_path" in config:
-        llm = load_llm(config.pop("llm_path"))
+        llm = load_llm(config.pop("llm_path"), **kwargs)
     else:
         raise ValueError("One of `llm_chain` or `llm_chain_path` must be present.")
     if "prompt" in config:
         prompt_config = config.pop("prompt")
         prompt = load_prompt_from_config(prompt_config)
     elif "prompt_path" in config:
         prompt = load_prompt(config.pop("prompt_path"))
     if llm_chain:
-        return LLMBashChain(llm_chain=llm_chain, prompt=prompt, **config)
+        return LLMBashChain(llm_chain=llm_chain, prompt=prompt, **config)  # type: ignore[arg-type]
     else:
         return LLMBashChain(llm=llm, prompt=prompt, **config)
 
 
 def _load_llm_checker_chain(config: dict, **kwargs: Any) -> LLMCheckerChain:
     if "llm" in config:
         llm_config = config.pop("llm")
-        llm = load_llm_from_config(llm_config)
+        llm = load_llm_from_config(llm_config, **kwargs)
     elif "llm_path" in config:
-        llm = load_llm(config.pop("llm_path"))
+        llm = load_llm(config.pop("llm_path"), **kwargs)
     else:
         raise ValueError("One of `llm` or `llm_path` must be present.")
     if "create_draft_answer_prompt" in config:
         create_draft_answer_prompt_config = config.pop("create_draft_answer_prompt")
         create_draft_answer_prompt = load_prompt_from_config(
             create_draft_answer_prompt_config
         )
@@ -246,138 +282,142 @@
     if "revised_answer_prompt" in config:
         revised_answer_prompt_config = config.pop("revised_answer_prompt")
         revised_answer_prompt = load_prompt_from_config(revised_answer_prompt_config)
     elif "revised_answer_prompt_path" in config:
         revised_answer_prompt = load_prompt(config.pop("revised_answer_prompt_path"))
     return LLMCheckerChain(
         llm=llm,
-        create_draft_answer_prompt=create_draft_answer_prompt,
-        list_assertions_prompt=list_assertions_prompt,
-        check_assertions_prompt=check_assertions_prompt,
-        revised_answer_prompt=revised_answer_prompt,
+        create_draft_answer_prompt=create_draft_answer_prompt,  # type: ignore[arg-type]
+        list_assertions_prompt=list_assertions_prompt,  # type: ignore[arg-type]
+        check_assertions_prompt=check_assertions_prompt,  # type: ignore[arg-type]
+        revised_answer_prompt=revised_answer_prompt,  # type: ignore[arg-type]
         **config,
     )
 
 
 def _load_llm_math_chain(config: dict, **kwargs: Any) -> LLMMathChain:
     llm_chain = None
     if "llm_chain" in config:
         llm_chain_config = config.pop("llm_chain")
-        llm_chain = load_chain_from_config(llm_chain_config)
+        llm_chain = load_chain_from_config(llm_chain_config, **kwargs)
     elif "llm_chain_path" in config:
-        llm_chain = load_chain(config.pop("llm_chain_path"))
+        llm_chain = load_chain(config.pop("llm_chain_path"), **kwargs)
     # llm attribute is deprecated in favor of llm_chain, here to support old configs
     elif "llm" in config:
         llm_config = config.pop("llm")
-        llm = load_llm_from_config(llm_config)
+        llm = load_llm_from_config(llm_config, **kwargs)
     # llm_path attribute is deprecated in favor of llm_chain_path,
     # its to support old configs
     elif "llm_path" in config:
-        llm = load_llm(config.pop("llm_path"))
+        llm = load_llm(config.pop("llm_path"), **kwargs)
     else:
         raise ValueError("One of `llm_chain` or `llm_chain_path` must be present.")
     if "prompt" in config:
         prompt_config = config.pop("prompt")
         prompt = load_prompt_from_config(prompt_config)
     elif "prompt_path" in config:
         prompt = load_prompt(config.pop("prompt_path"))
     if llm_chain:
-        return LLMMathChain(llm_chain=llm_chain, prompt=prompt, **config)
+        return LLMMathChain(llm_chain=llm_chain, prompt=prompt, **config)  # type: ignore[arg-type]
     else:
         return LLMMathChain(llm=llm, prompt=prompt, **config)
 
 
 def _load_map_rerank_documents_chain(
     config: dict, **kwargs: Any
 ) -> MapRerankDocumentsChain:
     if "llm_chain" in config:
         llm_chain_config = config.pop("llm_chain")
-        llm_chain = load_chain_from_config(llm_chain_config)
+        llm_chain = load_chain_from_config(llm_chain_config, **kwargs)
     elif "llm_chain_path" in config:
-        llm_chain = load_chain(config.pop("llm_chain_path"))
+        llm_chain = load_chain(config.pop("llm_chain_path"), **kwargs)
     else:
         raise ValueError("One of `llm_chain` or `llm_chain_path` must be present.")
-    return MapRerankDocumentsChain(llm_chain=llm_chain, **config)
+    return MapRerankDocumentsChain(llm_chain=llm_chain, **config)  # type: ignore[arg-type]
 
 
 def _load_pal_chain(config: dict, **kwargs: Any) -> Any:
     from langchain_experimental.pal_chain import PALChain
 
     if "llm_chain" in config:
         llm_chain_config = config.pop("llm_chain")
-        llm_chain = load_chain_from_config(llm_chain_config)
+        llm_chain = load_chain_from_config(llm_chain_config, **kwargs)
     elif "llm_chain_path" in config:
-        llm_chain = load_chain(config.pop("llm_chain_path"))
+        llm_chain = load_chain(config.pop("llm_chain_path"), **kwargs)
     else:
         raise ValueError("One of `llm_chain` or `llm_chain_path` must be present.")
-    return PALChain(llm_chain=llm_chain, **config)
+    return PALChain(llm_chain=llm_chain, **config)  # type: ignore[arg-type]
 
 
 def _load_refine_documents_chain(config: dict, **kwargs: Any) -> RefineDocumentsChain:
     if "initial_llm_chain" in config:
         initial_llm_chain_config = config.pop("initial_llm_chain")
-        initial_llm_chain = load_chain_from_config(initial_llm_chain_config)
+        initial_llm_chain = load_chain_from_config(initial_llm_chain_config, **kwargs)
     elif "initial_llm_chain_path" in config:
-        initial_llm_chain = load_chain(config.pop("initial_llm_chain_path"))
+        initial_llm_chain = load_chain(config.pop("initial_llm_chain_path"), **kwargs)
     else:
         raise ValueError(
             "One of `initial_llm_chain` or `initial_llm_chain_path` must be present."
         )
     if "refine_llm_chain" in config:
         refine_llm_chain_config = config.pop("refine_llm_chain")
-        refine_llm_chain = load_chain_from_config(refine_llm_chain_config)
+        refine_llm_chain = load_chain_from_config(refine_llm_chain_config, **kwargs)
     elif "refine_llm_chain_path" in config:
-        refine_llm_chain = load_chain(config.pop("refine_llm_chain_path"))
+        refine_llm_chain = load_chain(config.pop("refine_llm_chain_path"), **kwargs)
     else:
         raise ValueError(
             "One of `refine_llm_chain` or `refine_llm_chain_path` must be present."
         )
     if "document_prompt" in config:
         prompt_config = config.pop("document_prompt")
         document_prompt = load_prompt_from_config(prompt_config)
     elif "document_prompt_path" in config:
         document_prompt = load_prompt(config.pop("document_prompt_path"))
     return RefineDocumentsChain(
-        initial_llm_chain=initial_llm_chain,
-        refine_llm_chain=refine_llm_chain,
+        initial_llm_chain=initial_llm_chain,  # type: ignore[arg-type]
+        refine_llm_chain=refine_llm_chain,  # type: ignore[arg-type]
         document_prompt=document_prompt,
         **config,
     )
 
 
 def _load_qa_with_sources_chain(config: dict, **kwargs: Any) -> QAWithSourcesChain:
     if "combine_documents_chain" in config:
         combine_documents_chain_config = config.pop("combine_documents_chain")
-        combine_documents_chain = load_chain_from_config(combine_documents_chain_config)
+        combine_documents_chain = load_chain_from_config(
+            combine_documents_chain_config, **kwargs
+        )
     elif "combine_documents_chain_path" in config:
-        combine_documents_chain = load_chain(config.pop("combine_documents_chain_path"))
+        combine_documents_chain = load_chain(
+            config.pop("combine_documents_chain_path"), **kwargs
+        )
     else:
         raise ValueError(
             "One of `combine_documents_chain` or "
             "`combine_documents_chain_path` must be present."
         )
-    return QAWithSourcesChain(combine_documents_chain=combine_documents_chain, **config)
+    return QAWithSourcesChain(combine_documents_chain=combine_documents_chain, **config)  # type: ignore[arg-type]
 
 
 def _load_sql_database_chain(config: dict, **kwargs: Any) -> Any:
     from langchain_experimental.sql import SQLDatabaseChain
 
     if "database" in kwargs:
         database = kwargs.pop("database")
     else:
         raise ValueError("`database` must be present.")
     if "llm_chain" in config:
         llm_chain_config = config.pop("llm_chain")
-        chain = load_chain_from_config(llm_chain_config)
+        chain = load_chain_from_config(llm_chain_config, **kwargs)
         return SQLDatabaseChain(llm_chain=chain, database=database, **config)
     if "llm" in config:
         llm_config = config.pop("llm")
-        llm = load_llm_from_config(llm_config)
+        llm = load_llm_from_config(llm_config, **kwargs)
     elif "llm_path" in config:
-        llm = load_llm(config.pop("llm_path"))
+        llm = load_llm(config.pop("llm_path"), **kwargs)
     else:
         raise ValueError("One of `llm` or `llm_path` must be present.")
     if "prompt" in config:
         prompt_config = config.pop("prompt")
         prompt = load_prompt_from_config(prompt_config)
     else:
         prompt = None
@@ -390,158 +430,193 @@
 ) -> VectorDBQAWithSourcesChain:
     if "vectorstore" in kwargs:
         vectorstore = kwargs.pop("vectorstore")
     else:
         raise ValueError("`vectorstore` must be present.")
     if "combine_documents_chain" in config:
         combine_documents_chain_config = config.pop("combine_documents_chain")
-        combine_documents_chain = load_chain_from_config(combine_documents_chain_config)
+        combine_documents_chain = load_chain_from_config(
+            combine_documents_chain_config, **kwargs
+        )
     elif "combine_documents_chain_path" in config:
-        combine_documents_chain = load_chain(config.pop("combine_documents_chain_path"))
+        combine_documents_chain = load_chain(
+            config.pop("combine_documents_chain_path"), **kwargs
+        )
     else:
         raise ValueError(
             "One of `combine_documents_chain` or "
             "`combine_documents_chain_path` must be present."
         )
     return VectorDBQAWithSourcesChain(
-        combine_documents_chain=combine_documents_chain,
+        combine_documents_chain=combine_documents_chain,  # type: ignore[arg-type]
         vectorstore=vectorstore,
         **config,
     )
 
 
 def _load_retrieval_qa(config: dict, **kwargs: Any) -> RetrievalQA:
     if "retriever" in kwargs:
         retriever = kwargs.pop("retriever")
     else:
         raise ValueError("`retriever` must be present.")
     if "combine_documents_chain" in config:
         combine_documents_chain_config = config.pop("combine_documents_chain")
-        combine_documents_chain = load_chain_from_config(combine_documents_chain_config)
+        combine_documents_chain = load_chain_from_config(
+            combine_documents_chain_config, **kwargs
+        )
     elif "combine_documents_chain_path" in config:
-        combine_documents_chain = load_chain(config.pop("combine_documents_chain_path"))
+        combine_documents_chain = load_chain(
+            config.pop("combine_documents_chain_path"), **kwargs
+        )
     else:
         raise ValueError(
             "One of `combine_documents_chain` or "
             "`combine_documents_chain_path` must be present."
         )
     return RetrievalQA(
-        combine_documents_chain=combine_documents_chain,
+        combine_documents_chain=combine_documents_chain,  # type: ignore[arg-type]
         retriever=retriever,
         **config,
     )
 
 
 def _load_retrieval_qa_with_sources_chain(
     config: dict, **kwargs: Any
 ) -> RetrievalQAWithSourcesChain:
     if "retriever" in kwargs:
         retriever = kwargs.pop("retriever")
     else:
         raise ValueError("`retriever` must be present.")
     if "combine_documents_chain" in config:
         combine_documents_chain_config = config.pop("combine_documents_chain")
-        combine_documents_chain = load_chain_from_config(combine_documents_chain_config)
+        combine_documents_chain = load_chain_from_config(
+            combine_documents_chain_config, **kwargs
+        )
     elif "combine_documents_chain_path" in config:
-        combine_documents_chain = load_chain(config.pop("combine_documents_chain_path"))
+        combine_documents_chain = load_chain(
+            config.pop("combine_documents_chain_path"), **kwargs
+        )
     else:
         raise ValueError(
             "One of `combine_documents_chain` or "
             "`combine_documents_chain_path` must be present."
         )
     return RetrievalQAWithSourcesChain(
-        combine_documents_chain=combine_documents_chain,
+        combine_documents_chain=combine_documents_chain,  # type: ignore[arg-type]
         retriever=retriever,
         **config,
     )
 
 
 def _load_vector_db_qa(config: dict, **kwargs: Any) -> VectorDBQA:
     if "vectorstore" in kwargs:
         vectorstore = kwargs.pop("vectorstore")
     else:
         raise ValueError("`vectorstore` must be present.")
     if "combine_documents_chain" in config:
         combine_documents_chain_config = config.pop("combine_documents_chain")
-        combine_documents_chain = load_chain_from_config(combine_documents_chain_config)
+        combine_documents_chain = load_chain_from_config(
+            combine_documents_chain_config, **kwargs
+        )
     elif "combine_documents_chain_path" in config:
-        combine_documents_chain = load_chain(config.pop("combine_documents_chain_path"))
+        combine_documents_chain = load_chain(
+            config.pop("combine_documents_chain_path"), **kwargs
+        )
     else:
         raise ValueError(
             "One of `combine_documents_chain` or "
             "`combine_documents_chain_path` must be present."
         )
     return VectorDBQA(
-        combine_documents_chain=combine_documents_chain,
+        combine_documents_chain=combine_documents_chain,  # type: ignore[arg-type]
         vectorstore=vectorstore,
         **config,
     )
 
 
 def _load_graph_cypher_chain(config: dict, **kwargs: Any) -> GraphCypherQAChain:
     if "graph" in kwargs:
         graph = kwargs.pop("graph")
     else:
         raise ValueError("`graph` must be present.")
     if "cypher_generation_chain" in config:
         cypher_generation_chain_config = config.pop("cypher_generation_chain")
-        cypher_generation_chain = load_chain_from_config(cypher_generation_chain_config)
+        cypher_generation_chain = load_chain_from_config(
+            cypher_generation_chain_config, **kwargs
+        )
     else:
         raise ValueError("`cypher_generation_chain` must be present.")
     if "qa_chain" in config:
         qa_chain_config = config.pop("qa_chain")
-        qa_chain = load_chain_from_config(qa_chain_config)
+        qa_chain = load_chain_from_config(qa_chain_config, **kwargs)
     else:
         raise ValueError("`qa_chain` must be present.")
 
+    try:
+        from langchain_community.chains.graph_qa.cypher import GraphCypherQAChain
+    except ImportError:
+        raise ImportError(
+            "To use this GraphCypherQAChain functionality you must install the "
+            "langchain_community package. "
+            "You can install it with `pip install langchain_community`"
+        )
     return GraphCypherQAChain(
         graph=graph,
-        cypher_generation_chain=cypher_generation_chain,
-        qa_chain=qa_chain,
+        cypher_generation_chain=cypher_generation_chain,  # type: ignore[arg-type]
+        qa_chain=qa_chain,  # type: ignore[arg-type]
         **config,
     )
 
 
 def _load_api_chain(config: dict, **kwargs: Any) -> APIChain:
     if "api_request_chain" in config:
         api_request_chain_config = config.pop("api_request_chain")
-        api_request_chain = load_chain_from_config(api_request_chain_config)
+        api_request_chain = load_chain_from_config(api_request_chain_config, **kwargs)
     elif "api_request_chain_path" in config:
         api_request_chain = load_chain(config.pop("api_request_chain_path"))
     else:
         raise ValueError(
             "One of `api_request_chain` or `api_request_chain_path` must be present."
         )
     if "api_answer_chain" in config:
         api_answer_chain_config = config.pop("api_answer_chain")
-        api_answer_chain = load_chain_from_config(api_answer_chain_config)
+        api_answer_chain = load_chain_from_config(api_answer_chain_config, **kwargs)
     elif "api_answer_chain_path" in config:
-        api_answer_chain = load_chain(config.pop("api_answer_chain_path"))
+        api_answer_chain = load_chain(config.pop("api_answer_chain_path"), **kwargs)
     else:
         raise ValueError(
             "One of `api_answer_chain` or `api_answer_chain_path` must be present."
         )
     if "requests_wrapper" in kwargs:
         requests_wrapper = kwargs.pop("requests_wrapper")
     else:
         raise ValueError("`requests_wrapper` must be present.")
     return APIChain(
-        api_request_chain=api_request_chain,
-        api_answer_chain=api_answer_chain,
+        api_request_chain=api_request_chain,  # type: ignore[arg-type]
+        api_answer_chain=api_answer_chain,  # type: ignore[arg-type]
         requests_wrapper=requests_wrapper,
         **config,
     )
 
 
 def _load_llm_requests_chain(config: dict, **kwargs: Any) -> LLMRequestsChain:
+    try:
+        from langchain.chains.llm_requests import LLMRequestsChain
+    except ImportError:
+        raise ImportError(
+            "To use this LLMRequestsChain functionality you must install the "
+            "langchain package. "
+            "You can install it with `pip install langchain`"
+        )
+
     if "llm_chain" in config:
         llm_chain_config = config.pop("llm_chain")
-        llm_chain = load_chain_from_config(llm_chain_config)
+        llm_chain = load_chain_from_config(llm_chain_config, **kwargs)
     elif "llm_chain_path" in config:
-        llm_chain = load_chain(config.pop("llm_chain_path"))
+        llm_chain = load_chain(config.pop("llm_chain_path"), **kwargs)
     else:
         raise ValueError("One of `llm_chain` or `llm_chain_path` must be present.")
     if "requests_wrapper" in kwargs:
         requests_wrapper = kwargs.pop("requests_wrapper")
         return LLMRequestsChain(
             llm_chain=llm_chain, requests_wrapper=requests_wrapper, **config
         )
@@ -584,20 +659,21 @@
 
     chain_loader = type_to_loader_dict[config_type]
     return chain_loader(config, **kwargs)
 
 
 def load_chain(path: Union[str, Path], **kwargs: Any) -> Chain:
     """Unified method for loading a chain from LangChainHub or local fs."""
-    if hub_result := try_load_from_hub(
-        path, _load_chain_from_file, "chains", {"json", "yaml"}, **kwargs
-    ):
-        return hub_result
-    else:
-        return _load_chain_from_file(path, **kwargs)
+    if isinstance(path, str) and path.startswith("lc://"):
+        raise RuntimeError(
+            "Loading from the deprecated github-based Hub is no longer supported. "
+            "Please use the new LangChain Hub at https://smith.langchain.com/hub "
+            "instead."
+        )
+    return _load_chain_from_file(path, **kwargs)
 
 
 def _load_chain_from_file(file: Union[str, Path], **kwargs: Any) -> Chain:
     """Load chain from file."""
     # Convert file to Path object.
     if isinstance(file, str):
         file_path = Path(file)
```

### Comparing `gigachain-0.1.9/langchain/chains/mapreduce.py` & `gigachain-0.2.0/langchain/chains/mapreduce.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """Map-reduce chain.
 
 Splits up a document, sends the smaller parts to the LLM with one prompt,
 then combines the results with another one.
 """
+
 from __future__ import annotations
 
 from typing import Any, Dict, List, Mapping, Optional
 
 from langchain_core.callbacks import CallbackManagerForChainRun, Callbacks
 from langchain_core.documents import Document
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.prompts import BasePromptTemplate
 from langchain_core.pydantic_v1 import Extra
+from langchain_text_splitters import TextSplitter
 
 from langchain.chains import ReduceDocumentsChain
 from langchain.chains.base import Chain
 from langchain.chains.combine_documents.base import BaseCombineDocumentsChain
 from langchain.chains.combine_documents.map_reduce import MapReduceDocumentsChain
 from langchain.chains.combine_documents.stuff import StuffDocumentsChain
 from langchain.chains.llm import LLMChain
-from langchain.text_splitter import TextSplitter
 
 
 class MapReduceChain(Chain):
     """Map-reduce chain."""
 
     combine_documents_chain: BaseCombineDocumentsChain
     """Chain to use to combine documents."""
```

### Comparing `gigachain-0.1.9/langchain/chains/moderation.py` & `gigachain-0.2.0/langchain/chains/moderation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """Pass input through a moderation endpoint."""
+
 from typing import Any, Dict, List, Optional
 
-from langchain_core.callbacks import CallbackManagerForChainRun
-from langchain_core.pydantic_v1 import root_validator
-from langchain_core.utils import get_from_dict_or_env
+from langchain_core.callbacks import (
+    AsyncCallbackManagerForChainRun,
+    CallbackManagerForChainRun,
+)
+from langchain_core.pydantic_v1 import Field, root_validator
+from langchain_core.utils import check_package_version, get_from_dict_or_env
 
 from langchain.chains.base import Chain
 
 
 class OpenAIModerationChain(Chain):
     """Pass input through a moderation endpoint.
 
@@ -21,22 +25,24 @@
         .. code-block:: python
 
             from langchain.chains import OpenAIModerationChain
             moderation = OpenAIModerationChain()
     """
 
     client: Any  #: :meta private:
+    async_client: Any  #: :meta private:
     model_name: Optional[str] = None
     """Moderation model name to use."""
     error: bool = False
     """Whether or not to error if bad content was found."""
     input_key: str = "input"  #: :meta private:
     output_key: str = "output"  #: :meta private:
     openai_api_key: Optional[str] = None
     openai_organization: Optional[str] = None
+    _openai_pre_1_0: bool = Field(default=None)
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that api key and python package exists in environment."""
         openai_api_key = get_from_dict_or_env(
             values, "openai_api_key", "OPENAI_API_KEY"
         )
@@ -48,15 +54,24 @@
         )
         try:
             import openai
 
             openai.api_key = openai_api_key
             if openai_organization:
                 openai.organization = openai_organization
-            values["client"] = openai.Moderation  # type: ignore
+            values["_openai_pre_1_0"] = False
+            try:
+                check_package_version("openai", gte_version="1.0")
+            except ValueError:
+                values["_openai_pre_1_0"] = True
+            if values["_openai_pre_1_0"]:
+                values["client"] = openai.Moderation
+            else:
+                values["client"] = openai.OpenAI()
+                values["async_client"] = openai.AsyncOpenAI()
         except ImportError:
             raise ImportError(
                 "Could not import openai python package. "
                 "Please install it with `pip install openai`."
             )
         return values
 
@@ -72,25 +87,45 @@
     def output_keys(self) -> List[str]:
         """Return output key.
 
         :meta private:
         """
         return [self.output_key]
 
-    def _moderate(self, text: str, results: dict) -> str:
-        if results["flagged"]:
+    def _moderate(self, text: str, results: Any) -> str:
+        if self._openai_pre_1_0:
+            condition = results["flagged"]
+        else:
+            condition = results.flagged
+        if condition:
             error_str = "Text was found that violates OpenAI's content policy."
             if self.error:
                 raise ValueError(error_str)
             else:
                 return error_str
         return text
 
     def _call(
         self,
-        inputs: Dict[str, str],
+        inputs: Dict[str, Any],
         run_manager: Optional[CallbackManagerForChainRun] = None,
-    ) -> Dict[str, str]:
+    ) -> Dict[str, Any]:
+        text = inputs[self.input_key]
+        if self._openai_pre_1_0:
+            results = self.client.create(text)
+            output = self._moderate(text, results["results"][0])
+        else:
+            results = self.client.moderations.create(input=text)
+            output = self._moderate(text, results.results[0])
+        return {self.output_key: output}
+
+    async def _acall(
+        self,
+        inputs: Dict[str, Any],
+        run_manager: Optional[AsyncCallbackManagerForChainRun] = None,
+    ) -> Dict[str, Any]:
+        if self._openai_pre_1_0:
+            return await super()._acall(inputs, run_manager=run_manager)
         text = inputs[self.input_key]
-        results = self.client.create(text)
-        output = self._moderate(text, results["results"][0])
+        results = await self.async_client.moderations.create(input=text)
+        output = self._moderate(text, results.results[0])
         return {self.output_key: output}
```

### Comparing `gigachain-0.1.9/langchain/chains/natbot/base.py` & `gigachain-0.2.0/langchain/chains/natbot/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Implement an LLM driven browser."""
+
 from __future__ import annotations
 
 import warnings
 from typing import Any, Dict, List, Optional
 
-from langchain_community.llms.openai import OpenAI
 from langchain_core.callbacks import CallbackManagerForChainRun
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.pydantic_v1 import Extra, root_validator
 
 from langchain.chains.base import Chain
 from langchain.chains.llm import LLMChain
 from langchain.chains.natbot.prompt import PROMPT
@@ -64,16 +64,19 @@
             if "llm_chain" not in values and values["llm"] is not None:
                 values["llm_chain"] = LLMChain(llm=values["llm"], prompt=PROMPT)
         return values
 
     @classmethod
     def from_default(cls, objective: str, **kwargs: Any) -> NatBotChain:
         """Load with default LLMChain."""
-        llm = OpenAI(temperature=0.5, best_of=10, n=3, max_tokens=50)
-        return cls.from_llm(llm, objective, **kwargs)
+        raise NotImplementedError(
+            "This method is no longer implemented. Please use from_llm."
+            "llm = OpenAI(temperature=0.5, best_of=10, n=3, max_tokens=50)"
+            "For example, NatBotChain.from_llm(llm, objective)"
+        )
 
     @classmethod
     def from_llm(
         cls, llm: BaseLanguageModel, objective: str, **kwargs: Any
     ) -> NatBotChain:
         """Load from LLM."""
         llm_chain = LLMChain(llm=llm, prompt=PROMPT)
```

### Comparing `gigachain-0.1.9/langchain/chains/natbot/crawler.py` & `gigachain-0.2.0/langchain/chains/natbot/crawler.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/natbot/prompt.py` & `gigachain-0.2.0/langchain/chains/natbot/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/openai_functions/__init__.py` & `gigachain-0.2.0/langchain/chains/openai_functions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from langchain_core.utils.function_calling import convert_to_openai_function
+
 from langchain.chains.openai_functions.base import (
-    convert_to_openai_function,
     create_openai_fn_chain,
     create_structured_output_chain,
 )
 from langchain.chains.openai_functions.citation_fuzzy_match import (
     create_citation_fuzzy_match_chain,
 )
 from langchain.chains.openai_functions.extraction import (
```

### Comparing `gigachain-0.1.9/langchain/chains/openai_functions/base.py` & `gigachain-0.2.0/langchain/chains/openai_functions/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Methods for creating chains that use OpenAI function-calling APIs."""
+
 from typing import (
     Any,
     Callable,
     Dict,
     Optional,
     Sequence,
     Type,
@@ -30,33 +31,33 @@
     create_structured_output_runnable,
     get_openai_output_parser,
 )
 
 __all__ = [
     "get_openai_output_parser",
     "create_openai_fn_runnable",
-    "create_structured_output_runnable",
+    "create_structured_output_runnable",  # deprecated
     "create_openai_fn_chain",  # deprecated
     "create_structured_output_chain",  # deprecated
     "PYTHON_TO_JSON_TYPES",  # backwards compatibility
     "convert_to_openai_function",  # backwards compatibility
 ]
 
 
-@deprecated(since="0.1.1", removal="0.2.0", alternative="create_openai_fn_runnable")
+@deprecated(since="0.1.1", removal="0.3.0", alternative="create_openai_fn_runnable")
 def create_openai_fn_chain(
     functions: Sequence[Union[Dict[str, Any], Type[BaseModel], Callable]],
     llm: BaseLanguageModel,
     prompt: BasePromptTemplate,
     *,
     enforce_single_function_usage: bool = True,
     output_key: str = "function",
     output_parser: Optional[BaseLLMOutputParser] = None,
     **kwargs: Any,
-) -> LLMChain:
+) -> LLMChain:  # type: ignore[valid-type]
     """[Legacy] Create an LLM chain that uses OpenAI functions.
 
     Args:
         functions: A sequence of either dictionaries, pydantic.BaseModels classes, or
             Python functions. If dictionaries are passed in, they are assumed to
             already be a valid OpenAI functions. If only a single
             function is passed in, then it will be enforced that the model use that
@@ -128,37 +129,37 @@
     openai_functions = [convert_to_openai_function(f) for f in functions]
     output_parser = output_parser or get_openai_output_parser(functions)
     llm_kwargs: Dict[str, Any] = {
         "functions": openai_functions,
     }
     if len(openai_functions) == 1 and enforce_single_function_usage:
         llm_kwargs["function_call"] = {"name": openai_functions[0]["name"]}
-    llm_chain = LLMChain(
+    llm_chain = LLMChain(  # type: ignore[misc]
         llm=llm,
         prompt=prompt,
         output_parser=output_parser,
         llm_kwargs=llm_kwargs,
         output_key=output_key,
         **kwargs,
     )
     return llm_chain
 
 
 @deprecated(
-    since="0.1.1", removal="0.2.0", alternative="create_structured_output_runnable"
+    since="0.1.1", removal="0.3.0", alternative="ChatOpenAI.with_structured_output"
 )
 def create_structured_output_chain(
     output_schema: Union[Dict[str, Any], Type[BaseModel]],
     llm: BaseLanguageModel,
     prompt: BasePromptTemplate,
     *,
     output_key: str = "function",
     output_parser: Optional[BaseLLMOutputParser] = None,
     **kwargs: Any,
-) -> LLMChain:
+) -> LLMChain:  # type: ignore[valid-type]
     """[Legacy] Create an LLMChain that uses an OpenAI function to get a structured output.
 
     Args:
         output_schema: Either a dictionary or pydantic.BaseModel class. If a dictionary
             is passed in, it's assumed to already be a valid JsonSchema.
             For best results, pydantic.BaseModels should have docstrings describing what
             the schema represents and descriptions for the parameters.
@@ -203,23 +204,23 @@
                 chain.run("Harry was a chubby brown beagle who loved chicken")
                 # -> Dog(name="Harry", color="brown", fav_food="chicken")
     """  # noqa: E501
     if isinstance(output_schema, dict):
         function: Any = {
             "name": "output_formatter",
             "description": (
-                "Output formatter. Should always be used to format your response to the"
-                " user."
+                "Output formatter. Всегда используй его чтобы отформатировать свой"
+                " ответ пользователю."
             ),
             "parameters": output_schema,
         }
     else:
 
         class _OutputFormatter(BaseModel):
-            """Output formatter. Should always be used to format your response to the user."""  # noqa: E501
+            """Output formatter. Всегда используй его чтобы отформатировать свой ответ пользователю."""  # noqa: E501
 
             output: output_schema  # type: ignore
 
         function = _OutputFormatter
         output_parser = output_parser or PydanticAttrOutputFunctionsParser(
             pydantic_schema=_OutputFormatter, attr_name="output"
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gigachain-0.1.9/langchain/chains/openai_functions/extraction.py` & `gigachain-0.2.0/langchain/chains/openai_functions/qa_with_structure.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,122 +1,112 @@
-from typing import Any, List, Optional
+from typing import Any, List, Optional, Type, Union
 
 from langchain_core.language_models import BaseLanguageModel
+from langchain_core.messages import HumanMessage, SystemMessage
+from langchain_core.output_parsers import BaseLLMOutputParser
 from langchain_core.output_parsers.openai_functions import (
-    JsonKeyOutputFunctionsParser,
-    PydanticAttrOutputFunctionsParser,
+    OutputFunctionsParser,
+    PydanticOutputFunctionsParser,
 )
-from langchain_core.prompts import BasePromptTemplate, ChatPromptTemplate
-from langchain_core.pydantic_v1 import BaseModel
+from langchain_core.prompts import PromptTemplate
+from langchain_core.prompts.chat import ChatPromptTemplate, HumanMessagePromptTemplate
+from langchain_core.pydantic_v1 import BaseModel, Field
 
-from langchain.chains.base import Chain
 from langchain.chains.llm import LLMChain
-from langchain.chains.openai_functions.utils import (
-    _convert_schema,
-    _resolve_schema_references,
-    get_llm_kwargs,
-)
-
-
-def _get_extraction_function(entity_schema: dict) -> dict:
-    return {
-        "name": "information_extraction",
-        "description": "Extracts the relevant information from the passage.",
-        "parameters": {
-            "type": "object",
-            "properties": {
-                "info": {"type": "array", "items": _convert_schema(entity_schema)}
-            },
-            "required": ["info"],
-        },
-    }
-
-
-_EXTRACTION_TEMPLATE = """Извлеките и сохраните соответствующие упомянутые сущности \
-вместе с их свойствами из текста.
+from langchain.chains.openai_functions.utils import get_llm_kwargs
 
-Извлекайте только свойства, указанные в функции 'information_extraction'.
 
-Если свойство отсутствует и не требуется в параметрах функции, не включайте его в вывод.
+class AnswerWithSources(BaseModel):
+    """An answer to the question, with sources."""
 
-Текст из которого нужно извлечь сущности:
-{input}
-"""  # noqa: E501
+    answer: str = Field(..., description="Answer to the question that was asked")
+    sources: List[str] = Field(
+        ..., description="List of sources used to answer the question"
+    )
 
 
-def create_extraction_chain(
-    schema: dict,
+def create_qa_with_structure_chain(
     llm: BaseLanguageModel,
-    prompt: Optional[BasePromptTemplate] = None,
-    tags: Optional[List[str]] = None,
+    schema: Union[dict, Type[BaseModel]],
+    output_parser: str = "base",
+    prompt: Optional[Union[PromptTemplate, ChatPromptTemplate]] = None,
     verbose: bool = False,
-) -> Chain:
-    """Creates a chain that extracts information from a passage.
+) -> LLMChain:
+    """Create a question answering chain that returns an answer with sources
+     based on schema.
 
     Args:
-        schema: The schema of the entities to extract.
-        llm: The language model to use.
-        prompt: The prompt to use for extraction.
-        verbose: Whether to run in verbose mode. In verbose mode, some intermediate
-            logs will be printed to the console. Defaults to the global `verbose` value,
-            accessible via `langchain.globals.get_verbose()`.
+        llm: Language model to use for the chain.
+        schema: Pydantic schema to use for the output.
+        output_parser: Output parser to use. Should be one of `pydantic` or `base`.
+            Default to `base`.
+        prompt: Optional prompt to use for the chain.
 
     Returns:
-        Chain that can be used to extract information from a passage.
+
     """
-    function = _get_extraction_function(schema)
-    extraction_prompt = prompt or ChatPromptTemplate.from_template(_EXTRACTION_TEMPLATE)
-    output_parser = JsonKeyOutputFunctionsParser(key_name="info")
+    if output_parser == "pydantic":
+        if not (isinstance(schema, type) and issubclass(schema, BaseModel)):
+            raise ValueError(
+                "Must provide a pydantic class for schema when output_parser is "
+                "'pydantic'."
+            )
+        _output_parser: BaseLLMOutputParser = PydanticOutputFunctionsParser(
+            pydantic_schema=schema
+        )
+    elif output_parser == "base":
+        _output_parser = OutputFunctionsParser()
+    else:
+        raise ValueError(
+            f"Got unexpected output_parser: {output_parser}. "
+            f"Should be one of `pydantic` or `base`."
+        )
+    if isinstance(schema, type) and issubclass(schema, BaseModel):
+        schema_dict = schema.schema()
+    else:
+        schema_dict = schema
+    function = {
+        "name": schema_dict["title"],
+        "description": schema_dict["description"],
+        "parameters": schema_dict,
+    }
     llm_kwargs = get_llm_kwargs(function)
+    messages = [
+        SystemMessage(
+            content=(
+                "You are a world class algorithm to answer "
+                "questions in a specific format."
+            )
+        ),
+        HumanMessage(content="Answer question using the following context"),
+        HumanMessagePromptTemplate.from_template("{context}"),
+        HumanMessagePromptTemplate.from_template("Question: {question}"),
+        HumanMessage(content="Tips: Make sure to answer in the correct format"),
+    ]
+    prompt = prompt or ChatPromptTemplate(messages=messages)  # type: ignore[arg-type, call-arg]
+
     chain = LLMChain(
         llm=llm,
-        prompt=extraction_prompt,
+        prompt=prompt,
         llm_kwargs=llm_kwargs,
-        output_parser=output_parser,
-        tags=tags,
+        output_parser=_output_parser,
         verbose=verbose,
     )
     return chain
 
 
-def create_extraction_chain_pydantic(
-    pydantic_schema: Any,
-    llm: BaseLanguageModel,
-    prompt: Optional[BasePromptTemplate] = None,
-    verbose: bool = False,
-) -> Chain:
-    """Creates a chain that extracts information from a passage using pydantic schema.
+def create_qa_with_sources_chain(
+    llm: BaseLanguageModel, verbose: bool = False, **kwargs: Any
+) -> LLMChain:
+    """Create a question answering chain that returns an answer with sources.
 
     Args:
-        pydantic_schema: The pydantic schema of the entities to extract.
-        llm: The language model to use.
-        prompt: The prompt to use for extraction.
-        verbose: Whether to run in verbose mode. In verbose mode, some intermediate
-            logs will be printed to the console. Defaults to the global `verbose` value,
-            accessible via `langchain.globals.get_verbose()`
+        llm: Language model to use for the chain.
+        verbose: Whether to print the details of the chain
+        **kwargs: Keyword arguments to pass to `create_qa_with_structure_chain`.
 
     Returns:
-        Chain that can be used to extract information from a passage.
+        Chain (LLMChain) that can be used to answer questions with citations.
     """
-
-    class PydanticSchema(BaseModel):
-        info: List[pydantic_schema]  # type: ignore
-
-    openai_schema = pydantic_schema.schema()
-    openai_schema = _resolve_schema_references(
-        openai_schema, openai_schema.get("definitions", {})
-    )
-
-    function = _get_extraction_function(openai_schema)
-    extraction_prompt = prompt or ChatPromptTemplate.from_template(_EXTRACTION_TEMPLATE)
-    output_parser = PydanticAttrOutputFunctionsParser(
-        pydantic_schema=PydanticSchema, attr_name="info"
+    return create_qa_with_structure_chain(
+        llm, AnswerWithSources, verbose=verbose, **kwargs
     )
-    llm_kwargs = get_llm_kwargs(function)
-    chain = LLMChain(
-        llm=llm,
-        prompt=extraction_prompt,
-        llm_kwargs=llm_kwargs,
-        output_parser=output_parser,
-        verbose=verbose,
-    )
-    return chain
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gigachain-0.1.9/langchain/chains/openai_functions/openapi.py` & `gigachain-0.2.0/langchain/chains/openai_functions/openapi.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,29 +2,27 @@
 
 import json
 import re
 from collections import defaultdict
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
 
 import requests
-from langchain_community.chat_models import ChatOpenAI
-from langchain_community.utilities.openapi import OpenAPISpec
 from langchain_core.callbacks import CallbackManagerForChainRun
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.output_parsers.openai_functions import JsonOutputFunctionsParser
 from langchain_core.prompts import BasePromptTemplate, ChatPromptTemplate
 from langchain_core.utils.input import get_colored_text
 from requests import Response
 
 from langchain.chains.base import Chain
 from langchain.chains.llm import LLMChain
 from langchain.chains.sequential import SequentialChain
-from langchain.tools import APIOperation
 
 if TYPE_CHECKING:
+    from langchain_community.utilities.openapi import OpenAPISpec
     from openapi_pydantic import Parameter
 
 
 def _get_description(o: Any, prefer_short: bool) -> Optional[str]:
     summary = getattr(o, "summary", None)
     description = getattr(o, "description", None)
     if prefer_short:
@@ -97,14 +95,22 @@
     Args:
         spec: OpenAPI spec to convert.
 
     Returns:
         Tuple of the OpenAI functions JSON schema and a default function for executing
             a request based on the OpenAI function schema.
     """
+    try:
+        from langchain_community.tools import APIOperation
+    except ImportError:
+        raise ImportError(
+            "Could not import langchain_community.tools. "
+            "Please install it with `pip install langchain-community`."
+        )
+
     if not spec.paths:
         return [], lambda: None
     functions = []
     _name_to_call_map = {}
     for path in spec.paths:
         path_params = {
             (p.name, p.param_in): p for p in spec.get_parameters_for_path(path)
@@ -252,14 +258,21 @@
     Args:
         spec: OpenAPISpec or url/file/text string corresponding to one.
         llm: language model, should be an OpenAI function-calling model, e.g.
             `ChatOpenAI(model="gpt-3.5-turbo-0613")`.
         prompt: Main prompt template to use.
         request_chain: Chain for taking the functions output and executing the request.
     """
+    try:
+        from langchain_community.utilities.openapi import OpenAPISpec
+    except ImportError as e:
+        raise ImportError(
+            "Could not import langchain_community.utilities.openapi. "
+            "Please install it with `pip install langchain-community`."
+        ) from e
     if isinstance(spec, str):
         for conversion in (
             OpenAPISpec.from_url,
             OpenAPISpec.from_file,
             OpenAPISpec.from_text,
         ):
             try:
@@ -268,17 +281,20 @@
             except ImportError as e:
                 raise e
             except Exception:  # noqa: E722
                 pass
         if isinstance(spec, str):
             raise ValueError(f"Unable to parse spec from source {spec}")
     openai_fns, call_api_fn = openapi_spec_to_openai_fn(spec)
-    llm = llm or ChatOpenAI(
-        model="gpt-3.5-turbo-0613",
-    )
+    if not llm:
+        raise ValueError(
+            "Must provide an LLM for this chain.For example,\n"
+            "from langchain_openai import ChatOpenAI\n"
+            "llm = ChatOpenAI()\n"
+        )
     prompt = prompt or ChatPromptTemplate.from_template(
         "Use the provided API's to respond to this user query:\n\n{query}"
     )
     llm_chain = LLMChain(
         llm=llm,
         prompt=prompt,
         llm_kwargs={"functions": openai_fns},
```

### Comparing `gigachain-0.1.9/langchain/chains/openai_functions/tagging.py` & `gigachain-0.2.0/langchain/chains/openai_functions/tagging.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,35 +11,35 @@
 from langchain.chains.llm import LLMChain
 from langchain.chains.openai_functions.utils import _convert_schema, get_llm_kwargs
 
 
 def _get_tagging_function(schema: dict) -> dict:
     return {
         "name": "information_extraction",
-        "description": "Extracts the relevant information from the passage.",
+        "description": "Извлекает релевантную информацию из текста",
         "parameters": _convert_schema(schema),
     }
 
 
-_TAGGING_TEMPLATE = """Extract the desired information from the following passage.
+_TAGGING_TEMPLATE = """Извлеки релевантную информацию из следующего текста.
 
-Only extract the properties mentioned in the 'information_extraction' function.
+Извлекай только свойства, приведенные в функции 'information_extraction'.
 
-Passage:
+Текст:
 {input}
 """
 
 
 def create_tagging_chain(
     schema: dict,
     llm: BaseLanguageModel,
     prompt: Optional[ChatPromptTemplate] = None,
     **kwargs: Any,
 ) -> Chain:
-    """Creates a chain that extracts information from a passage
+    """Create a chain that extracts information from a passage
      based on a schema.
 
     Args:
         schema: The schema of the entities to extract.
         llm: The language model to use.
 
     Returns:
@@ -61,15 +61,15 @@
 
 def create_tagging_chain_pydantic(
     pydantic_schema: Any,
     llm: BaseLanguageModel,
     prompt: Optional[ChatPromptTemplate] = None,
     **kwargs: Any,
 ) -> Chain:
-    """Creates a chain that extracts information from a passage
+    """Create a chain that extracts information from a passage
      based on a pydantic schema.
 
     Args:
         pydantic_schema: The pydantic schema of the entities to extract.
         llm: The language model to use.
 
     Returns:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gigachain-0.1.9/langchain/chains/openai_functions/utils.py` & `gigachain-0.2.0/langchain/chains/openai_functions/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Dict
 
 
 def _resolve_schema_references(schema: Any, definitions: Dict[str, Any]) -> Any:
     """
-    Resolves the $ref keys in a JSON schema object using the provided definitions.
+    Resolve the $ref keys in a JSON schema object using the provided definitions.
     """
     if isinstance(schema, list):
         for i, item in enumerate(schema):
             schema[i] = _resolve_schema_references(item, definitions)
     elif isinstance(schema, dict):
         if "$ref" in schema:
             ref_key = schema.pop("$ref").split("/")[-1]
@@ -25,15 +25,15 @@
         "type": "object",
         "properties": props,
         "required": schema.get("required", []),
     }
 
 
 def get_llm_kwargs(function: dict) -> dict:
-    """Returns the kwargs for the LLMChain constructor.
+    """Return the kwargs for the LLMChain constructor.
 
     Args:
         function: The function to use.
 
     Returns:
         The kwargs for the LLMChain constructor.
     """
```

### Comparing `gigachain-0.1.9/langchain/chains/prompt_selector.py` & `gigachain-0.2.0/langchain/chains/prompt_selector.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/qa_generation/base.py` & `gigachain-0.2.0/langchain/chains/qa_generation/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import json
 from typing import Any, Dict, List, Optional
 
 from langchain_core.callbacks import CallbackManagerForChainRun
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.prompts import BasePromptTemplate
 from langchain_core.pydantic_v1 import Field
+from langchain_text_splitters import RecursiveCharacterTextSplitter, TextSplitter
 
 from langchain.chains.base import Chain
 from langchain.chains.llm import LLMChain
 from langchain.chains.qa_generation.prompt import PROMPT_SELECTOR
-from langchain.text_splitter import RecursiveCharacterTextSplitter, TextSplitter
 
 
 class QAGenerationChain(Chain):
     """Base class for question-answer generation chains."""
 
     llm_chain: LLMChain
     """LLM Chain that generates responses from user input and context."""
```

### Comparing `gigachain-0.1.9/langchain/chains/qa_generation/prompt.py` & `gigachain-0.2.0/langchain/chains/qa_generation/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/qa_with_sources/base.py` & `gigachain-0.2.0/langchain/chains/qa_with_sources/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         llm_question_chain = LLMChain(llm=llm, prompt=question_prompt)
         llm_combine_chain = LLMChain(llm=llm, prompt=combine_prompt)
         combine_results_chain = StuffDocumentsChain(
             llm_chain=llm_combine_chain,
             document_prompt=document_prompt,
             document_variable_name="summaries",
         )
-        reduce_documents_chain = ReduceDocumentsChain(
+        reduce_documents_chain = ReduceDocumentsChain(  # type: ignore[misc]
             combine_documents_chain=combine_results_chain
         )
         combine_documents_chain = MapReduceDocumentsChain(
             llm_chain=llm_question_chain,
             reduce_documents_chain=reduce_documents_chain,
             document_variable_name="context",
         )
```

### Comparing `gigachain-0.1.9/langchain/chains/qa_with_sources/loading.py` & `gigachain-0.2.0/langchain/chains/summarize/chain.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,183 +1,166 @@
-"""Load question answering with sources chains."""
-from __future__ import annotations
-
+"""Load summarizing chains."""
 from typing import Any, Mapping, Optional, Protocol
 
+from langchain_core.callbacks import Callbacks
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.prompts import BasePromptTemplate
 
 from langchain.chains.combine_documents.base import BaseCombineDocumentsChain
 from langchain.chains.combine_documents.map_reduce import MapReduceDocumentsChain
-from langchain.chains.combine_documents.map_rerank import MapRerankDocumentsChain
 from langchain.chains.combine_documents.reduce import ReduceDocumentsChain
 from langchain.chains.combine_documents.refine import RefineDocumentsChain
 from langchain.chains.combine_documents.stuff import StuffDocumentsChain
 from langchain.chains.llm import LLMChain
-from langchain.chains.qa_with_sources import (
-    map_reduce_prompt,
-    refine_prompts,
-    stuff_prompt,
-)
-from langchain.chains.question_answering.map_rerank_prompt import (
-    PROMPT as MAP_RERANK_PROMPT,
-)
+from langchain.chains.summarize import map_reduce_prompt, refine_prompts, stuff_prompt
 
 
 class LoadingCallable(Protocol):
     """Interface for loading the combine documents chain."""
 
     def __call__(
         self, llm: BaseLanguageModel, **kwargs: Any
     ) -> BaseCombineDocumentsChain:
         """Callable to load the combine documents chain."""
 
 
-def _load_map_rerank_chain(
-    llm: BaseLanguageModel,
-    prompt: BasePromptTemplate = MAP_RERANK_PROMPT,
-    verbose: bool = False,
-    document_variable_name: str = "context",
-    rank_key: str = "score",
-    answer_key: str = "answer",
-    **kwargs: Any,
-) -> MapRerankDocumentsChain:
-    llm_chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
-    return MapRerankDocumentsChain(
-        llm_chain=llm_chain,
-        rank_key=rank_key,
-        answer_key=answer_key,
-        document_variable_name=document_variable_name,
-        **kwargs,
-    )
-
-
 def _load_stuff_chain(
     llm: BaseLanguageModel,
     prompt: BasePromptTemplate = stuff_prompt.PROMPT,
-    document_prompt: BasePromptTemplate = stuff_prompt.EXAMPLE_PROMPT,
-    document_variable_name: str = "summaries",
+    document_variable_name: str = "text",
     verbose: Optional[bool] = None,
     **kwargs: Any,
 ) -> StuffDocumentsChain:
-    llm_chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
+    llm_chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)  # type: ignore[arg-type]
+    # TODO: document prompt
     return StuffDocumentsChain(
         llm_chain=llm_chain,
         document_variable_name=document_variable_name,
-        document_prompt=document_prompt,
-        verbose=verbose,
+        verbose=verbose,  # type: ignore[arg-type]
         **kwargs,
     )
 
 
 def _load_map_reduce_chain(
     llm: BaseLanguageModel,
-    question_prompt: BasePromptTemplate = map_reduce_prompt.QUESTION_PROMPT,
-    combine_prompt: BasePromptTemplate = map_reduce_prompt.COMBINE_PROMPT,
-    document_prompt: BasePromptTemplate = map_reduce_prompt.EXAMPLE_PROMPT,
-    combine_document_variable_name: str = "summaries",
-    map_reduce_document_variable_name: str = "context",
+    map_prompt: BasePromptTemplate = map_reduce_prompt.PROMPT,
+    combine_prompt: BasePromptTemplate = map_reduce_prompt.PROMPT,
+    combine_document_variable_name: str = "text",
+    map_reduce_document_variable_name: str = "text",
     collapse_prompt: Optional[BasePromptTemplate] = None,
     reduce_llm: Optional[BaseLanguageModel] = None,
     collapse_llm: Optional[BaseLanguageModel] = None,
     verbose: Optional[bool] = None,
     token_max: int = 3000,
+    callbacks: Callbacks = None,
+    *,
+    collapse_max_retries: Optional[int] = None,
     **kwargs: Any,
 ) -> MapReduceDocumentsChain:
-    map_chain = LLMChain(llm=llm, prompt=question_prompt, verbose=verbose)
+    map_chain = LLMChain(
+        llm=llm,
+        prompt=map_prompt,
+        verbose=verbose,  # type: ignore[arg-type]
+        callbacks=callbacks,  # type: ignore[arg-type]
+    )
     _reduce_llm = reduce_llm or llm
-    reduce_chain = LLMChain(llm=_reduce_llm, prompt=combine_prompt, verbose=verbose)
+    reduce_chain = LLMChain(
+        llm=_reduce_llm,
+        prompt=combine_prompt,
+        verbose=verbose,  # type: ignore[arg-type]
+        callbacks=callbacks,  # type: ignore[arg-type]
+    )
+    # TODO: document prompt
     combine_documents_chain = StuffDocumentsChain(
         llm_chain=reduce_chain,
         document_variable_name=combine_document_variable_name,
-        document_prompt=document_prompt,
-        verbose=verbose,
+        verbose=verbose,  # type: ignore[arg-type]
+        callbacks=callbacks,
     )
     if collapse_prompt is None:
         collapse_chain = None
         if collapse_llm is not None:
             raise ValueError(
                 "collapse_llm provided, but collapse_prompt was not: please "
                 "provide one or stop providing collapse_llm."
             )
     else:
         _collapse_llm = collapse_llm or llm
         collapse_chain = StuffDocumentsChain(
             llm_chain=LLMChain(
                 llm=_collapse_llm,
                 prompt=collapse_prompt,
-                verbose=verbose,
+                verbose=verbose,  # type: ignore[arg-type]
+                callbacks=callbacks,
             ),
             document_variable_name=combine_document_variable_name,
-            document_prompt=document_prompt,
         )
     reduce_documents_chain = ReduceDocumentsChain(
         combine_documents_chain=combine_documents_chain,
         collapse_documents_chain=collapse_chain,
         token_max=token_max,
-        verbose=verbose,
+        verbose=verbose,  # type: ignore[arg-type]
+        callbacks=callbacks,
+        collapse_max_retries=collapse_max_retries,
     )
     return MapReduceDocumentsChain(
         llm_chain=map_chain,
         reduce_documents_chain=reduce_documents_chain,
         document_variable_name=map_reduce_document_variable_name,
-        verbose=verbose,
+        verbose=verbose,  # type: ignore[arg-type]
+        callbacks=callbacks,
         **kwargs,
     )
 
 
 def _load_refine_chain(
     llm: BaseLanguageModel,
-    question_prompt: BasePromptTemplate = refine_prompts.DEFAULT_TEXT_QA_PROMPT,
-    refine_prompt: BasePromptTemplate = refine_prompts.DEFAULT_REFINE_PROMPT,
-    document_prompt: BasePromptTemplate = refine_prompts.EXAMPLE_PROMPT,
-    document_variable_name: str = "context_str",
+    question_prompt: BasePromptTemplate = refine_prompts.PROMPT,
+    refine_prompt: BasePromptTemplate = refine_prompts.REFINE_PROMPT,
+    document_variable_name: str = "text",
     initial_response_name: str = "existing_answer",
     refine_llm: Optional[BaseLanguageModel] = None,
     verbose: Optional[bool] = None,
     **kwargs: Any,
 ) -> RefineDocumentsChain:
-    initial_chain = LLMChain(llm=llm, prompt=question_prompt, verbose=verbose)
+    initial_chain = LLMChain(llm=llm, prompt=question_prompt, verbose=verbose)  # type: ignore[arg-type]
     _refine_llm = refine_llm or llm
-    refine_chain = LLMChain(llm=_refine_llm, prompt=refine_prompt, verbose=verbose)
+    refine_chain = LLMChain(llm=_refine_llm, prompt=refine_prompt, verbose=verbose)  # type: ignore[arg-type]
     return RefineDocumentsChain(
         initial_llm_chain=initial_chain,
         refine_llm_chain=refine_chain,
         document_variable_name=document_variable_name,
         initial_response_name=initial_response_name,
-        document_prompt=document_prompt,
-        verbose=verbose,
+        verbose=verbose,  # type: ignore[arg-type]
         **kwargs,
     )
 
 
-def load_qa_with_sources_chain(
+def load_summarize_chain(
     llm: BaseLanguageModel,
     chain_type: str = "stuff",
     verbose: Optional[bool] = None,
     **kwargs: Any,
 ) -> BaseCombineDocumentsChain:
-    """Load a question answering with sources chain.
+    """Load summarizing chain.
 
     Args:
         llm: Language Model to use in the chain.
         chain_type: Type of document combining chain to use. Should be one of "stuff",
-            "map_reduce", "refine" and "map_rerank".
+            "map_reduce", and "refine".
         verbose: Whether chains should be run in verbose mode or not. Note that this
             applies to all chains that make up the final chain.
 
     Returns:
-        A chain to use for question answering with sources.
+        A chain to use for summarizing.
     """
     loader_mapping: Mapping[str, LoadingCallable] = {
         "stuff": _load_stuff_chain,
         "map_reduce": _load_map_reduce_chain,
         "refine": _load_refine_chain,
-        "map_rerank": _load_map_rerank_chain,
     }
     if chain_type not in loader_mapping:
         raise ValueError(
             f"Got unsupported chain type: {chain_type}. "
             f"Should be one of {loader_mapping.keys()}"
         )
-    _func: LoadingCallable = loader_mapping[chain_type]
-    return _func(llm, verbose=verbose, **kwargs)
+    return loader_mapping[chain_type](llm, verbose=verbose, **kwargs)
```

### Comparing `gigachain-0.1.9/langchain/chains/qa_with_sources/map_reduce_prompt.py` & `gigachain-0.2.0/langchain/chains/qa_with_sources/map_reduce_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/qa_with_sources/refine_prompts.py` & `gigachain-0.2.0/langchain/chains/qa_with_sources/refine_prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/qa_with_sources/retrieval.py` & `gigachain-0.2.0/langchain/chains/qa_with_sources/retrieval.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,25 +42,25 @@
 
         return docs[:num_docs]
 
     def _get_docs(
         self, inputs: Dict[str, Any], *, run_manager: CallbackManagerForChainRun
     ) -> List[Document]:
         question = inputs[self.question_key]
-        docs = self.retriever.get_relevant_documents(
-            question, callbacks=run_manager.get_child()
+        docs = self.retriever.invoke(
+            question, config={"callbacks": run_manager.get_child()}
         )
         return self._reduce_tokens_below_limit(docs)
 
     async def _aget_docs(
         self, inputs: Dict[str, Any], *, run_manager: AsyncCallbackManagerForChainRun
     ) -> List[Document]:
         question = inputs[self.question_key]
-        docs = await self.retriever.aget_relevant_documents(
-            question, callbacks=run_manager.get_child()
+        docs = await self.retriever.ainvoke(
+            question, config={"callbacks": run_manager.get_child()}
         )
         return self._reduce_tokens_below_limit(docs)
 
     @property
     def _chain_type(self) -> str:
         """Return the chain type."""
         return "retrieval_qa_with_sources_chain"
```

### Comparing `gigachain-0.1.9/langchain/chains/qa_with_sources/stuff_prompt.py` & `gigachain-0.2.0/langchain/chains/qa_with_sources/stuff_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/qa_with_sources/vector_db.py` & `gigachain-0.2.0/langchain/chains/qa_with_sources/vector_db.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/query_constructor/base.py` & `gigachain-0.2.0/langchain/chains/query_constructor/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """LLM Chain for turning a user text query into a structured query."""
+
 from __future__ import annotations
 
 import json
 from typing import Any, Callable, List, Optional, Sequence, Tuple, Union, cast
 
 from langchain_core.exceptions import OutputParserException
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.output_parsers import BaseOutputParser
 from langchain_core.output_parsers.json import parse_and_check_json_markdown
 from langchain_core.prompts import BasePromptTemplate
 from langchain_core.prompts.few_shot import FewShotPromptTemplate
 from langchain_core.runnables import Runnable
-
-from langchain.chains.llm import LLMChain
-from langchain.chains.query_constructor.ir import (
+from langchain_core.structured_query import (
     Comparator,
     Comparison,
     FilterDirective,
     Operation,
     Operator,
     StructuredQuery,
 )
+
+from langchain.chains.llm import LLMChain
 from langchain.chains.query_constructor.parser import get_parser
 from langchain.chains.query_constructor.prompt import (
     DEFAULT_EXAMPLES,
     DEFAULT_PREFIX,
     DEFAULT_SCHEMA_PROMPT,
     DEFAULT_SUFFIX,
     EXAMPLE_PROMPT,
@@ -133,23 +134,26 @@
         if allowed_attributes and filter.attribute not in allowed_attributes:
             return None
         return filter
     elif isinstance(filter, Operation):
         if allowed_operators and filter.operator not in allowed_operators:
             return None
         args = [
-            fix_filter_directive(
-                arg,
-                allowed_comparators=allowed_comparators,
-                allowed_operators=allowed_operators,
-                allowed_attributes=allowed_attributes,
+            cast(
+                FilterDirective,
+                fix_filter_directive(
+                    arg,
+                    allowed_comparators=allowed_comparators,
+                    allowed_operators=allowed_operators,
+                    allowed_attributes=allowed_attributes,
+                ),
             )
             for arg in filter.arguments
+            if arg is not None
         ]
-        args = [arg for arg in args if arg is not None]
         if not args:
             return None
         elif len(args) == 1 and filter.operator in (Operator.AND, Operator.OR):
             return args[0]
         else:
             return Operation(
                 operator=filter.operator,
```

### Comparing `gigachain-0.1.9/langchain/chains/query_constructor/parser.py` & `gigachain-0.2.0/langchain/chains/query_constructor/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def v_args(*args: Any, **kwargs: Any) -> Any:  # type: ignore
         """Dummy decorator for when lark is not installed."""
         return lambda _: None
 
     Transformer = object  # type: ignore
     Lark = object  # type: ignore
 
-from langchain.chains.query_constructor.ir import (
+from langchain_core.structured_query import (
     Comparator,
     Comparison,
     FilterDirective,
     Operation,
     Operator,
 )
 
@@ -59,15 +59,15 @@
 
     date: str
     type: Literal["date"]
 
 
 @v_args(inline=True)
 class QueryTransformer(Transformer):
-    """Transforms a query string into an intermediate representation."""
+    """Transform a query string into an intermediate representation."""
 
     def __init__(
         self,
         *args: Any,
         allowed_comparators: Optional[Sequence[Comparator]] = None,
         allowed_operators: Optional[Sequence[Operator]] = None,
         allowed_attributes: Optional[Sequence[str]] = None,
@@ -155,16 +155,15 @@
 
 
 def get_parser(
     allowed_comparators: Optional[Sequence[Comparator]] = None,
     allowed_operators: Optional[Sequence[Operator]] = None,
     allowed_attributes: Optional[Sequence[str]] = None,
 ) -> Lark:
-    """
-    Returns a parser for the query language.
+    """Return a parser for the query language.
 
     Args:
         allowed_comparators: Optional[Sequence[Comparator]]
         allowed_operators: Optional[Sequence[Operator]]
 
     Returns:
         Lark parser for the query language.
```

### Comparing `gigachain-0.1.9/langchain/chains/query_constructor/prompt.py` & `gigachain-0.2.0/langchain/chains/query_constructor/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/question_answering/__init__.py` & `gigachain-0.2.0/langchain/chains/question_answering/chain.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,23 +69,23 @@
     callbacks: Callbacks = None,
     **kwargs: Any,
 ) -> StuffDocumentsChain:
     _prompt = prompt or stuff_prompt.PROMPT_SELECTOR.get_prompt(llm)
     llm_chain = LLMChain(
         llm=llm,
         prompt=_prompt,
-        verbose=verbose,
+        verbose=verbose,  # type: ignore[arg-type]
         callback_manager=callback_manager,
         callbacks=callbacks,
     )
     # TODO: document prompt
     return StuffDocumentsChain(
         llm_chain=llm_chain,
         document_variable_name=document_variable_name,
-        verbose=verbose,
+        verbose=verbose,  # type: ignore[arg-type]
         callback_manager=callback_manager,
         callbacks=callbacks,
         **kwargs,
     )
 
 
 def _load_map_reduce_chain(
@@ -108,31 +108,31 @@
     )
     _combine_prompt = (
         combine_prompt or map_reduce_prompt.COMBINE_PROMPT_SELECTOR.get_prompt(llm)
     )
     map_chain = LLMChain(
         llm=llm,
         prompt=_question_prompt,
-        verbose=verbose,
+        verbose=verbose,  # type: ignore[arg-type]
         callback_manager=callback_manager,
         callbacks=callbacks,
     )
     _reduce_llm = reduce_llm or llm
     reduce_chain = LLMChain(
         llm=_reduce_llm,
         prompt=_combine_prompt,
-        verbose=verbose,
+        verbose=verbose,  # type: ignore[arg-type]
         callback_manager=callback_manager,
         callbacks=callbacks,
     )
     # TODO: document prompt
     combine_documents_chain = StuffDocumentsChain(
         llm_chain=reduce_chain,
         document_variable_name=combine_document_variable_name,
-        verbose=verbose,
+        verbose=verbose,  # type: ignore[arg-type]
         callback_manager=callback_manager,
         callbacks=callbacks,
     )
     if collapse_prompt is None:
         collapse_chain = None
         if collapse_llm is not None:
             raise ValueError(
@@ -141,33 +141,33 @@
             )
     else:
         _collapse_llm = collapse_llm or llm
         collapse_chain = StuffDocumentsChain(
             llm_chain=LLMChain(
                 llm=_collapse_llm,
                 prompt=collapse_prompt,
-                verbose=verbose,
+                verbose=verbose,  # type: ignore[arg-type]
                 callback_manager=callback_manager,
                 callbacks=callbacks,
             ),
             document_variable_name=combine_document_variable_name,
-            verbose=verbose,
+            verbose=verbose,  # type: ignore[arg-type]
             callback_manager=callback_manager,
         )
-    reduce_documents_chain = ReduceDocumentsChain(
+    reduce_documents_chain = ReduceDocumentsChain(  # type: ignore[misc]
         combine_documents_chain=combine_documents_chain,
         collapse_documents_chain=collapse_chain,
         token_max=token_max,
         verbose=verbose,
     )
     return MapReduceDocumentsChain(
         llm_chain=map_chain,
         document_variable_name=map_reduce_document_variable_name,
         reduce_documents_chain=reduce_documents_chain,
-        verbose=verbose,
+        verbose=verbose,  # type: ignore[arg-type]
         callback_manager=callback_manager,
         callbacks=callbacks,
         **kwargs,
     )
 
 
 def _load_refine_chain(
@@ -187,32 +187,32 @@
     )
     _refine_prompt = refine_prompt or refine_prompts.REFINE_PROMPT_SELECTOR.get_prompt(
         llm
     )
     initial_chain = LLMChain(
         llm=llm,
         prompt=_question_prompt,
-        verbose=verbose,
+        verbose=verbose,  # type: ignore[arg-type]
         callback_manager=callback_manager,
         callbacks=callbacks,
     )
     _refine_llm = refine_llm or llm
     refine_chain = LLMChain(
         llm=_refine_llm,
         prompt=_refine_prompt,
-        verbose=verbose,
+        verbose=verbose,  # type: ignore[arg-type]
         callback_manager=callback_manager,
         callbacks=callbacks,
     )
     return RefineDocumentsChain(
         initial_llm_chain=initial_chain,
         refine_llm_chain=refine_chain,
         document_variable_name=document_variable_name,
         initial_response_name=initial_response_name,
-        verbose=verbose,
+        verbose=verbose,  # type: ignore[arg-type]
         callback_manager=callback_manager,
         callbacks=callbacks,
         **kwargs,
     )
 
 
 def load_qa_chain(
```

### Comparing `gigachain-0.1.9/langchain/chains/question_answering/map_reduce_prompt.py` & `gigachain-0.2.0/langchain/chains/question_answering/map_reduce_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/question_answering/map_rerank_prompt.py` & `gigachain-0.2.0/langchain/chains/question_answering/map_rerank_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/question_answering/refine_prompts.py` & `gigachain-0.2.0/langchain/chains/question_answering/refine_prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/question_answering/stuff_prompt.py` & `gigachain-0.2.0/langchain/chains/question_answering/stuff_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/retrieval.py` & `gigachain-0.2.0/langchain/chains/retrieval.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/retrieval_qa/prompt.py` & `gigachain-0.2.0/langchain/chains/retrieval_qa/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/router/base.py` & `gigachain-0.2.0/langchain/chains/router/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base classes for chain routing."""
+
 from __future__ import annotations
 
 from abc import ABC
 from typing import Any, Dict, List, Mapping, NamedTuple, Optional
 
 from langchain_core.callbacks import (
     AsyncCallbackManagerForChainRun,
```

### Comparing `gigachain-0.1.9/langchain/chains/router/embedding_router.py` & `gigachain-0.2.0/langchain/chains/router/embedding_router.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Type
 
-from langchain_core.callbacks import CallbackManagerForChainRun
+from langchain_core.callbacks import (
+    AsyncCallbackManagerForChainRun,
+    CallbackManagerForChainRun,
+)
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.pydantic_v1 import Extra
 from langchain_core.vectorstores import VectorStore
 
 from langchain.chains.router.base import RouterChain
 
@@ -36,14 +39,23 @@
         inputs: Dict[str, Any],
         run_manager: Optional[CallbackManagerForChainRun] = None,
     ) -> Dict[str, Any]:
         _input = ", ".join([inputs[k] for k in self.routing_keys])
         results = self.vectorstore.similarity_search(_input, k=1)
         return {"next_inputs": inputs, "destination": results[0].metadata["name"]}
 
+    async def _acall(
+        self,
+        inputs: Dict[str, Any],
+        run_manager: Optional[AsyncCallbackManagerForChainRun] = None,
+    ) -> Dict[str, Any]:
+        _input = ", ".join([inputs[k] for k in self.routing_keys])
+        results = await self.vectorstore.asimilarity_search(_input, k=1)
+        return {"next_inputs": inputs, "destination": results[0].metadata["name"]}
+
     @classmethod
     def from_names_and_descriptions(
         cls,
         names_and_descriptions: Sequence[Tuple[str, Sequence[str]]],
         vectorstore_cls: Type[VectorStore],
         embeddings: Embeddings,
         **kwargs: Any,
@@ -53,7 +65,25 @@
         for name, descriptions in names_and_descriptions:
             for description in descriptions:
                 documents.append(
                     Document(page_content=description, metadata={"name": name})
                 )
         vectorstore = vectorstore_cls.from_documents(documents, embeddings)
         return cls(vectorstore=vectorstore, **kwargs)
+
+    @classmethod
+    async def afrom_names_and_descriptions(
+        cls,
+        names_and_descriptions: Sequence[Tuple[str, Sequence[str]]],
+        vectorstore_cls: Type[VectorStore],
+        embeddings: Embeddings,
+        **kwargs: Any,
+    ) -> EmbeddingRouterChain:
+        """Convenience constructor."""
+        documents = []
+        for name, descriptions in names_and_descriptions:
+            for description in descriptions:
+                documents.append(
+                    Document(page_content=description, metadata={"name": name})
+                )
+        vectorstore = await vectorstore_cls.afrom_documents(documents, embeddings)
+        return cls(vectorstore=vectorstore, **kwargs)
```

### Comparing `gigachain-0.1.9/langchain/chains/router/llm_router.py` & `gigachain-0.2.0/langchain/chains/router/llm_router.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Base classes for LLM-powered router chains."""
+
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Type, cast
 
 from langchain_core.callbacks import (
     AsyncCallbackManagerForChainRun,
     CallbackManagerForChainRun,
 )
 from langchain_core.exceptions import OutputParserException
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.output_parsers import BaseOutputParser
 from langchain_core.prompts import BasePromptTemplate
 from langchain_core.pydantic_v1 import root_validator
+from langchain_core.utils.json import parse_and_check_json_markdown
 
 from langchain.chains import LLMChain
 from langchain.chains.router.base import RouterChain
-from langchain.output_parsers.json import parse_and_check_json_markdown
 
 
 class LLMRouterChain(RouterChain):
     """A router chain that uses an LLM chain to perform routing."""
 
     llm_chain: LLMChain
     """LLM chain used to perform routing"""
@@ -52,17 +53,19 @@
     def _call(
         self,
         inputs: Dict[str, Any],
         run_manager: Optional[CallbackManagerForChainRun] = None,
     ) -> Dict[str, Any]:
         _run_manager = run_manager or CallbackManagerForChainRun.get_noop_manager()
         callbacks = _run_manager.get_child()
+
+        prediction = self.llm_chain.predict(callbacks=callbacks, **inputs)
         output = cast(
             Dict[str, Any],
-            self.llm_chain.predict_and_parse(callbacks=callbacks, **inputs),
+            self.llm_chain.prompt.output_parser.parse(prediction),
         )
         return output
 
     async def _acall(
         self,
         inputs: Dict[str, Any],
         run_manager: Optional[AsyncCallbackManagerForChainRun] = None,
```

### Comparing `gigachain-0.1.9/langchain/chains/router/multi_prompt.py` & `gigachain-0.2.0/langchain/chains/router/multi_prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Use a single chain to route an input to one of multiple llm chains."""
+
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional
 
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.prompts import PromptTemplate
```

### Comparing `gigachain-0.1.9/langchain/chains/router/multi_prompt_prompt.py` & `gigachain-0.2.0/langchain/chains/router/multi_prompt_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/router/multi_retrieval_prompt.py` & `gigachain-0.2.0/langchain/chains/router/multi_retrieval_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/router/multi_retrieval_qa.py` & `gigachain-0.2.0/langchain/chains/router/multi_retrieval_qa.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Use a single chain to route an input to one of multiple retrieval qa chains."""
+
 from __future__ import annotations
 
 from typing import Any, Dict, List, Mapping, Optional
 
-from langchain_community.chat_models import ChatOpenAI
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.prompts import PromptTemplate
 from langchain_core.retrievers import BaseRetriever
 
 from langchain.chains import ConversationChain
 from langchain.chains.base import Chain
 from langchain.chains.conversation.prompt import DEFAULT_TEMPLATE
@@ -38,14 +38,16 @@
     def from_retrievers(
         cls,
         llm: BaseLanguageModel,
         retriever_infos: List[Dict[str, Any]],
         default_retriever: Optional[BaseRetriever] = None,
         default_prompt: Optional[PromptTemplate] = None,
         default_chain: Optional[Chain] = None,
+        *,
+        default_chain_llm: Optional[BaseLanguageModel] = None,
         **kwargs: Any,
     ) -> MultiRetrievalQAChain:
         if default_prompt and not default_retriever:
             raise ValueError(
                 "`default_retriever` must be specified if `default_prompt` is "
                 "provided. Received only `default_prompt`."
             )
@@ -74,16 +76,28 @@
                 llm, prompt=default_prompt, retriever=default_retriever
             )
         else:
             prompt_template = DEFAULT_TEMPLATE.replace("input", "query")
             prompt = PromptTemplate(
                 template=prompt_template, input_variables=["history", "query"]
             )
+            if default_chain_llm is None:
+                raise NotImplementedError(
+                    "conversation_llm must be provided if default_chain is not "
+                    "specified. This API has been changed to avoid instantiating "
+                    "default LLMs on behalf of users."
+                    "You can provide a conversation LLM like so:\n"
+                    "from langchain_openai import ChatOpenAI\n"
+                    "llm = ChatOpenAI()"
+                )
             _default_chain = ConversationChain(
-                llm=ChatOpenAI(), prompt=prompt, input_key="query", output_key="result"
+                llm=default_chain_llm,
+                prompt=prompt,
+                input_key="query",
+                output_key="result",
             )
         return cls(
             router_chain=router_chain,
             destination_chains=destination_chains,
             default_chain=_default_chain,
             **kwargs,
         )
```

### Comparing `gigachain-0.1.9/langchain/chains/sequential.py` & `gigachain-0.2.0/langchain/chains/sequential.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Chain pipeline where the outputs of one step feed directly into next."""
+
 from typing import Any, Dict, List, Optional
 
 from langchain_core.callbacks import (
     AsyncCallbackManagerForChainRun,
     CallbackManagerForChainRun,
 )
 from langchain_core.pydantic_v1 import Extra, root_validator
```

### Comparing `gigachain-0.1.9/langchain/chains/sql_database/prompt.py` & `gigachain-0.2.0/langchain/chains/sql_database/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/sql_database/query.py` & `gigachain-0.2.0/langchain/chains/sql_database/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-from typing import Any, Dict, List, Optional, TypedDict, Union
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, TypedDict, Union
 
-from langchain_community.utilities.sql_database import SQLDatabase
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.prompts import BasePromptTemplate
 from langchain_core.runnables import Runnable, RunnablePassthrough
 
 from langchain.chains.sql_database.prompt import PROMPT, SQL_PROMPTS
 
+if TYPE_CHECKING:
+    from langchain_community.utilities.sql_database import SQLDatabase
+
 
 def _strip(text: str) -> str:
     return text.strip()
 
 
 class SQLInput(TypedDict):
     """Input for a SQL Chain."""
```

### Comparing `gigachain-0.1.9/langchain/chains/structured_output/base.py` & `gigachain-0.2.0/langchain/chains/structured_output/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,70 @@
 import json
 from typing import Any, Callable, Dict, Literal, Optional, Sequence, Type, Union
 
+from langchain_core._api import deprecated
 from langchain_core.output_parsers import (
     BaseGenerationOutputParser,
     BaseOutputParser,
     JsonOutputParser,
+    PydanticOutputParser,
 )
 from langchain_core.output_parsers.openai_functions import (
     JsonOutputFunctionsParser,
     PydanticAttrOutputFunctionsParser,
     PydanticOutputFunctionsParser,
 )
+from langchain_core.output_parsers.openai_tools import (
+    JsonOutputKeyToolsParser,
+    PydanticToolsParser,
+)
 from langchain_core.prompts import BasePromptTemplate
 from langchain_core.pydantic_v1 import BaseModel
 from langchain_core.runnables import Runnable
 from langchain_core.utils.function_calling import (
     convert_to_openai_function,
     convert_to_openai_tool,
 )
 
-from langchain.output_parsers import (
-    JsonOutputKeyToolsParser,
-    PydanticOutputParser,
-    PydanticToolsParser,
-)
-
 
+@deprecated(
+    since="0.1.14",
+    message=(
+        "LangChain has introduced a method called `with_structured_output` that "
+        "is available on ChatModels capable of tool calling. "
+        "You can read more about the method here: "
+        "https://python.langchain.com/docs/modules/model_io/chat/structured_output/ "
+        "Please follow our extraction use case documentation for more guidelines "
+        "on how to do information extraction with LLMs. "
+        "https://python.langchain.com/docs/use_cases/extraction/. "
+        "If you notice other issues, please provide "
+        "feedback here: "
+        "https://github.com/langchain-ai/langchain/discussions/18154"
+    ),
+    removal="0.3.0",
+    alternative=(
+        """
+            from langchain_core.pydantic_v1 import BaseModel, Field
+            from langchain_anthropic import ChatAnthropic
+    
+            class Joke(BaseModel):
+                setup: str = Field(description="The setup of the joke")
+                punchline: str = Field(description="The punchline to the joke") 
+    
+            # Or any other chat model that supports tools.
+            # Please reference to to the documentation of structured_output
+            # to see an up to date list of which models support 
+            # with_structured_output.
+            model = ChatAnthropic(model="claude-3-opus-20240229", temperature=0)
+            structured_llm = model.with_structured_output(Joke)
+            structured_llm.invoke("Tell me a joke about cats. 
+                Make sure to call the Joke function.")
+            """
+    ),
+)
 def create_openai_fn_runnable(
     functions: Sequence[Union[Dict[str, Any], Type[BaseModel], Callable]],
     llm: Runnable,
     prompt: Optional[BasePromptTemplate] = None,
     *,
     enforce_single_function_usage: bool = True,
     output_parser: Optional[Union[BaseOutputParser, BaseGenerationOutputParser]] = None,
@@ -105,14 +140,49 @@
     output_parser = output_parser or get_openai_output_parser(functions)
     if prompt:
         return prompt | llm.bind(**llm_kwargs_) | output_parser
     else:
         return llm.bind(**llm_kwargs_) | output_parser
 
 
+@deprecated(
+    since="0.1.17",
+    message=(
+        "LangChain has introduced a method called `with_structured_output` that "
+        "is available on ChatModels capable of tool calling. "
+        "You can read more about the method here: "
+        "https://python.langchain.com/docs/modules/model_io/chat/structured_output/ "
+        "Please follow our extraction use case documentation for more guidelines "
+        "on how to do information extraction with LLMs. "
+        "https://python.langchain.com/docs/use_cases/extraction/. "
+        "If you notice other issues, please provide "
+        "feedback here: "
+        "https://github.com/langchain-ai/langchain/discussions/18154"
+    ),
+    removal="0.3.0",
+    alternative=(
+        """
+            from langchain_core.pydantic_v1 import BaseModel, Field
+            from langchain_anthropic import ChatAnthropic
+
+            class Joke(BaseModel):
+                setup: str = Field(description="The setup of the joke")
+                punchline: str = Field(description="The punchline to the joke") 
+
+            # Or any other chat model that supports tools.
+            # Please reference to to the documentation of structured_output
+            # to see an up to date list of which models support 
+            # with_structured_output.
+            model = ChatAnthropic(model="claude-3-opus-20240229", temperature=0)
+            structured_llm = model.with_structured_output(Joke)
+            structured_llm.invoke("Tell me a joke about cats. 
+                Make sure to call the Joke function.")
+            """
+    ),
+)
 def create_structured_output_runnable(
     output_schema: Union[Dict[str, Any], Type[BaseModel]],
     llm: Runnable,
     prompt: Optional[BasePromptTemplate] = None,
     *,
     output_parser: Optional[Union[BaseOutputParser, BaseGenerationOutputParser]] = None,
     enforce_function_usage: bool = True,
@@ -227,15 +297,15 @@
                         }
                     }
                 }
 
 
                 llm = ChatOpenAI(model="gpt-3.5-turbo-0125", temperature=0)
                 structured_llm = create_structured_output_runnable(
-                    doc_schema, 
+                    dog_schema, 
                     llm, 
                     mode="openai-tools", 
                     enforce_function_usage=True, 
                     return_single=True
                 )
                 structured_llm.invoke("Harry was a chubby brown beagle who loved chicken")
                 # -> {'name': 'Harry', 'color': 'brown', 'fav_food': 'chicken'}
@@ -473,23 +543,23 @@
     output_parser: Optional[Union[BaseOutputParser, BaseGenerationOutputParser]] = None,
     **llm_kwargs: Any,
 ) -> Runnable:
     if isinstance(output_schema, dict):
         function: Any = {
             "name": "output_formatter",
             "description": (
-                "Output formatter. Should always be used to format your response to the"
-                " user."
+                "Output formatter. Всегда используй его чтобы отформатировать свой"
+                " ответ пользователю."
             ),
             "parameters": output_schema,
         }
     else:
 
         class _OutputFormatter(BaseModel):
-            """Output formatter. Should always be used to format your response to the user."""  # noqa: E501
+            """Output formatter. Всегда используй его чтобы отформатировать свой ответ пользователю."""  # noqa: E501
 
             output: output_schema  # type: ignore
 
         function = _OutputFormatter
         output_parser = output_parser or PydanticAttrOutputFunctionsParser(
             pydantic_schema=_OutputFormatter, attr_name="output"
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gigachain-0.1.9/langchain/chains/summarize/__init__.py` & `gigachain-0.2.0/langchain/chains/qa_with_sources/loading.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,187 +1,184 @@
-"""Load summarizing chains."""
+"""Load question answering with sources chains."""
+
+from __future__ import annotations
+
 from typing import Any, Mapping, Optional, Protocol
 
-from langchain_core.callbacks import Callbacks
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.prompts import BasePromptTemplate
 
 from langchain.chains.combine_documents.base import BaseCombineDocumentsChain
-from langchain.chains.combine_documents.conditional import ConditionalDocumentsChain
 from langchain.chains.combine_documents.map_reduce import MapReduceDocumentsChain
+from langchain.chains.combine_documents.map_rerank import MapRerankDocumentsChain
 from langchain.chains.combine_documents.reduce import ReduceDocumentsChain
 from langchain.chains.combine_documents.refine import RefineDocumentsChain
 from langchain.chains.combine_documents.stuff import StuffDocumentsChain
 from langchain.chains.llm import LLMChain
-from langchain.chains.summarize import map_reduce_prompt, refine_prompts, stuff_prompt
+from langchain.chains.qa_with_sources import (
+    map_reduce_prompt,
+    refine_prompts,
+    stuff_prompt,
+)
+from langchain.chains.question_answering.map_rerank_prompt import (
+    PROMPT as MAP_RERANK_PROMPT,
+)
 
 
 class LoadingCallable(Protocol):
     """Interface for loading the combine documents chain."""
 
     def __call__(
         self, llm: BaseLanguageModel, **kwargs: Any
     ) -> BaseCombineDocumentsChain:
         """Callable to load the combine documents chain."""
 
 
+def _load_map_rerank_chain(
+    llm: BaseLanguageModel,
+    prompt: BasePromptTemplate = MAP_RERANK_PROMPT,
+    verbose: bool = False,
+    document_variable_name: str = "context",
+    rank_key: str = "score",
+    answer_key: str = "answer",
+    **kwargs: Any,
+) -> MapRerankDocumentsChain:
+    llm_chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
+    return MapRerankDocumentsChain(
+        llm_chain=llm_chain,
+        rank_key=rank_key,
+        answer_key=answer_key,
+        document_variable_name=document_variable_name,
+        **kwargs,
+    )
+
+
 def _load_stuff_chain(
     llm: BaseLanguageModel,
     prompt: BasePromptTemplate = stuff_prompt.PROMPT,
-    document_variable_name: str = "text",
+    document_prompt: BasePromptTemplate = stuff_prompt.EXAMPLE_PROMPT,
+    document_variable_name: str = "summaries",
     verbose: Optional[bool] = None,
     **kwargs: Any,
 ) -> StuffDocumentsChain:
-    llm_chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
-    # TODO: document prompt
+    llm_chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)  # type: ignore[arg-type]
     return StuffDocumentsChain(
         llm_chain=llm_chain,
         document_variable_name=document_variable_name,
-        verbose=verbose,
+        document_prompt=document_prompt,
+        verbose=verbose,  # type: ignore[arg-type]
         **kwargs,
     )
 
 
 def _load_map_reduce_chain(
     llm: BaseLanguageModel,
-    map_prompt: BasePromptTemplate = map_reduce_prompt.PROMPT,
-    combine_prompt: BasePromptTemplate = map_reduce_prompt.PROMPT,
-    combine_document_variable_name: str = "text",
-    map_reduce_document_variable_name: str = "text",
+    question_prompt: BasePromptTemplate = map_reduce_prompt.QUESTION_PROMPT,
+    combine_prompt: BasePromptTemplate = map_reduce_prompt.COMBINE_PROMPT,
+    document_prompt: BasePromptTemplate = map_reduce_prompt.EXAMPLE_PROMPT,
+    combine_document_variable_name: str = "summaries",
+    map_reduce_document_variable_name: str = "context",
     collapse_prompt: Optional[BasePromptTemplate] = None,
     reduce_llm: Optional[BaseLanguageModel] = None,
     collapse_llm: Optional[BaseLanguageModel] = None,
     verbose: Optional[bool] = None,
     token_max: int = 3000,
-    callbacks: Callbacks = None,
-    *,
-    collapse_max_retries: Optional[int] = None,
     **kwargs: Any,
 ) -> MapReduceDocumentsChain:
-    map_chain = LLMChain(
-        llm=llm, prompt=map_prompt, verbose=verbose, callbacks=callbacks
-    )
+    map_chain = LLMChain(llm=llm, prompt=question_prompt, verbose=verbose)  # type: ignore[arg-type]
     _reduce_llm = reduce_llm or llm
-    reduce_chain = LLMChain(
-        llm=_reduce_llm, prompt=combine_prompt, verbose=verbose, callbacks=callbacks
-    )
-    # TODO: document prompt
+    reduce_chain = LLMChain(llm=_reduce_llm, prompt=combine_prompt, verbose=verbose)  # type: ignore[arg-type]
     combine_documents_chain = StuffDocumentsChain(
         llm_chain=reduce_chain,
         document_variable_name=combine_document_variable_name,
-        verbose=verbose,
-        callbacks=callbacks,
+        document_prompt=document_prompt,
+        verbose=verbose,  # type: ignore[arg-type]
     )
     if collapse_prompt is None:
         collapse_chain = None
         if collapse_llm is not None:
             raise ValueError(
                 "collapse_llm provided, but collapse_prompt was not: please "
                 "provide one or stop providing collapse_llm."
             )
     else:
         _collapse_llm = collapse_llm or llm
         collapse_chain = StuffDocumentsChain(
             llm_chain=LLMChain(
                 llm=_collapse_llm,
                 prompt=collapse_prompt,
-                verbose=verbose,
-                callbacks=callbacks,
+                verbose=verbose,  # type: ignore[arg-type]
             ),
             document_variable_name=combine_document_variable_name,
+            document_prompt=document_prompt,
         )
     reduce_documents_chain = ReduceDocumentsChain(
         combine_documents_chain=combine_documents_chain,
         collapse_documents_chain=collapse_chain,
         token_max=token_max,
-        verbose=verbose,
-        callbacks=callbacks,
-        collapse_max_retries=collapse_max_retries,
+        verbose=verbose,  # type: ignore[arg-type]
     )
     return MapReduceDocumentsChain(
         llm_chain=map_chain,
         reduce_documents_chain=reduce_documents_chain,
         document_variable_name=map_reduce_document_variable_name,
-        verbose=verbose,
-        callbacks=callbacks,
+        verbose=verbose,  # type: ignore[arg-type]
         **kwargs,
     )
 
 
 def _load_refine_chain(
     llm: BaseLanguageModel,
-    question_prompt: BasePromptTemplate = refine_prompts.PROMPT,
-    refine_prompt: BasePromptTemplate = refine_prompts.REFINE_PROMPT,
-    document_variable_name: str = "text",
+    question_prompt: BasePromptTemplate = refine_prompts.DEFAULT_TEXT_QA_PROMPT,
+    refine_prompt: BasePromptTemplate = refine_prompts.DEFAULT_REFINE_PROMPT,
+    document_prompt: BasePromptTemplate = refine_prompts.EXAMPLE_PROMPT,
+    document_variable_name: str = "context_str",
     initial_response_name: str = "existing_answer",
     refine_llm: Optional[BaseLanguageModel] = None,
     verbose: Optional[bool] = None,
     **kwargs: Any,
 ) -> RefineDocumentsChain:
-    initial_chain = LLMChain(llm=llm, prompt=question_prompt, verbose=verbose)
+    initial_chain = LLMChain(llm=llm, prompt=question_prompt, verbose=verbose)  # type: ignore[arg-type]
     _refine_llm = refine_llm or llm
-    refine_chain = LLMChain(llm=_refine_llm, prompt=refine_prompt, verbose=verbose)
+    refine_chain = LLMChain(llm=_refine_llm, prompt=refine_prompt, verbose=verbose)  # type: ignore[arg-type]
     return RefineDocumentsChain(
         initial_llm_chain=initial_chain,
         refine_llm_chain=refine_chain,
         document_variable_name=document_variable_name,
         initial_response_name=initial_response_name,
-        verbose=verbose,
-        **kwargs,
-    )
-
-
-def _load_conditional_chain(
-    llm: BaseLanguageModel,
-    max_length: int = 3000,
-    verbose: Optional[bool] = None,
-    map_reduce_kwargs: Any = None,
-    stuff_kwargs: Any = None,
-    **kwargs: Any,
-) -> ConditionalDocumentsChain:
-    if stuff_kwargs is None:
-        stuff_kwargs = {}
-    if map_reduce_kwargs is None:
-        map_reduce_kwargs = {}
-    if verbose is not None:
-        stuff_kwargs["verbose"] = verbose
-        map_reduce_kwargs["verbose"] = verbose
-    stuff_chain = _load_stuff_chain(llm, **stuff_kwargs)
-    map_reduce_chain = _load_map_reduce_chain(llm, **map_reduce_kwargs)
-    return ConditionalDocumentsChain(
-        stuff_chain=stuff_chain,
-        map_reduce_chain=map_reduce_chain,
-        max_length=max_length,
+        document_prompt=document_prompt,
+        verbose=verbose,  # type: ignore[arg-type]
         **kwargs,
     )
 
 
-def load_summarize_chain(
+def load_qa_with_sources_chain(
     llm: BaseLanguageModel,
     chain_type: str = "stuff",
     verbose: Optional[bool] = None,
     **kwargs: Any,
 ) -> BaseCombineDocumentsChain:
-    """Load summarizing chain.
+    """Load a question answering with sources chain.
 
     Args:
         llm: Language Model to use in the chain.
         chain_type: Type of document combining chain to use. Should be one of "stuff",
-            "map_reduce", and "refine".
+            "map_reduce", "refine" and "map_rerank".
         verbose: Whether chains should be run in verbose mode or not. Note that this
             applies to all chains that make up the final chain.
 
     Returns:
-        A chain to use for summarizing.
+        A chain to use for question answering with sources.
     """
     loader_mapping: Mapping[str, LoadingCallable] = {
         "stuff": _load_stuff_chain,
         "map_reduce": _load_map_reduce_chain,
         "refine": _load_refine_chain,
-        "conditional": _load_conditional_chain,
+        "map_rerank": _load_map_rerank_chain,
     }
     if chain_type not in loader_mapping:
         raise ValueError(
             f"Got unsupported chain type: {chain_type}. "
             f"Should be one of {loader_mapping.keys()}"
         )
-    return loader_mapping[chain_type](llm, verbose=verbose, **kwargs)
+    _func: LoadingCallable = loader_mapping[chain_type]
+    return _func(llm, verbose=verbose, **kwargs)
```

### Comparing `gigachain-0.1.9/langchain/chains/summarize/refine_prompts.py` & `gigachain-0.2.0/langchain/chains/summarize/refine_prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/chains/transform.py` & `gigachain-0.2.0/langchain/chains/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Chain that runs an arbitrary python function."""
+
 import functools
 import logging
 from typing import Any, Awaitable, Callable, Dict, List, Optional
 
 from langchain_core.callbacks import (
     AsyncCallbackManagerForChainRun,
     CallbackManagerForChainRun,
```

### Comparing `gigachain-0.1.9/langchain/chat_models/__init__.py` & `gigachain-0.2.0/langchain/chat_models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 
 **Main helpers:**
 
 .. code-block::
 
     AIMessage, BaseMessage, HumanMessage
 """  # noqa: E501
+
 import warnings
 
 from langchain_core._api import LangChainDeprecationWarning
 
-from langchain.utils.interactive_env import is_interactive_env
+from langchain._api.interactive_env import is_interactive_env
 
 
 def __getattr__(name: str) -> None:
     from langchain_community import chat_models
 
     # If not in interactive env, raise warning.
     if not is_interactive_env():
```

### Comparing `gigachain-0.1.9/langchain/docstore/__init__.py` & `gigachain-0.2.0/langchain/docstore/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,33 +10,38 @@
 
 **Main helpers:**
 
 .. code-block::
 
     Document, AddableMixin
 """
-import warnings
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
-from langchain_core._api import LangChainDeprecationWarning
+from langchain._api import create_importer
 
-from langchain.utils.interactive_env import is_interactive_env
+if TYPE_CHECKING:
+    from langchain_community.docstore.arbitrary_fn import DocstoreFn
+    from langchain_community.docstore.in_memory import InMemoryDocstore
+    from langchain_community.docstore.wikipedia import Wikipedia
+
+# Create a way to dynamically look up deprecated imports.
+# Used to consolidate logic for raising deprecation warnings and
+# handling optional imports.
+DEPRECATED_LOOKUP = {
+    "DocstoreFn": "langchain_community.docstore.arbitrary_fn",
+    "InMemoryDocstore": "langchain_community.docstore.in_memory",
+    "Wikipedia": "langchain_community.docstore.wikipedia",
+}
 
+_import_attribute = create_importer(__package__, deprecated_lookups=DEPRECATED_LOOKUP)
 
-def __getattr__(name: str) -> Any:
-    from langchain_community import docstore
-
-    # If not in interactive env, raise warning.
-    if not is_interactive_env():
-        warnings.warn(
-            "Importing docstores from langchain is deprecated. Importing from "
-            "langchain will no longer be supported as of langchain==0.2.0. "
-            "Please import from langchain-community instead:\n\n"
-            f"`from langchain_community.docstore import {name}`.\n\n"
-            "To install gigachain-community run `pip install -U gigachain-community`.",
-            category=LangChainDeprecationWarning,
-        )
 
-    return getattr(docstore, name)
+def __getattr__(name: str) -> Any:
+    """Look up attributes dynamically."""
+    return _import_attribute(name)
 
 
-__all__ = ["DocstoreFn", "InMemoryDocstore", "Wikipedia"]
+__all__ = [
+    "DocstoreFn",
+    "InMemoryDocstore",
+    "Wikipedia",
+]
```

### Comparing `gigachain-0.1.9/langchain/document_transformers/loading.py` & `gigachain-0.2.0/langchain/document_transformers/loading.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/document_transformers/serializers.py` & `gigachain-0.2.0/langchain/document_transformers/serializers.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/document_transformers/xsl/html_chunks_with_headers.xslt` & `gigachain-0.2.0/langchain/document_transformers/xsl/html_chunks_with_headers.xslt`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/evaluation/__init__.py` & `gigachain-0.2.0/langchain/evaluation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,28 +34,29 @@
 
 **Some common use cases for evaluation include:**
 
 - Grading the accuracy of a response against ground truth answers: :class:`QAEvalChain <langchain.evaluation.qa.eval_chain.QAEvalChain>`
 - Comparing the output of two models: :class:`PairwiseStringEvalChain <langchain.evaluation.comparison.eval_chain.PairwiseStringEvalChain>` or :class:`LabeledPairwiseStringEvalChain <langchain.evaluation.comparison.eval_chain.LabeledPairwiseStringEvalChain>` when there is additionally a reference label.
 - Judging the efficacy of an agent's tool usage: :class:`TrajectoryEvalChain <langchain.evaluation.agents.trajectory_eval_chain.TrajectoryEvalChain>`
 - Checking whether an output complies with a set of criteria: :class:`CriteriaEvalChain <langchain.evaluation.criteria.eval_chain.CriteriaEvalChain>` or :class:`LabeledCriteriaEvalChain <langchain.evaluation.criteria.eval_chain.LabeledCriteriaEvalChain>` when there is additionally a reference label.
-- Computing semantic difference between a prediction and reference: :class:`EmbeddingDistanceEvalChain <langchain.evaluation.embedding_distance.base.EmbeddingDistanceEvalChain>` or between two predictions: :class:`PairwiseEmbeddingDistanceEvalChain <langchain.evaluation.embedding_distance.base.PairwiseEmbeddingDistanceEvalChain>` 
+- Computing semantic difference between a prediction and reference: :class:`EmbeddingDistanceEvalChain <langchain.evaluation.embedding_distance.base.EmbeddingDistanceEvalChain>` or between two predictions: :class:`PairwiseEmbeddingDistanceEvalChain <langchain.evaluation.embedding_distance.base.PairwiseEmbeddingDistanceEvalChain>`
 - Measuring the string distance between a prediction and reference :class:`StringDistanceEvalChain <langchain.evaluation.string_distance.base.StringDistanceEvalChain>` or between two predictions :class:`PairwiseStringDistanceEvalChain <langchain.evaluation.string_distance.base.PairwiseStringDistanceEvalChain>`
 
 **Low-level API**
 
 These evaluators implement one of the following interfaces:
 
 - :class:`StringEvaluator <langchain.evaluation.schema.StringEvaluator>`: Evaluate a prediction string against a reference label and/or input context.
 - :class:`PairwiseStringEvaluator <langchain.evaluation.schema.PairwiseStringEvaluator>`: Evaluate two prediction strings against each other. Useful for scoring preferences, measuring similarity between two chain or llm agents, or comparing outputs on similar inputs.
 - :class:`AgentTrajectoryEvaluator <langchain.evaluation.schema.AgentTrajectoryEvaluator>` Evaluate the full sequence of actions taken by an agent.
 
 These interfaces enable easier composability and usage within a higher level evaluation framework.
 
 """  # noqa: E501
+
 from langchain.evaluation.agents import TrajectoryEvalChain
 from langchain.evaluation.comparison import (
     LabeledPairwiseStringEvalChain,
     PairwiseStringEvalChain,
 )
 from langchain.evaluation.criteria import (
     Criteria,
```

### Comparing `gigachain-0.1.9/langchain/evaluation/agents/trajectory_eval_chain.py` & `gigachain-0.2.0/langchain/evaluation/agents/trajectory_eval_chain.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,26 +15,26 @@
     Tuple,
     TypedDict,
     Union,
     cast,
 )
 
 from langchain_core.agents import AgentAction
+from langchain_core.callbacks.manager import (
+    AsyncCallbackManagerForChainRun,
+    CallbackManagerForChainRun,
+    Callbacks,
+)
 from langchain_core.exceptions import OutputParserException
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.language_models.chat_models import BaseChatModel
 from langchain_core.output_parsers import BaseOutputParser
 from langchain_core.pydantic_v1 import Extra, Field
 from langchain_core.tools import BaseTool
 
-from langchain.callbacks.manager import (
-    AsyncCallbackManagerForChainRun,
-    CallbackManagerForChainRun,
-    Callbacks,
-)
 from langchain.chains.llm import LLMChain
 from langchain.evaluation.agents.trajectory_eval_prompt import (
     EVAL_CHAT_PROMPT,
     TOOL_FREE_EVAL_CHAT_PROMPT,
 )
 from langchain.evaluation.schema import AgentTrajectoryEvaluator, LLMEvalChain
 
@@ -251,15 +251,15 @@
             )
         if agent_tools:
             prompt = EVAL_CHAT_PROMPT
         else:
             prompt = TOOL_FREE_EVAL_CHAT_PROMPT
         eval_chain = LLMChain(llm=llm, prompt=prompt)
         return cls(
-            agent_tools=agent_tools,
+            agent_tools=agent_tools,  # type: ignore[arg-type]
             eval_chain=eval_chain,
             output_parser=output_parser or TrajectoryOutputParser(),
             **kwargs,
         )
 
     @property
     def input_keys(self) -> List[str]:
```

### Comparing `gigachain-0.1.9/langchain/evaluation/agents/trajectory_eval_prompt.py` & `gigachain-0.2.0/langchain/evaluation/agents/trajectory_eval_prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Prompt for trajectory evaluation chain."""
+
 # flake8: noqa
 from langchain_core.messages import HumanMessage, AIMessage, SystemMessage
 
 from langchain_core.prompts.chat import (
     ChatPromptTemplate,
     HumanMessagePromptTemplate,
 )
```

### Comparing `gigachain-0.1.9/langchain/evaluation/comparison/__init__.py` & `gigachain-0.2.0/langchain/evaluation/comparison/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,13 +23,14 @@
     #    "value": "B",
     #    "comment": "Both responses accurately state"
     #       " that the chemical formula for water is H2O."
     #       " However, Response B provides additional information"
     # .     " by explaining what the formula means.\\n[[B]]"
     # }
 """
+
 from langchain.evaluation.comparison.eval_chain import (
     LabeledPairwiseStringEvalChain,
     PairwiseStringEvalChain,
 )
 
 __all__ = ["PairwiseStringEvalChain", "LabeledPairwiseStringEvalChain"]
```

### Comparing `gigachain-0.1.9/langchain/evaluation/comparison/eval_chain.py` & `gigachain-0.2.0/langchain/evaluation/comparison/eval_chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Base classes for comparing the output of two models."""
+
 from __future__ import annotations
 
 import logging
 import re
 from typing import Any, Dict, List, Optional, Union
 
-from langchain_community.chat_models.azure_openai import AzureChatOpenAI
-from langchain_community.chat_models.openai import ChatOpenAI
+from langchain_core.callbacks.manager import Callbacks
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.output_parsers import BaseOutputParser
 from langchain_core.prompts.prompt import PromptTemplate
 from langchain_core.pydantic_v1 import Extra, Field
 
-from langchain.callbacks.manager import Callbacks
 from langchain.chains.constitutional_ai.models import ConstitutionalPrinciple
 from langchain.chains.llm import LLMChain
 from langchain.evaluation.comparison.prompt import (
     COMPARISON_TEMPLATE,
     COMPARISON_TEMPLATE_WITH_REFERENCE,
     CRITERIA_INSTRUCTIONS,
 )
@@ -250,18 +249,16 @@
         Returns:
             PairwiseStringEvalChain: The initialized PairwiseStringEvalChain.
 
         Raises:
             ValueError: If the input variables are not as expected.
 
         """
-        if not (
-            isinstance(llm, (ChatOpenAI, AzureChatOpenAI))
-            and llm.model_name.startswith("gpt-4")
-        ):
+        # Check if the model is GPT-4 if not raise a warning
+        if not hasattr(llm, "model_name") or not llm.model_name.startswith("gpt-4"):
             logger.warning(
                 "This chain was only tested with GPT-4. \
 Performance may be significantly worse with other models."
             )
 
         expected_input_vars = {"prediction", "prediction_b", "input", "criteria"}
         prompt_ = prompt or COMPARISON_TEMPLATE.partial(reference="")
```

### Comparing `gigachain-0.1.9/langchain/evaluation/comparison/prompt.py` & `gigachain-0.2.0/langchain/evaluation/comparison/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Prompts for comparing the outputs of two models for a given question.
 
 This prompt is used to compare two responses and evaluate which one best follows the instructions
 and answers the question. The prompt is based on the paper from
 Zheng, et. al. https://arxiv.org/abs/2306.05685
 """
+
 # flake8: noqa
 from langchain_core.prompts.chat import ChatPromptTemplate
 
 SYSTEM_MESSAGE = 'Please act as an impartial judge and evaluate the quality \
 of the responses provided by two AI assistants to the user question displayed below. \
 You should choose the assistant that follows the user\'s instructions \
 and answers \the user\'s question better. \
```

### Comparing `gigachain-0.1.9/langchain/evaluation/criteria/__init__.py` & `gigachain-0.2.0/langchain/evaluation/criteria/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/evaluation/criteria/eval_chain.py` & `gigachain-0.2.0/langchain/evaluation/criteria/eval_chain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 import re
 from enum import Enum
 from typing import Any, Dict, List, Mapping, Optional, Union
 
+from langchain_core.callbacks.manager import Callbacks
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.output_parsers import BaseOutputParser
 from langchain_core.prompts import BasePromptTemplate
 from langchain_core.pydantic_v1 import Extra, Field
 
-from langchain.callbacks.manager import Callbacks
 from langchain.chains.constitutional_ai.models import ConstitutionalPrinciple
 from langchain.chains.llm import LLMChain
 from langchain.evaluation.criteria.prompt import PROMPT, PROMPT_WITH_REFERENCES
 from langchain.evaluation.schema import LLMEvalChain, StringEvaluator
 from langchain.schema import RUN_KEY
 
 
@@ -189,27 +189,27 @@
     Returns
     -------
     CriteriaEvalChain
         An instance of the `CriteriaEvalChain` class.
 
     Examples
     --------
-    >>> from langchain_community.chat_models import ChatAnthropic
+    >>> from langchain_anthropic import ChatAnthropic
     >>> from langchain.evaluation.criteria import CriteriaEvalChain
     >>> llm = ChatAnthropic(temperature=0)
     >>> criteria = {"my-custom-criterion": "Is the submission the most amazing ever?"}
     >>> evaluator = CriteriaEvalChain.from_llm(llm=llm, criteria=criteria)
     >>> evaluator.evaluate_strings(prediction="Imagine an ice cream flavor for the color aquamarine", input="Tell me an idea")
     {
         'reasoning': 'Here is my step-by-step reasoning for the given criteria:\\n\\nThe criterion is: "Is the submission the most amazing ever?" This is a subjective criterion and open to interpretation. The submission suggests an aquamarine-colored ice cream flavor which is creative but may or may not be considered the most amazing idea ever conceived. There are many possible amazing ideas and this one ice cream flavor suggestion may or may not rise to that level for every person. \\n\\nN',
         'value': 'N',
         'score': 0,
     }
 
-    >>> from langchain_community.chat_models import ChatOpenAI
+    >>> from langchain_openai import ChatOpenAI
     >>> from langchain.evaluation.criteria import LabeledCriteriaEvalChain
     >>> llm = ChatOpenAI(model="gpt-4", temperature=0)
     >>> criteria = "correctness"
     >>> evaluator = LabeledCriteriaEvalChain.from_llm(
     ...     llm=llm,
     ...     criteria=criteria,
     ... )
@@ -340,15 +340,15 @@
         Returns
         -------
         CriteriaEvalChain
             An instance of the `CriteriaEvalChain` class.
 
         Examples
         --------
-        >>> from langchain_community.llms import OpenAI
+        >>> from langchain_openai import OpenAI
         >>> from langchain.evaluation.criteria import LabeledCriteriaEvalChain
         >>> llm = OpenAI()
         >>> criteria = {
                 "hallucination": (
                     "Does this submission contain information"
                     " not present in the input or reference?"
                 ),
@@ -428,15 +428,15 @@
         Returns
         -------
         dict
             The evaluation results.
 
         Examples
         --------
-        >>> from langchain_community.llms import OpenAI
+        >>> from langchain_openai import OpenAI
         >>> from langchain.evaluation.criteria import CriteriaEvalChain
         >>> llm = OpenAI()
         >>> criteria = "conciseness"
         >>> chain = CriteriaEvalChain.from_llm(llm=llm, criteria=criteria)
         >>> chain.evaluate_strings(
                 prediction="The answer is 42.",
                 reference="42",
@@ -483,15 +483,15 @@
         Returns
         -------
         dict
             The evaluation results.
 
         Examples
         --------
-        >>> from langchain_community.llms import OpenAI
+        >>> from langchain_openai import OpenAI
         >>> from langchain.evaluation.criteria import CriteriaEvalChain
         >>> llm = OpenAI()
         >>> criteria = "conciseness"
         >>> chain = CriteriaEvalChain.from_llm(llm=llm, criteria=criteria)
         >>> await chain.aevaluate_strings(
                 prediction="The answer is 42.",
                 reference="42",
@@ -564,15 +564,15 @@
         Returns
         -------
         LabeledCriteriaEvalChain
             An instance of the `LabeledCriteriaEvalChain` class.
 
         Examples
         --------
-        >>> from langchain_community.llms import OpenAI
+        >>> from langchain_openai import OpenAI
         >>> from langchain.evaluation.criteria import LabeledCriteriaEvalChain
         >>> llm = OpenAI()
         >>> criteria = {
                 "hallucination": (
                     "Does this submission contain information"
                     " not present in the input or reference?"
                 ),
```

### Comparing `gigachain-0.1.9/langchain/evaluation/criteria/prompt.py` & `gigachain-0.2.0/langchain/evaluation/criteria/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/evaluation/embedding_distance/base.py` & `gigachain-0.2.0/langchain/evaluation/string_distance/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,440 +1,424 @@
-"""A chain for comparing the output of two models using embeddings."""
-from enum import Enum
-from typing import Any, Dict, List, Optional
+"""String distance evaluators based on the RapidFuzz library."""
 
-import numpy as np
-from langchain_community.embeddings.openai import OpenAIEmbeddings
-from langchain_core.embeddings import Embeddings
-from langchain_core.pydantic_v1 import Field, root_validator
+from enum import Enum
+from typing import Any, Callable, Dict, List, Optional
 
-from langchain.callbacks.manager import (
+from langchain_core.callbacks.manager import (
     AsyncCallbackManagerForChainRun,
     CallbackManagerForChainRun,
     Callbacks,
 )
+from langchain_core.pydantic_v1 import Field, root_validator
+
 from langchain.chains.base import Chain
 from langchain.evaluation.schema import PairwiseStringEvaluator, StringEvaluator
 from langchain.schema import RUN_KEY
-from langchain.utils.math import cosine_similarity
-
 
-class EmbeddingDistance(str, Enum):
-    """Embedding Distance Metric.
 
-    Attributes:
-        COSINE: Cosine distance metric.
-        EUCLIDEAN: Euclidean distance metric.
-        MANHATTAN: Manhattan distance metric.
-        CHEBYSHEV: Chebyshev distance metric.
-        HAMMING: Hamming distance metric.
+def _load_rapidfuzz() -> Any:
     """
+    Load the RapidFuzz library.
 
-    COSINE = "cosine"
-    EUCLIDEAN = "euclidean"
-    MANHATTAN = "manhattan"
-    CHEBYSHEV = "chebyshev"
-    HAMMING = "hamming"
+    Raises:
+        ImportError: If the rapidfuzz library is not installed.
+
+    Returns:
+        Any: The rapidfuzz.distance module.
+    """
+    try:
+        import rapidfuzz
+    except ImportError:
+        raise ImportError(
+            "Please install the rapidfuzz library to use the FuzzyMatchStringEvaluator."
+            "Please install it with `pip install rapidfuzz`."
+        )
+    return rapidfuzz.distance
 
 
-class _EmbeddingDistanceChainMixin(Chain):
-    """Shared functionality for embedding distance evaluators.
+class StringDistance(str, Enum):
+    """Distance metric to use.
 
     Attributes:
-        embeddings (Embeddings): The embedding objects to vectorize the outputs.
-        distance_metric (EmbeddingDistance): The distance metric to use
-                                            for comparing the embeddings.
+        DAMERAU_LEVENSHTEIN: The Damerau-Levenshtein distance.
+        LEVENSHTEIN: The Levenshtein distance.
+        JARO: The Jaro distance.
+        JARO_WINKLER: The Jaro-Winkler distance.
+        HAMMING: The Hamming distance.
+        INDEL: The Indel distance.
     """
 
-    embeddings: Embeddings = Field(default_factory=OpenAIEmbeddings)
-    distance_metric: EmbeddingDistance = Field(default=EmbeddingDistance.COSINE)
+    DAMERAU_LEVENSHTEIN = "damerau_levenshtein"
+    LEVENSHTEIN = "levenshtein"
+    JARO = "jaro"
+    JARO_WINKLER = "jaro_winkler"
+    HAMMING = "hamming"
+    INDEL = "indel"
+
+
+class _RapidFuzzChainMixin(Chain):
+    """Shared methods for the rapidfuzz string distance evaluators."""
+
+    distance: StringDistance = Field(default=StringDistance.JARO_WINKLER)
+    normalize_score: bool = Field(default=True)
+    """Whether to normalize the score to a value between 0 and 1.
+    Applies only to the Levenshtein and Damerau-Levenshtein distances."""
 
-    @root_validator(pre=False)
-    def _validate_tiktoken_installed(cls, values: Dict[str, Any]) -> Dict[str, Any]:
-        """Validate that the TikTok library is installed.
+    @root_validator
+    def validate_dependencies(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+        """
+        Validate that the rapidfuzz library is installed.
 
         Args:
-            values (Dict[str, Any]): The values to validate.
+            values (Dict[str, Any]): The input values.
 
         Returns:
             Dict[str, Any]: The validated values.
         """
-        embeddings = values.get("embeddings")
-        if isinstance(embeddings, OpenAIEmbeddings):
-            try:
-                import tiktoken  # noqa: F401
-            except ImportError:
-                raise ImportError(
-                    "The tiktoken library is required to use the default "
-                    "OpenAI embeddings with embedding distance evaluators."
-                    " Please either manually select a different Embeddings object"
-                    " or install tiktoken using `pip install tiktoken`."
-                )
+        _load_rapidfuzz()
         return values
 
-    class Config:
-        """Permit embeddings to go unvalidated."""
-
-        arbitrary_types_allowed: bool = True
-
     @property
     def output_keys(self) -> List[str]:
-        """Return the output keys of the chain.
+        """
+        Get the output keys.
 
         Returns:
             List[str]: The output keys.
         """
         return ["score"]
 
-    def _prepare_output(self, result: dict) -> dict:
-        parsed = {"score": result["score"]}
-        if RUN_KEY in result:
-            parsed[RUN_KEY] = result[RUN_KEY]
-        return parsed
-
-    def _get_metric(self, metric: EmbeddingDistance) -> Any:
-        """Get the metric function for the given metric name.
-
-        Args:
-            metric (EmbeddingDistance): The metric name.
-
-        Returns:
-            Any: The metric function.
+    def _prepare_output(self, result: Dict[str, Any]) -> Dict[str, Any]:
         """
-        metrics = {
-            EmbeddingDistance.COSINE: self._cosine_distance,
-            EmbeddingDistance.EUCLIDEAN: self._euclidean_distance,
-            EmbeddingDistance.MANHATTAN: self._manhattan_distance,
-            EmbeddingDistance.CHEBYSHEV: self._chebyshev_distance,
-            EmbeddingDistance.HAMMING: self._hamming_distance,
-        }
-        if metric in metrics:
-            return metrics[metric]
-        else:
-            raise ValueError(f"Invalid metric: {metric}")
-
-    @staticmethod
-    def _cosine_distance(a: np.ndarray, b: np.ndarray) -> np.ndarray:
-        """Compute the cosine distance between two vectors.
+        Prepare the output dictionary.
 
         Args:
-            a (np.ndarray): The first vector.
-            b (np.ndarray): The second vector.
+            result (Dict[str, Any]): The evaluation results.
 
         Returns:
-            np.ndarray: The cosine distance.
+            Dict[str, Any]: The prepared output dictionary.
         """
-        return 1.0 - cosine_similarity(a, b)
+        result = {"score": result["score"]}
+        if RUN_KEY in result:
+            result[RUN_KEY] = result[RUN_KEY].dict()
+        return result
 
     @staticmethod
-    def _euclidean_distance(a: np.ndarray, b: np.ndarray) -> np.floating:
-        """Compute the Euclidean distance between two vectors.
-
-        Args:
-            a (np.ndarray): The first vector.
-            b (np.ndarray): The second vector.
-
-        Returns:
-            np.floating: The Euclidean distance.
+    def _get_metric(distance: str, normalize_score: bool = False) -> Callable:
         """
-        return np.linalg.norm(a - b)
-
-    @staticmethod
-    def _manhattan_distance(a: np.ndarray, b: np.ndarray) -> np.floating:
-        """Compute the Manhattan distance between two vectors.
+        Get the distance metric function based on the distance type.
 
         Args:
-            a (np.ndarray): The first vector.
-            b (np.ndarray): The second vector.
+            distance (str): The distance type.
 
         Returns:
-            np.floating: The Manhattan distance.
+            Callable: The distance metric function.
+
+        Raises:
+            ValueError: If the distance metric is invalid.
         """
-        return np.sum(np.abs(a - b))
+        from rapidfuzz import distance as rf_distance
 
-    @staticmethod
-    def _chebyshev_distance(a: np.ndarray, b: np.ndarray) -> np.floating:
-        """Compute the Chebyshev distance between two vectors.
+        module_map: Dict[str, Any] = {
+            StringDistance.DAMERAU_LEVENSHTEIN: rf_distance.DamerauLevenshtein,
+            StringDistance.LEVENSHTEIN: rf_distance.Levenshtein,
+            StringDistance.JARO: rf_distance.Jaro,
+            StringDistance.JARO_WINKLER: rf_distance.JaroWinkler,
+            StringDistance.HAMMING: rf_distance.Hamming,
+            StringDistance.INDEL: rf_distance.Indel,
+        }
+        if distance not in module_map:
+            raise ValueError(
+                f"Invalid distance metric: {distance}"
+                f"\nMust be one of: {list(StringDistance)}"
+            )
+        module = module_map[distance]
+        if normalize_score:
+            return module.normalized_distance
+        else:
+            return module.distance
 
-        Args:
-            a (np.ndarray): The first vector.
-            b (np.ndarray): The second vector.
+    @property
+    def metric(self) -> Callable:
+        """
+        Get the distance metric function.
 
         Returns:
-            np.floating: The Chebyshev distance.
+            Callable: The distance metric function.
         """
-        return np.max(np.abs(a - b))
+        return _RapidFuzzChainMixin._get_metric(
+            self.distance, normalize_score=self.normalize_score
+        )
 
-    @staticmethod
-    def _hamming_distance(a: np.ndarray, b: np.ndarray) -> np.floating:
-        """Compute the Hamming distance between two vectors.
+    def compute_metric(self, a: str, b: str) -> float:
+        """
+        Compute the distance between two strings.
 
         Args:
-            a (np.ndarray): The first vector.
-            b (np.ndarray): The second vector.
+            a (str): The first string.
+            b (str): The second string.
 
         Returns:
-            np.floating: The Hamming distance.
+            float: The distance between the two strings.
         """
-        return np.mean(a != b)
+        return self.metric(a, b)
 
-    def _compute_score(self, vectors: np.ndarray) -> float:
-        """Compute the score based on the distance metric.
 
-        Args:
-            vectors (np.ndarray): The input vectors.
+class StringDistanceEvalChain(StringEvaluator, _RapidFuzzChainMixin):
+    """Compute string distances between the prediction and the reference.
 
-        Returns:
-            float: The computed score.
-        """
-        metric = self._get_metric(self.distance_metric)
-        score = metric(vectors[0].reshape(1, -1), vectors[1].reshape(1, -1)).item()
-        return score
+    Examples
+    ----------
 
+    >>> from langchain.evaluation import StringDistanceEvalChain
+    >>> evaluator = StringDistanceEvalChain()
+    >>> evaluator.evaluate_strings(
+            prediction="Mindy is the CTO",
+            reference="Mindy is the CEO",
+        )
 
-class EmbeddingDistanceEvalChain(_EmbeddingDistanceChainMixin, StringEvaluator):
-    """Use embedding distances to score semantic difference between
-    a prediction and reference.
+    Using the `load_evaluator` function:
 
-    Examples:
-        >>> chain = EmbeddingDistanceEvalChain()
-        >>> result = chain.evaluate_strings(prediction="Hello", reference="Hi")
-        >>> print(result)
-        {'score': 0.5}
+    >>> from langchain.evaluation import load_evaluator
+    >>> evaluator = load_evaluator("string_distance")
+    >>> evaluator.evaluate_strings(
+            prediction="The answer is three",
+            reference="three",
+        )
     """
 
     @property
-    def requires_reference(self) -> bool:
-        """Return whether the chain requires a reference.
-
-        Returns:
-            bool: True if a reference is required, False otherwise.
+    def requires_input(self) -> bool:
         """
-        return True
+        This evaluator does not require input.
+        """
+        return False
 
     @property
-    def evaluation_name(self) -> str:
-        return f"embedding_{self.distance_metric.value}_distance"
+    def requires_reference(self) -> bool:
+        """
+        This evaluator does not require a reference.
+        """
+        return True
 
     @property
     def input_keys(self) -> List[str]:
-        """Return the input keys of the chain.
+        """
+        Get the input keys.
 
         Returns:
             List[str]: The input keys.
         """
-        return ["prediction", "reference"]
+        return ["reference", "prediction"]
+
+    @property
+    def evaluation_name(self) -> str:
+        """
+        Get the evaluation name.
+
+        Returns:
+            str: The evaluation name.
+        """
+        return f"{self.distance.value}_distance"
 
     def _call(
         self,
         inputs: Dict[str, Any],
         run_manager: Optional[CallbackManagerForChainRun] = None,
     ) -> Dict[str, Any]:
-        """Compute the score for a prediction and reference.
+        """
+        Compute the string distance between the prediction and the reference.
 
         Args:
-            inputs (Dict[str, Any]): The input data.
-            run_manager (Optional[CallbackManagerForChainRun], optional):
+            inputs (Dict[str, Any]): The input values.
+            run_manager (Optional[CallbackManagerForChainRun]):
                 The callback manager.
 
         Returns:
-            Dict[str, Any]: The computed score.
+            Dict[str, Any]: The evaluation results containing the score.
         """
-        vectors = np.array(
-            self.embeddings.embed_documents([inputs["prediction"], inputs["reference"]])
-        )
-        score = self._compute_score(vectors)
-        return {"score": score}
+        return {"score": self.compute_metric(inputs["reference"], inputs["prediction"])}
 
     async def _acall(
         self,
         inputs: Dict[str, Any],
         run_manager: Optional[AsyncCallbackManagerForChainRun] = None,
     ) -> Dict[str, Any]:
-        """Asynchronously compute the score for a prediction and reference.
+        """
+        Asynchronously compute the string distance between the prediction
+            and the reference.
 
         Args:
-            inputs (Dict[str, Any]): The input data.
-            run_manager (AsyncCallbackManagerForChainRun, optional):
+            inputs (Dict[str, Any]): The input values.
+            run_manager (Optional[AsyncCallbackManagerForChainRun]:
                 The callback manager.
 
         Returns:
-            Dict[str, Any]: The computed score.
+            Dict[str, Any]: The evaluation results containing the score.
         """
-        embedded = await self.embeddings.aembed_documents(
-            [inputs["prediction"], inputs["reference"]]
-        )
-        vectors = np.array(embedded)
-        score = self._compute_score(vectors)
-        return {"score": score}
+        return {"score": self.compute_metric(inputs["reference"], inputs["prediction"])}
 
     def _evaluate_strings(
         self,
         *,
         prediction: str,
         reference: Optional[str] = None,
+        input: Optional[str] = None,
         callbacks: Callbacks = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         include_run_info: bool = False,
         **kwargs: Any,
     ) -> dict:
-        """Evaluate the embedding distance between a prediction and
-        reference.
+        """
+        Evaluate the string distance between the prediction and the reference.
 
         Args:
-            prediction (str): The output string from the first model.
-            reference (str): The reference string (required)
+            prediction (str): The prediction string.
+            reference (Optional[str], optional): The reference string.
+            input (Optional[str], optional): The input string.
             callbacks (Callbacks, optional): The callbacks to use.
-            **kwargs (Any): Additional keyword arguments.
+            **kwargs: Additional keyword arguments.
 
         Returns:
-            dict: A dictionary containing:
-                - score: The embedding distance between the two
-                    predictions.
+            dict: The evaluation results containing the score.
         """
         result = self(
             inputs={"prediction": prediction, "reference": reference},
             callbacks=callbacks,
             tags=tags,
             metadata=metadata,
             include_run_info=include_run_info,
         )
+
         return self._prepare_output(result)
 
     async def _aevaluate_strings(
         self,
         *,
         prediction: str,
         reference: Optional[str] = None,
+        input: Optional[str] = None,
         callbacks: Callbacks = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         include_run_info: bool = False,
         **kwargs: Any,
     ) -> dict:
-        """Asynchronously evaluate the embedding distance between
-        a prediction and reference.
+        """
+        Asynchronously evaluate the string distance between the
+            prediction and the reference.
 
         Args:
-            prediction (str): The output string from the first model.
-            reference (str): The output string from the second model.
+            prediction (str): The prediction string.
+            reference (Optional[str], optional): The reference string.
+            input (Optional[str], optional): The input string.
             callbacks (Callbacks, optional): The callbacks to use.
-            **kwargs (Any): Additional keyword arguments.
+            **kwargs: Additional keyword arguments.
 
         Returns:
-            dict: A dictionary containing:
-                - score: The embedding distance between the two
-                    predictions.
+            dict: The evaluation results containing the score.
         """
         result = await self.acall(
             inputs={"prediction": prediction, "reference": reference},
             callbacks=callbacks,
             tags=tags,
             metadata=metadata,
             include_run_info=include_run_info,
         )
         return self._prepare_output(result)
 
 
-class PairwiseEmbeddingDistanceEvalChain(
-    _EmbeddingDistanceChainMixin, PairwiseStringEvaluator
-):
-    """Use embedding distances to score semantic difference between two predictions.
-
-    Examples:
-    >>> chain = PairwiseEmbeddingDistanceEvalChain()
-    >>> result = chain.evaluate_string_pairs(prediction="Hello", prediction_b="Hi")
-    >>> print(result)
-    {'score': 0.5}
-    """
+class PairwiseStringDistanceEvalChain(PairwiseStringEvaluator, _RapidFuzzChainMixin):
+    """Compute string edit distances between two predictions."""
 
     @property
     def input_keys(self) -> List[str]:
-        """Return the input keys of the chain.
+        """
+        Get the input keys.
 
         Returns:
             List[str]: The input keys.
         """
         return ["prediction", "prediction_b"]
 
     @property
     def evaluation_name(self) -> str:
-        return f"pairwise_embedding_{self.distance_metric.value}_distance"
+        """
+        Get the evaluation name.
+
+        Returns:
+            str: The evaluation name.
+        """
+        return f"pairwise_{self.distance.value}_distance"
 
     def _call(
         self,
         inputs: Dict[str, Any],
         run_manager: Optional[CallbackManagerForChainRun] = None,
     ) -> Dict[str, Any]:
-        """Compute the score for two predictions.
+        """
+        Compute the string distance between two predictions.
 
         Args:
-            inputs (Dict[str, Any]): The input data.
-            run_manager (CallbackManagerForChainRun, optional):
+            inputs (Dict[str, Any]): The input values.
+            run_manager (CallbackManagerForChainRun , optional):
                 The callback manager.
 
         Returns:
-            Dict[str, Any]: The computed score.
+            Dict[str, Any]: The evaluation results containing the score.
         """
-        vectors = np.array(
-            self.embeddings.embed_documents(
-                [inputs["prediction"], inputs["prediction_b"]]
-            )
-        )
-        score = self._compute_score(vectors)
-        return {"score": score}
+        return {
+            "score": self.compute_metric(inputs["prediction"], inputs["prediction_b"])
+        }
 
     async def _acall(
         self,
         inputs: Dict[str, Any],
         run_manager: Optional[AsyncCallbackManagerForChainRun] = None,
     ) -> Dict[str, Any]:
-        """Asynchronously compute the score for two predictions.
+        """
+        Asynchronously compute the string distance between two predictions.
 
         Args:
-            inputs (Dict[str, Any]): The input data.
-            run_manager (AsyncCallbackManagerForChainRun, optional):
+            inputs (Dict[str, Any]): The input values.
+            run_manager (AsyncCallbackManagerForChainRun , optional):
                 The callback manager.
 
         Returns:
-            Dict[str, Any]: The computed score.
+            Dict[str, Any]: The evaluation results containing the score.
         """
-        embedded = await self.embeddings.aembed_documents(
-            [inputs["prediction"], inputs["prediction_b"]]
-        )
-        vectors = np.array(embedded)
-        score = self._compute_score(vectors)
-        return {"score": score}
+        return {
+            "score": self.compute_metric(inputs["prediction"], inputs["prediction_b"])
+        }
 
     def _evaluate_string_pairs(
         self,
         *,
         prediction: str,
         prediction_b: str,
         callbacks: Callbacks = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         include_run_info: bool = False,
         **kwargs: Any,
     ) -> dict:
-        """Evaluate the embedding distance between two predictions.
+        """
+        Evaluate the string distance between two predictions.
 
         Args:
-            prediction (str): The output string from the first model.
-            prediction_b (str): The output string from the second model.
+            prediction (str): The first prediction string.
+            prediction_b (str): The second prediction string.
             callbacks (Callbacks, optional): The callbacks to use.
-            tags (List[str], optional): Tags to apply to traces
-            metadata (Dict[str, Any], optional): metadata to apply to
-            **kwargs (Any): Additional keyword arguments.
+            tags (List[str], optional): Tags to apply to traces.
+            metadata (Dict[str, Any], optional): Metadata to apply to traces.
+            **kwargs: Additional keyword arguments.
 
         Returns:
-            dict: A dictionary containing:
-                - score: The embedding distance between the two
-                    predictions.
+            dict: The evaluation results containing the score.
         """
         result = self(
             inputs={"prediction": prediction, "prediction_b": prediction_b},
             callbacks=callbacks,
             tags=tags,
             metadata=metadata,
             include_run_info=include_run_info,
@@ -448,30 +432,27 @@
         prediction_b: str,
         callbacks: Callbacks = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         include_run_info: bool = False,
         **kwargs: Any,
     ) -> dict:
-        """Asynchronously evaluate the embedding distance
-
-        between two predictions.
+        """
+        Asynchronously evaluate the string distance between two predictions.
 
         Args:
-            prediction (str): The output string from the first model.
-            prediction_b (str): The output string from the second model.
+            prediction (str): The first prediction string.
+            prediction_b (str): The second prediction string.
             callbacks (Callbacks, optional): The callbacks to use.
-            tags (List[str], optional): Tags to apply to traces
-            metadata (Dict[str, Any], optional): metadata to apply to traces
-            **kwargs (Any): Additional keyword arguments.
+            tags (List[str], optional): Tags to apply to traces.
+            metadata (Dict[str, Any], optional): Metadata to apply to traces.
+            **kwargs: Additional keyword arguments.
 
         Returns:
-            dict: A dictionary containing:
-                - score: The embedding distance between the two
-                    predictions.
+            dict: The evaluation results containing the score.
         """
         result = await self.acall(
             inputs={"prediction": prediction, "prediction_b": prediction_b},
             callbacks=callbacks,
             tags=tags,
             metadata=metadata,
             include_run_info=include_run_info,
```

### Comparing `gigachain-0.1.9/langchain/evaluation/exact_match/base.py` & `gigachain-0.2.0/langchain/evaluation/exact_match/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/evaluation/loading.py` & `gigachain-0.2.0/langchain/evaluation/loading.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Loading datasets and evaluators."""
+
 from typing import Any, Dict, List, Optional, Sequence, Type, Union
 
-from langchain_community.chat_models.openai import ChatOpenAI
 from langchain_core.language_models import BaseLanguageModel
 
 from langchain.chains.base import Chain
 from langchain.evaluation.agents.trajectory_eval_chain import TrajectoryEvalChain
 from langchain.evaluation.comparison import PairwiseStringEvalChain
 from langchain.evaluation.comparison.eval_chain import LabeledPairwiseStringEvalChain
 from langchain.evaluation.criteria.eval_chain import (
@@ -127,15 +127,29 @@
         raise ValueError(
             f"Unknown evaluator type: {evaluator}"
             f"\nValid types are: {list(_EVALUATOR_MAP.keys())}"
         )
     evaluator_cls = _EVALUATOR_MAP[evaluator]
     if issubclass(evaluator_cls, LLMEvalChain):
         try:
-            llm = llm or ChatOpenAI(
+            try:
+                from langchain_openai import ChatOpenAI
+            except ImportError:
+                try:
+                    from langchain_community.chat_models.openai import ChatOpenAI
+                except ImportError:
+                    raise ImportError(
+                        "Could not import langchain_openai or fallback onto "
+                        "langchain_community. Please install langchain_openai "
+                        "or specify a language model explicitly. "
+                        "It's recommended to install langchain_openai AND "
+                        "specify a language model explicitly."
+                    )
+
+            llm = llm or ChatOpenAI(  # type: ignore[call-arg]
                 model="gpt-4", model_kwargs={"seed": 42}, temperature=0
             )
         except Exception as e:
             raise ValueError(
                 f"Evaluation with the {evaluator_cls} requires a "
                 "language model to function."
                 " Failed to create the default 'gpt-4' model."
```

### Comparing `gigachain-0.1.9/langchain/evaluation/parsing/base.py` & `gigachain-0.2.0/langchain/evaluation/parsing/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Evaluators for parsing strings."""
+
 import json
 from operator import eq
 from typing import Any, Callable, Optional, Union, cast
 
+from langchain_core.utils.json import parse_json_markdown
+
 from langchain.evaluation.schema import StringEvaluator
-from langchain.output_parsers.json import parse_json_markdown
 
 
 class JsonValidityEvaluator(StringEvaluator):
-    """Evaluates whether the prediction is valid JSON.
+    """Evaluate whether the prediction is valid JSON.
 
     This evaluator checks if the prediction is a valid JSON string. It does not
         require any input or reference.
 
     Attributes:
         requires_input (bool): Whether this evaluator requires an input
             string. Always False.
@@ -72,15 +74,15 @@
             parse_json_markdown(prediction, parser=json.loads)
             return {"score": 1}
         except Exception as e:
             return {"score": 0, "reasoning": str(e)}
 
 
 class JsonEqualityEvaluator(StringEvaluator):
-    """Evaluates whether the prediction is equal to the reference after
+    """Evaluate whether the prediction is equal to the reference after
         parsing both as JSON.
 
     This evaluator checks if the prediction, after parsing as JSON, is equal
         to the reference,
     which is also parsed as JSON. It does not require an input string.
 
     Attributes:
```

### Comparing `gigachain-0.1.9/langchain/evaluation/parsing/json_distance.py` & `gigachain-0.2.0/langchain/evaluation/parsing/json_distance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 from typing import Any, Callable, Optional, Union
 
+from langchain_core.utils.json import parse_json_markdown
+
 from langchain.evaluation.schema import StringEvaluator
-from langchain.output_parsers.json import parse_json_markdown
 
 
 class JsonEditDistanceEvaluator(StringEvaluator):
     """
     An evaluator that calculates the edit distance between JSON strings.
 
     This evaluator computes a normalized Damerau-Levenshtein distance between two JSON strings
@@ -41,15 +42,15 @@
         **kwargs: Any,
     ) -> None:
         super().__init__()
         if string_distance is not None:
             self._string_distance = string_distance
         else:
             try:
-                from rapidfuzz import distance as rfd  # noqa: F401
+                from rapidfuzz import distance as rfd
             except ImportError:
                 raise ImportError(
                     "The default string_distance operator for the "
                     " JsonEditDistanceEvaluator requires installation of "
                     "the rapidfuzz package. "
                     "Please install it with `pip install rapidfuzz`."
                 )
```

### Comparing `gigachain-0.1.9/langchain/evaluation/parsing/json_schema.py` & `gigachain-0.2.0/langchain/evaluation/parsing/json_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, Union
 
+from langchain_core.utils.json import parse_json_markdown
+
 from langchain.evaluation.schema import StringEvaluator
-from langchain.output_parsers.json import parse_json_markdown
 
 
 class JsonSchemaEvaluator(StringEvaluator):
     """An evaluator that validates a JSON prediction against a JSON schema reference.
 
     This evaluator checks if a given JSON prediction conforms to the provided JSON schema.
     If the prediction is valid, the score is True (no errors). Otherwise, the score is False (error occurred).
@@ -69,15 +70,15 @@
             return parse_json_markdown(node)
         elif hasattr(node, "schema") and callable(getattr(node, "schema")):
             # Pydantic model
             return getattr(node, "schema")()
         return node
 
     def _validate(self, prediction: Any, schema: Any) -> dict:
-        from jsonschema import ValidationError, validate  # noqa: F401
+        from jsonschema import ValidationError, validate
 
         try:
             validate(instance=prediction, schema=schema)
             return {
                 "score": True,
             }
         except ValidationError as e:
```

### Comparing `gigachain-0.1.9/langchain/evaluation/qa/eval_chain.py` & `gigachain-0.2.0/langchain/evaluation/qa/eval_chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """LLM Chains for evaluating question answering."""
+
 from __future__ import annotations
 
 import re
 import string
 from typing import Any, List, Optional, Sequence, Tuple
 
+from langchain_core.callbacks.manager import Callbacks
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.prompts import PromptTemplate
 from langchain_core.pydantic_v1 import Extra
 
-from langchain.callbacks.manager import Callbacks
 from langchain.chains.llm import LLMChain
 from langchain.evaluation.qa.eval_prompt import CONTEXT_PROMPT, COT_PROMPT, PROMPT
 from langchain.evaluation.schema import LLMEvalChain, StringEvaluator
 from langchain.schema import RUN_KEY
 
 
 def _get_score(text: str) -> Optional[Tuple[str, int]]:
```

### Comparing `gigachain-0.1.9/langchain/evaluation/qa/eval_prompt.py` & `gigachain-0.2.0/langchain/evaluation/qa/eval_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/evaluation/qa/generate_chain.py` & `gigachain-0.2.0/langchain/evaluation/qa/generate_chain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """LLM Chain for generating examples for question answering."""
+
 from __future__ import annotations
 
 from typing import Any
 
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.output_parsers import BaseLLMOutputParser
 from langchain_core.pydantic_v1 import Field
```

### Comparing `gigachain-0.1.9/langchain/evaluation/qa/generate_prompt.py` & `gigachain-0.2.0/langchain/evaluation/qa/generate_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/evaluation/regex_match/base.py` & `gigachain-0.2.0/langchain/evaluation/regex_match/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/evaluation/schema.py` & `gigachain-0.2.0/langchain/evaluation/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Interfaces to be implemented by general evaluators."""
+
 from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import Any, Optional, Sequence, Tuple, Union
 from warnings import warn
```

### Comparing `gigachain-0.1.9/langchain/evaluation/scoring/__init__.py` & `gigachain-0.2.0/langchain/evaluation/scoring/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,13 +18,14 @@
     # {
     #    "score": 8,
     #    "comment": "The response accurately states "
     #    "that the chemical formula for water is H2O."
     #    "However, it does not provide an explanation of what the formula means."
     # }
 """
+
 from langchain.evaluation.scoring.eval_chain import (
     LabeledScoreStringEvalChain,
     ScoreStringEvalChain,
 )
 
 __all__ = ["ScoreStringEvalChain", "LabeledScoreStringEvalChain"]
```

### Comparing `gigachain-0.1.9/langchain/evaluation/scoring/eval_chain.py` & `gigachain-0.2.0/langchain/evaluation/scoring/eval_chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Base classes for scoring the output of a model on a scale of 1-10."""
+
 from __future__ import annotations
 
 import logging
 import re
 from typing import Any, Dict, List, Optional, Union
 
-from langchain_community.chat_models.azure_openai import AzureChatOpenAI
-from langchain_community.chat_models.openai import ChatOpenAI
+from langchain_core.callbacks.manager import Callbacks
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.output_parsers import BaseOutputParser
 from langchain_core.prompts.prompt import PromptTemplate
 from langchain_core.pydantic_v1 import Extra, Field
 
-from langchain.callbacks.manager import Callbacks
 from langchain.chains.constitutional_ai.models import ConstitutionalPrinciple
 from langchain.chains.llm import LLMChain
 from langchain.evaluation.criteria.eval_chain import (
     CRITERIA_TYPE,
     Criteria,
 )
 from langchain.evaluation.schema import LLMEvalChain, StringEvaluator
@@ -254,18 +253,15 @@
         Returns:
             ScoreStringEvalChain: The initialized ScoreStringEvalChain.
 
         Raises:
             ValueError: If the input variables are not as expected.
 
         """
-        if not (
-            isinstance(llm, (ChatOpenAI, AzureChatOpenAI))
-            and llm.model_name.startswith("gpt-4")
-        ):
+        if not (hasattr(llm, "model_name") and not llm.model_name.startswith("gpt-4")):
             logger.warning(
                 "This chain was only tested with GPT-4. \
 Performance may be significantly worse with other models."
             )
 
         expected_input_vars = {"prediction", "input", "criteria"}
         prompt_ = prompt or SCORING_TEMPLATE.partial(reference="")
```

### Comparing `gigachain-0.1.9/langchain/evaluation/scoring/prompt.py` & `gigachain-0.2.0/langchain/evaluation/scoring/prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Prompts for scoring the outputs of a models for a given question.
 
 This prompt is used to socre the responses and evaluate how it follows the instructions
 and answers the question. The prompt is based on the paper from
 Zheng, et. al. https://arxiv.org/abs/2306.05685
 """
+
 # flake8: noqa
 from langchain_core.prompts.chat import ChatPromptTemplate
 
 SYSTEM_MESSAGE = "You are a helpful assistant."
 
 CRITERIA_INSTRUCTIONS = (
     "For this evaluation, you should primarily consider the following criteria:\n"
```

### Comparing `gigachain-0.1.9/langchain/evaluation/string_distance/base.py` & `gigachain-0.2.0/langchain/evaluation/embedding_distance/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,424 +1,489 @@
-"""String distance evaluators based on the RapidFuzz library."""
+"""A chain for comparing the output of two models using embeddings."""
 
 from enum import Enum
-from typing import Any, Callable, Dict, List, Optional
+from typing import Any, Dict, List, Optional
 
-from langchain_core.pydantic_v1 import Field, root_validator
-
-from langchain.callbacks.manager import (
+import numpy as np
+from langchain_core.callbacks.manager import (
     AsyncCallbackManagerForChainRun,
     CallbackManagerForChainRun,
     Callbacks,
 )
+from langchain_core.embeddings import Embeddings
+from langchain_core.pydantic_v1 import Field, root_validator
+
 from langchain.chains.base import Chain
 from langchain.evaluation.schema import PairwiseStringEvaluator, StringEvaluator
 from langchain.schema import RUN_KEY
 
 
-def _load_rapidfuzz() -> Any:
-    """
-    Load the RapidFuzz library.
-
-    Raises:
-        ImportError: If the rapidfuzz library is not installed.
-
+def _embedding_factory() -> Embeddings:
+    """Create an Embeddings object.
     Returns:
-        Any: The rapidfuzz.distance module.
+        Embeddings: The created Embeddings object.
     """
+    # Here for backwards compatibility.
+    # Generally, we do not want to be seeing imports from langchain community
+    # or partner packages in langchain.
     try:
-        import rapidfuzz
+        from langchain_openai import OpenAIEmbeddings
     except ImportError:
-        raise ImportError(
-            "Please install the rapidfuzz library to use the FuzzyMatchStringEvaluator."
-            "Please install it with `pip install rapidfuzz`."
-        )
-    return rapidfuzz.distance
+        try:
+            from langchain_community.embeddings.openai import OpenAIEmbeddings
+        except ImportError:
+            raise ImportError(
+                "Could not import OpenAIEmbeddings. Please install the "
+                "OpenAIEmbeddings package using `pip install langchain-openai`."
+            )
+    return OpenAIEmbeddings()
 
 
-class StringDistance(str, Enum):
-    """Distance metric to use.
+class EmbeddingDistance(str, Enum):
+    """Embedding Distance Metric.
 
     Attributes:
-        DAMERAU_LEVENSHTEIN: The Damerau-Levenshtein distance.
-        LEVENSHTEIN: The Levenshtein distance.
-        JARO: The Jaro distance.
-        JARO_WINKLER: The Jaro-Winkler distance.
-        HAMMING: The Hamming distance.
-        INDEL: The Indel distance.
+        COSINE: Cosine distance metric.
+        EUCLIDEAN: Euclidean distance metric.
+        MANHATTAN: Manhattan distance metric.
+        CHEBYSHEV: Chebyshev distance metric.
+        HAMMING: Hamming distance metric.
     """
 
-    DAMERAU_LEVENSHTEIN = "damerau_levenshtein"
-    LEVENSHTEIN = "levenshtein"
-    JARO = "jaro"
-    JARO_WINKLER = "jaro_winkler"
+    COSINE = "cosine"
+    EUCLIDEAN = "euclidean"
+    MANHATTAN = "manhattan"
+    CHEBYSHEV = "chebyshev"
     HAMMING = "hamming"
-    INDEL = "indel"
 
 
-class _RapidFuzzChainMixin(Chain):
-    """Shared methods for the rapidfuzz string distance evaluators."""
+class _EmbeddingDistanceChainMixin(Chain):
+    """Shared functionality for embedding distance evaluators.
 
-    distance: StringDistance = Field(default=StringDistance.JARO_WINKLER)
-    normalize_score: bool = Field(default=True)
-    """Whether to normalize the score to a value between 0 and 1.
-    Applies only to the Levenshtein and Damerau-Levenshtein distances."""
+    Attributes:
+        embeddings (Embeddings): The embedding objects to vectorize the outputs.
+        distance_metric (EmbeddingDistance): The distance metric to use
+                                            for comparing the embeddings.
+    """
 
-    @root_validator
-    def validate_dependencies(cls, values: Dict[str, Any]) -> Dict[str, Any]:
-        """
-        Validate that the rapidfuzz library is installed.
+    embeddings: Embeddings = Field(default_factory=_embedding_factory)
+    distance_metric: EmbeddingDistance = Field(default=EmbeddingDistance.COSINE)
+
+    @root_validator(pre=False)
+    def _validate_tiktoken_installed(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+        """Validate that the TikTok library is installed.
 
         Args:
-            values (Dict[str, Any]): The input values.
+            values (Dict[str, Any]): The values to validate.
 
         Returns:
             Dict[str, Any]: The validated values.
         """
-        _load_rapidfuzz()
+        embeddings = values.get("embeddings")
+        types_ = []
+        try:
+            from langchain_openai import OpenAIEmbeddings
+
+            types_.append(OpenAIEmbeddings)
+        except ImportError:
+            pass
+
+        try:
+            from langchain_community.embeddings.openai import OpenAIEmbeddings
+
+            types_.append(OpenAIEmbeddings)
+        except ImportError:
+            pass
+
+        if not types_:
+            raise ImportError(
+                "Could not import OpenAIEmbeddings. Please install the "
+                "OpenAIEmbeddings package using `pip install langchain-openai`."
+            )
+
+        if isinstance(embeddings, tuple(types_)):
+            try:
+                import tiktoken  # noqa: F401
+            except ImportError:
+                raise ImportError(
+                    "The tiktoken library is required to use the default "
+                    "OpenAI embeddings with embedding distance evaluators."
+                    " Please either manually select a different Embeddings object"
+                    " or install tiktoken using `pip install tiktoken`."
+                )
         return values
 
+    class Config:
+        """Permit embeddings to go unvalidated."""
+
+        arbitrary_types_allowed: bool = True
+
     @property
     def output_keys(self) -> List[str]:
-        """
-        Get the output keys.
+        """Return the output keys of the chain.
 
         Returns:
             List[str]: The output keys.
         """
         return ["score"]
 
-    def _prepare_output(self, result: Dict[str, Any]) -> Dict[str, Any]:
-        """
-        Prepare the output dictionary.
+    def _prepare_output(self, result: dict) -> dict:
+        parsed = {"score": result["score"]}
+        if RUN_KEY in result:
+            parsed[RUN_KEY] = result[RUN_KEY]
+        return parsed
+
+    def _get_metric(self, metric: EmbeddingDistance) -> Any:
+        """Get the metric function for the given metric name.
 
         Args:
-            result (Dict[str, Any]): The evaluation results.
+            metric (EmbeddingDistance): The metric name.
 
         Returns:
-            Dict[str, Any]: The prepared output dictionary.
+            Any: The metric function.
         """
-        result = {"score": result["score"]}
-        if RUN_KEY in result:
-            result[RUN_KEY] = result[RUN_KEY].dict()
-        return result
+        metrics = {
+            EmbeddingDistance.COSINE: self._cosine_distance,
+            EmbeddingDistance.EUCLIDEAN: self._euclidean_distance,
+            EmbeddingDistance.MANHATTAN: self._manhattan_distance,
+            EmbeddingDistance.CHEBYSHEV: self._chebyshev_distance,
+            EmbeddingDistance.HAMMING: self._hamming_distance,
+        }
+        if metric in metrics:
+            return metrics[metric]
+        else:
+            raise ValueError(f"Invalid metric: {metric}")
 
     @staticmethod
-    def _get_metric(distance: str, normalize_score: bool = False) -> Callable:
-        """
-        Get the distance metric function based on the distance type.
+    def _cosine_distance(a: np.ndarray, b: np.ndarray) -> np.ndarray:
+        """Compute the cosine distance between two vectors.
 
         Args:
-            distance (str): The distance type.
+            a (np.ndarray): The first vector.
+            b (np.ndarray): The second vector.
 
         Returns:
-            Callable: The distance metric function.
-
-        Raises:
-            ValueError: If the distance metric is invalid.
+            np.ndarray: The cosine distance.
         """
-        from rapidfuzz import distance as rf_distance
-
-        module_map: Dict[str, Any] = {
-            StringDistance.DAMERAU_LEVENSHTEIN: rf_distance.DamerauLevenshtein,
-            StringDistance.LEVENSHTEIN: rf_distance.Levenshtein,
-            StringDistance.JARO: rf_distance.Jaro,
-            StringDistance.JARO_WINKLER: rf_distance.JaroWinkler,
-            StringDistance.HAMMING: rf_distance.Hamming,
-            StringDistance.INDEL: rf_distance.Indel,
-        }
-        if distance not in module_map:
-            raise ValueError(
-                f"Invalid distance metric: {distance}"
-                f"\nMust be one of: {list(StringDistance)}"
+        try:
+            from langchain_community.utils.math import cosine_similarity
+        except ImportError:
+            raise ImportError(
+                "The cosine_similarity function is required to compute cosine distance."
+                " Please install the langchain-community package using"
+                " `pip install langchain-community`."
             )
-        module = module_map[distance]
-        if normalize_score:
-            return module.normalized_distance
-        else:
-            return module.distance
+        return 1.0 - cosine_similarity(a, b)
 
-    @property
-    def metric(self) -> Callable:
+    @staticmethod
+    def _euclidean_distance(a: np.ndarray, b: np.ndarray) -> np.floating:
+        """Compute the Euclidean distance between two vectors.
+
+        Args:
+            a (np.ndarray): The first vector.
+            b (np.ndarray): The second vector.
+
+        Returns:
+            np.floating: The Euclidean distance.
         """
-        Get the distance metric function.
+        return np.linalg.norm(a - b)
+
+    @staticmethod
+    def _manhattan_distance(a: np.ndarray, b: np.ndarray) -> np.floating:
+        """Compute the Manhattan distance between two vectors.
+
+        Args:
+            a (np.ndarray): The first vector.
+            b (np.ndarray): The second vector.
 
         Returns:
-            Callable: The distance metric function.
+            np.floating: The Manhattan distance.
         """
-        return _RapidFuzzChainMixin._get_metric(
-            self.distance, normalize_score=self.normalize_score
-        )
+        return np.sum(np.abs(a - b))
+
+    @staticmethod
+    def _chebyshev_distance(a: np.ndarray, b: np.ndarray) -> np.floating:
+        """Compute the Chebyshev distance between two vectors.
 
-    def compute_metric(self, a: str, b: str) -> float:
+        Args:
+            a (np.ndarray): The first vector.
+            b (np.ndarray): The second vector.
+
+        Returns:
+            np.floating: The Chebyshev distance.
         """
-        Compute the distance between two strings.
+        return np.max(np.abs(a - b))
+
+    @staticmethod
+    def _hamming_distance(a: np.ndarray, b: np.ndarray) -> np.floating:
+        """Compute the Hamming distance between two vectors.
 
         Args:
-            a (str): The first string.
-            b (str): The second string.
+            a (np.ndarray): The first vector.
+            b (np.ndarray): The second vector.
 
         Returns:
-            float: The distance between the two strings.
+            np.floating: The Hamming distance.
         """
-        return self.metric(a, b)
+        return np.mean(a != b)
 
+    def _compute_score(self, vectors: np.ndarray) -> float:
+        """Compute the score based on the distance metric.
 
-class StringDistanceEvalChain(StringEvaluator, _RapidFuzzChainMixin):
-    """Compute string distances between the prediction and the reference.
+        Args:
+            vectors (np.ndarray): The input vectors.
 
-    Examples
-    ----------
+        Returns:
+            float: The computed score.
+        """
+        metric = self._get_metric(self.distance_metric)
+        score = metric(vectors[0].reshape(1, -1), vectors[1].reshape(1, -1)).item()
+        return score
 
-    >>> from langchain.evaluation import StringDistanceEvalChain
-    >>> evaluator = StringDistanceEvalChain()
-    >>> evaluator.evaluate_strings(
-            prediction="Mindy is the CTO",
-            reference="Mindy is the CEO",
-        )
 
-    Using the `load_evaluator` function:
+class EmbeddingDistanceEvalChain(_EmbeddingDistanceChainMixin, StringEvaluator):
+    """Use embedding distances to score semantic difference between
+    a prediction and reference.
 
-    >>> from langchain.evaluation import load_evaluator
-    >>> evaluator = load_evaluator("string_distance")
-    >>> evaluator.evaluate_strings(
-            prediction="The answer is three",
-            reference="three",
-        )
+    Examples:
+        >>> chain = EmbeddingDistanceEvalChain()
+        >>> result = chain.evaluate_strings(prediction="Hello", reference="Hi")
+        >>> print(result)
+        {'score': 0.5}
     """
 
     @property
-    def requires_input(self) -> bool:
-        """
-        This evaluator does not require input.
-        """
-        return False
-
-    @property
     def requires_reference(self) -> bool:
-        """
-        This evaluator does not require a reference.
-        """
-        return True
-
-    @property
-    def input_keys(self) -> List[str]:
-        """
-        Get the input keys.
+        """Return whether the chain requires a reference.
 
         Returns:
-            List[str]: The input keys.
+            bool: True if a reference is required, False otherwise.
         """
-        return ["reference", "prediction"]
+        return True
 
     @property
     def evaluation_name(self) -> str:
-        """
-        Get the evaluation name.
+        return f"embedding_{self.distance_metric.value}_distance"
+
+    @property
+    def input_keys(self) -> List[str]:
+        """Return the input keys of the chain.
 
         Returns:
-            str: The evaluation name.
+            List[str]: The input keys.
         """
-        return f"{self.distance.value}_distance"
+        return ["prediction", "reference"]
 
     def _call(
         self,
         inputs: Dict[str, Any],
         run_manager: Optional[CallbackManagerForChainRun] = None,
     ) -> Dict[str, Any]:
-        """
-        Compute the string distance between the prediction and the reference.
+        """Compute the score for a prediction and reference.
 
         Args:
-            inputs (Dict[str, Any]): The input values.
-            run_manager (Optional[CallbackManagerForChainRun]):
+            inputs (Dict[str, Any]): The input data.
+            run_manager (Optional[CallbackManagerForChainRun], optional):
                 The callback manager.
 
         Returns:
-            Dict[str, Any]: The evaluation results containing the score.
+            Dict[str, Any]: The computed score.
         """
-        return {"score": self.compute_metric(inputs["reference"], inputs["prediction"])}
+        vectors = np.array(
+            self.embeddings.embed_documents([inputs["prediction"], inputs["reference"]])
+        )
+        score = self._compute_score(vectors)
+        return {"score": score}
 
     async def _acall(
         self,
         inputs: Dict[str, Any],
         run_manager: Optional[AsyncCallbackManagerForChainRun] = None,
     ) -> Dict[str, Any]:
-        """
-        Asynchronously compute the string distance between the prediction
-            and the reference.
+        """Asynchronously compute the score for a prediction and reference.
 
         Args:
-            inputs (Dict[str, Any]): The input values.
-            run_manager (Optional[AsyncCallbackManagerForChainRun]:
+            inputs (Dict[str, Any]): The input data.
+            run_manager (AsyncCallbackManagerForChainRun, optional):
                 The callback manager.
 
         Returns:
-            Dict[str, Any]: The evaluation results containing the score.
+            Dict[str, Any]: The computed score.
         """
-        return {"score": self.compute_metric(inputs["reference"], inputs["prediction"])}
+        embedded = await self.embeddings.aembed_documents(
+            [inputs["prediction"], inputs["reference"]]
+        )
+        vectors = np.array(embedded)
+        score = self._compute_score(vectors)
+        return {"score": score}
 
     def _evaluate_strings(
         self,
         *,
         prediction: str,
         reference: Optional[str] = None,
-        input: Optional[str] = None,
         callbacks: Callbacks = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         include_run_info: bool = False,
         **kwargs: Any,
     ) -> dict:
-        """
-        Evaluate the string distance between the prediction and the reference.
+        """Evaluate the embedding distance between a prediction and
+        reference.
 
         Args:
-            prediction (str): The prediction string.
-            reference (Optional[str], optional): The reference string.
-            input (Optional[str], optional): The input string.
+            prediction (str): The output string from the first model.
+            reference (str): The reference string (required)
             callbacks (Callbacks, optional): The callbacks to use.
-            **kwargs: Additional keyword arguments.
+            **kwargs (Any): Additional keyword arguments.
 
         Returns:
-            dict: The evaluation results containing the score.
+            dict: A dictionary containing:
+                - score: The embedding distance between the two
+                    predictions.
         """
         result = self(
             inputs={"prediction": prediction, "reference": reference},
             callbacks=callbacks,
             tags=tags,
             metadata=metadata,
             include_run_info=include_run_info,
         )
-
         return self._prepare_output(result)
 
     async def _aevaluate_strings(
         self,
         *,
         prediction: str,
         reference: Optional[str] = None,
-        input: Optional[str] = None,
         callbacks: Callbacks = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         include_run_info: bool = False,
         **kwargs: Any,
     ) -> dict:
-        """
-        Asynchronously evaluate the string distance between the
-            prediction and the reference.
+        """Asynchronously evaluate the embedding distance between
+        a prediction and reference.
 
         Args:
-            prediction (str): The prediction string.
-            reference (Optional[str], optional): The reference string.
-            input (Optional[str], optional): The input string.
+            prediction (str): The output string from the first model.
+            reference (str): The output string from the second model.
             callbacks (Callbacks, optional): The callbacks to use.
-            **kwargs: Additional keyword arguments.
+            **kwargs (Any): Additional keyword arguments.
 
         Returns:
-            dict: The evaluation results containing the score.
+            dict: A dictionary containing:
+                - score: The embedding distance between the two
+                    predictions.
         """
         result = await self.acall(
             inputs={"prediction": prediction, "reference": reference},
             callbacks=callbacks,
             tags=tags,
             metadata=metadata,
             include_run_info=include_run_info,
         )
         return self._prepare_output(result)
 
 
-class PairwiseStringDistanceEvalChain(PairwiseStringEvaluator, _RapidFuzzChainMixin):
-    """Compute string edit distances between two predictions."""
+class PairwiseEmbeddingDistanceEvalChain(
+    _EmbeddingDistanceChainMixin, PairwiseStringEvaluator
+):
+    """Use embedding distances to score semantic difference between two predictions.
+
+    Examples:
+    >>> chain = PairwiseEmbeddingDistanceEvalChain()
+    >>> result = chain.evaluate_string_pairs(prediction="Hello", prediction_b="Hi")
+    >>> print(result)
+    {'score': 0.5}
+    """
 
     @property
     def input_keys(self) -> List[str]:
-        """
-        Get the input keys.
+        """Return the input keys of the chain.
 
         Returns:
             List[str]: The input keys.
         """
         return ["prediction", "prediction_b"]
 
     @property
     def evaluation_name(self) -> str:
-        """
-        Get the evaluation name.
-
-        Returns:
-            str: The evaluation name.
-        """
-        return f"pairwise_{self.distance.value}_distance"
+        return f"pairwise_embedding_{self.distance_metric.value}_distance"
 
     def _call(
         self,
         inputs: Dict[str, Any],
         run_manager: Optional[CallbackManagerForChainRun] = None,
     ) -> Dict[str, Any]:
-        """
-        Compute the string distance between two predictions.
+        """Compute the score for two predictions.
 
         Args:
-            inputs (Dict[str, Any]): The input values.
-            run_manager (CallbackManagerForChainRun , optional):
+            inputs (Dict[str, Any]): The input data.
+            run_manager (CallbackManagerForChainRun, optional):
                 The callback manager.
 
         Returns:
-            Dict[str, Any]: The evaluation results containing the score.
+            Dict[str, Any]: The computed score.
         """
-        return {
-            "score": self.compute_metric(inputs["prediction"], inputs["prediction_b"])
-        }
+        vectors = np.array(
+            self.embeddings.embed_documents(
+                [inputs["prediction"], inputs["prediction_b"]]
+            )
+        )
+        score = self._compute_score(vectors)
+        return {"score": score}
 
     async def _acall(
         self,
         inputs: Dict[str, Any],
         run_manager: Optional[AsyncCallbackManagerForChainRun] = None,
     ) -> Dict[str, Any]:
-        """
-        Asynchronously compute the string distance between two predictions.
+        """Asynchronously compute the score for two predictions.
 
         Args:
-            inputs (Dict[str, Any]): The input values.
-            run_manager (AsyncCallbackManagerForChainRun , optional):
+            inputs (Dict[str, Any]): The input data.
+            run_manager (AsyncCallbackManagerForChainRun, optional):
                 The callback manager.
 
         Returns:
-            Dict[str, Any]: The evaluation results containing the score.
+            Dict[str, Any]: The computed score.
         """
-        return {
-            "score": self.compute_metric(inputs["prediction"], inputs["prediction_b"])
-        }
+        embedded = await self.embeddings.aembed_documents(
+            [inputs["prediction"], inputs["prediction_b"]]
+        )
+        vectors = np.array(embedded)
+        score = self._compute_score(vectors)
+        return {"score": score}
 
     def _evaluate_string_pairs(
         self,
         *,
         prediction: str,
         prediction_b: str,
         callbacks: Callbacks = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         include_run_info: bool = False,
         **kwargs: Any,
     ) -> dict:
-        """
-        Evaluate the string distance between two predictions.
+        """Evaluate the embedding distance between two predictions.
 
         Args:
-            prediction (str): The first prediction string.
-            prediction_b (str): The second prediction string.
+            prediction (str): The output string from the first model.
+            prediction_b (str): The output string from the second model.
             callbacks (Callbacks, optional): The callbacks to use.
-            tags (List[str], optional): Tags to apply to traces.
-            metadata (Dict[str, Any], optional): Metadata to apply to traces.
-            **kwargs: Additional keyword arguments.
+            tags (List[str], optional): Tags to apply to traces
+            metadata (Dict[str, Any], optional): metadata to apply to
+            **kwargs (Any): Additional keyword arguments.
 
         Returns:
-            dict: The evaluation results containing the score.
+            dict: A dictionary containing:
+                - score: The embedding distance between the two
+                    predictions.
         """
         result = self(
             inputs={"prediction": prediction, "prediction_b": prediction_b},
             callbacks=callbacks,
             tags=tags,
             metadata=metadata,
             include_run_info=include_run_info,
@@ -432,27 +497,30 @@
         prediction_b: str,
         callbacks: Callbacks = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         include_run_info: bool = False,
         **kwargs: Any,
     ) -> dict:
-        """
-        Asynchronously evaluate the string distance between two predictions.
+        """Asynchronously evaluate the embedding distance
+
+        between two predictions.
 
         Args:
-            prediction (str): The first prediction string.
-            prediction_b (str): The second prediction string.
+            prediction (str): The output string from the first model.
+            prediction_b (str): The output string from the second model.
             callbacks (Callbacks, optional): The callbacks to use.
-            tags (List[str], optional): Tags to apply to traces.
-            metadata (Dict[str, Any], optional): Metadata to apply to traces.
-            **kwargs: Additional keyword arguments.
+            tags (List[str], optional): Tags to apply to traces
+            metadata (Dict[str, Any], optional): metadata to apply to traces
+            **kwargs (Any): Additional keyword arguments.
 
         Returns:
-            dict: The evaluation results containing the score.
+            dict: A dictionary containing:
+                - score: The embedding distance between the two
+                    predictions.
         """
         result = await self.acall(
             inputs={"prediction": prediction, "prediction_b": prediction_b},
             callbacks=callbacks,
             tags=tags,
             metadata=metadata,
             include_run_info=include_run_info,
```

### Comparing `gigachain-0.1.9/langchain/globals/__init__.py` & `gigachain-0.2.0/langchain/globals/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Global values and configuration that apply to all of LangChain."""
+
 import warnings
 from typing import TYPE_CHECKING, Optional
 
 if TYPE_CHECKING:
     from langchain_core.caches import BaseCache
```

### Comparing `gigachain-0.1.9/langchain/graphs/__init__.py` & `gigachain-0.2.0/langchain/graphs/networkx_graph.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-"""**Graphs** provide a natural language interface to graph databases."""
-import warnings
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
-from langchain_core._api import LangChainDeprecationWarning
+from langchain._api import create_importer
 
-from langchain.utils.interactive_env import is_interactive_env
+if TYPE_CHECKING:
+    from langchain_community.graphs import NetworkxEntityGraph
+    from langchain_community.graphs.networkx_graph import (
+        KnowledgeTriple,
+        get_entities,
+        parse_triples,
+    )
+
+# Create a way to dynamically look up deprecated imports.
+# Used to consolidate logic for raising deprecation warnings and
+# handling optional imports.
+DEPRECATED_LOOKUP = {
+    "KnowledgeTriple": "langchain_community.graphs.networkx_graph",
+    "parse_triples": "langchain_community.graphs.networkx_graph",
+    "get_entities": "langchain_community.graphs.networkx_graph",
+    "NetworkxEntityGraph": "langchain_community.graphs",
+}
 
+_import_attribute = create_importer(__package__, deprecated_lookups=DEPRECATED_LOOKUP)
 
-def __getattr__(name: str) -> Any:
-    from langchain_community import graphs
-
-    # If not in interactive env, raise warning.
-    if not is_interactive_env():
-        warnings.warn(
-            "Importing graphs from langchain is deprecated. Importing from "
-            "langchain will no longer be supported as of langchain==0.2.0. "
-            "Please import from langchain-community instead:\n\n"
-            f"`from langchain_community.graphs import {name}`.\n\n"
-            "To install gigachain-community run `pip install -U gigachain-community`.",
-            category=LangChainDeprecationWarning,
-        )
 
-    return getattr(graphs, name)
+def __getattr__(name: str) -> Any:
+    """Look up attributes dynamically."""
+    return _import_attribute(name)
 
 
 __all__ = [
-    "MemgraphGraph",
+    "KnowledgeTriple",
+    "parse_triples",
+    "get_entities",
     "NetworkxEntityGraph",
-    "Neo4jGraph",
-    "NebulaGraph",
-    "NeptuneGraph",
-    "KuzuGraph",
-    "HugeGraph",
-    "RdfGraph",
-    "ArangoGraph",
-    "FalkorDBGraph",
 ]
```

### Comparing `gigachain-0.1.9/langchain/hub.py` & `gigachain-0.2.0/langchain/hub.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """Interface with the LangChain Hub."""
+
 from __future__ import annotations
 
+import json
 from typing import TYPE_CHECKING, Any, Optional
 
 from langchain_core.load.dump import dumps
 from langchain_core.load.load import loads
+from langchain_core.prompts import BasePromptTemplate
 
 if TYPE_CHECKING:
     from langchainhub import Client
 
 
 def _get_client(api_url: Optional[str] = None, api_key: Optional[str] = None) -> Client:
     try:
@@ -30,15 +33,15 @@
     api_url: Optional[str] = None,
     api_key: Optional[str] = None,
     parent_commit_hash: Optional[str] = "latest",
     new_repo_is_public: bool = True,
     new_repo_description: str = "",
 ) -> str:
     """
-    Pushes an object to the hub and returns the URL it can be viewed at in a browser.
+    Push an object to the hub and returns the URL it can be viewed at in a browser.
 
     :param repo_full_name: The full name of the repo to push to in the format of
         `owner/repo`.
     :param object: The LangChain to serialize and push to the hub.
     :param api_url: The URL of the LangChain Hub API. Defaults to the hosted API service
         if you have an api key set, or a localhost instance if not.
     :param api_key: The API key to use to authenticate with the LangChain Hub API.
@@ -64,18 +67,32 @@
 def pull(
     owner_repo_commit: str,
     *,
     api_url: Optional[str] = None,
     api_key: Optional[str] = None,
 ) -> Any:
     """
-    Pulls an object from the hub and returns it as a LangChain object.
+    Pull an object from the hub and returns it as a LangChain object.
 
     :param owner_repo_commit: The full name of the repo to pull from in the format of
         `owner/repo:commit_hash`.
     :param api_url: The URL of the LangChain Hub API. Defaults to the hosted API service
         if you have an api key set, or a localhost instance if not.
     :param api_key: The API key to use to authenticate with the LangChain Hub API.
     """
     client = _get_client(api_url=api_url, api_key=api_key)
+
+    if hasattr(client, "pull_repo"):
+        # >= 0.1.15
+        res_dict = client.pull_repo(owner_repo_commit)
+        obj = loads(json.dumps(res_dict["manifest"]))
+        if isinstance(obj, BasePromptTemplate):
+            if obj.metadata is None:
+                obj.metadata = {}
+            obj.metadata["lc_hub_owner"] = res_dict["owner"]
+            obj.metadata["lc_hub_repo"] = res_dict["repo"]
+            obj.metadata["lc_hub_commit_hash"] = res_dict["commit_hash"]
+        return obj
+
+    # Then it's < 0.1.15
     resp: str = client.pull(owner_repo_commit)
     return loads(resp)
```

### Comparing `gigachain-0.1.9/langchain/indexes/_sql_record_manager.py` & `gigachain-0.2.0/langchain/indexes/_sql_record_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,19 +9,21 @@
 allow it to work with a variety of SQL as a backend.
 
 * Each key is associated with an updated_at field.
 * This filed is updated whenever the key is updated.
 * Keys can be listed based on the updated at field.
 * Keys can be deleted.
 """
+
 import contextlib
 import decimal
 import uuid
 from typing import Any, AsyncGenerator, Dict, Generator, List, Optional, Sequence, Union
 
+from langchain_core.indexing import RecordManager
 from sqlalchemy import (
     URL,
     Column,
     Engine,
     Float,
     Index,
     String,
@@ -37,16 +39,14 @@
     AsyncSession,
     async_sessionmaker,
     create_async_engine,
 )
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import Query, Session, sessionmaker
 
-from langchain.indexes.base import RecordManager
-
 Base = declarative_base()
 
 
 class UpsertionRecord(Base):  # type: ignore[valid-type,misc]
     """Table used to keep track of when a key was last updated."""
 
     # ATTENTION:
@@ -304,15 +304,15 @@
                 from sqlalchemy.dialects.postgresql import insert as pg_insert
 
                 # Note: uses postgresql insert to make on_conflict_do_update work.
                 # This code needs to be generalized a bit to work with more dialects.
                 pg_insert_stmt: PgInsertType = pg_insert(UpsertionRecord).values(
                     records_to_upsert
                 )
-                stmt = pg_insert_stmt.on_conflict_do_update(
+                stmt = pg_insert_stmt.on_conflict_do_update(  # type: ignore[assignment]
                     "uix_key_namespace",  # Name of constraint
                     set_=dict(
                         updated_at=pg_insert_stmt.excluded.updated_at,
                         group_id=pg_insert_stmt.excluded.group_id,
                     ),
                 )
             else:
@@ -383,15 +383,15 @@
                 from sqlalchemy.dialects.postgresql import insert as pg_insert
 
                 # Note: uses SQLite insert to make on_conflict_do_update work.
                 # This code needs to be generalized a bit to work with more dialects.
                 pg_insert_stmt: PgInsertType = pg_insert(UpsertionRecord).values(
                     records_to_upsert
                 )
-                stmt = pg_insert_stmt.on_conflict_do_update(
+                stmt = pg_insert_stmt.on_conflict_do_update(  # type: ignore[assignment]
                     "uix_key_namespace",  # Name of constraint
                     set_=dict(
                         updated_at=pg_insert_stmt.excluded.updated_at,
                         group_id=pg_insert_stmt.excluded.group_id,
                     ),
                 )
             else:
@@ -468,15 +468,15 @@
         after: Optional[float] = None,
         group_ids: Optional[Sequence[str]] = None,
         limit: Optional[int] = None,
     ) -> List[str]:
         """List records in the SQLite database based on the provided date range."""
         session: AsyncSession
         async with self._amake_session() as session:
-            query: Query = select(UpsertionRecord.key).filter(
+            query: Query = select(UpsertionRecord.key).filter(  # type: ignore[assignment]
                 UpsertionRecord.namespace == self.namespace
             )
 
             # mypy does not recognize .all() or .filter()
             if after:
                 query = query.filter(UpsertionRecord.updated_at > after)
             if before:
```

### Comparing `gigachain-0.1.9/langchain/indexes/prompts/entity_extraction.py` & `gigachain-0.2.0/langchain/indexes/prompts/entity_extraction.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/indexes/prompts/entity_summarization.py` & `gigachain-0.2.0/langchain/indexes/prompts/entity_summarization.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/indexes/prompts/knowledge_triplet_extraction.py` & `gigachain-0.2.0/langchain/indexes/prompts/knowledge_triplet_extraction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # flake8: noqa
 
-from langchain_community.graphs.networkx_graph import KG_TRIPLE_DELIMITER
 from langchain_core.prompts.prompt import PromptTemplate
 
+KG_TRIPLE_DELIMITER = "<|>"
+
 _DEFAULT_KNOWLEDGE_TRIPLE_EXTRACTION_TEMPLATE = (
     "Ты сетевой интеллект, помогающий человеку отслеживать тройки знаний"
     " обо всех соответствующих людях, вещах, концепциях и т.д. и интегрировать"
     " их с твоими знаниями, хранящимися в твоих весах,"
     " а также с теми, что хранятся в графе знаний."
     " Извлеки все тройки знаний из текста."
     " Тройка знаний - это предложение, которое содержит субъект, предикат"
```

### Comparing `gigachain-0.1.9/langchain/llms/__init__.py` & `gigachain-0.2.0/langchain/llms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,21 +13,22 @@
 .. code-block::
 
     LLMResult, PromptValue,
     CallbackManagerForLLMRun, AsyncCallbackManagerForLLMRun,
     CallbackManager, AsyncCallbackManager,
     AIMessage, BaseMessage
 """  # noqa: E501
+
 import warnings
 from typing import Any, Callable, Dict, Type
 
 from langchain_core._api import LangChainDeprecationWarning
 from langchain_core.language_models.llms import BaseLLM
 
-from langchain.utils.interactive_env import is_interactive_env
+from langchain._api.interactive_env import is_interactive_env
 
 
 def _import_ai21() -> Any:
     from langchain_community.llms.ai21 import AI21
 
     return AI21
 
@@ -173,15 +174,15 @@
 def _import_edenai() -> Any:
     from langchain_community.llms.edenai import EdenAI
 
     return EdenAI
 
 
 def _import_fake() -> Any:
-    from langchain_community.llms.fake import FakeListLLM
+    from langchain_core.language_models import FakeListLLM
 
     return FakeListLLM
 
 
 def _import_fireworks() -> Any:
     from langchain_community.llms.fireworks import Fireworks
 
@@ -465,17 +466,17 @@
 def _import_titan_takeoff() -> Any:
     from langchain_community.llms.titan_takeoff import TitanTakeoff
 
     return TitanTakeoff
 
 
 def _import_titan_takeoff_pro() -> Any:
-    from langchain_community.llms.titan_takeoff_pro import TitanTakeoffPro
+    from langchain_community.llms.titan_takeoff import TitanTakeoff
 
-    return TitanTakeoffPro
+    return TitanTakeoff
 
 
 def _import_together() -> Any:
     from langchain_community.llms.together import Together
 
     return Together
```

### Comparing `gigachain-0.1.9/langchain/llms/grammars/json.gbnf` & `gigachain-0.2.0/langchain/llms/grammars/json.gbnf`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/memory/buffer.py` & `gigachain-0.2.0/langchain/memory/buffer.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/memory/buffer_window.py` & `gigachain-0.2.0/langchain/memory/buffer_window.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/memory/chat_memory.py` & `gigachain-0.2.0/langchain/memory/chat_memory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,55 @@
+import warnings
 from abc import ABC
 from typing import Any, Dict, Optional, Tuple
 
-from langchain_community.chat_message_histories.in_memory import ChatMessageHistory
-from langchain_core.chat_history import BaseChatMessageHistory
+from langchain_core.chat_history import (
+    BaseChatMessageHistory,
+    InMemoryChatMessageHistory,
+)
 from langchain_core.memory import BaseMemory
 from langchain_core.messages import AIMessage, HumanMessage
 from langchain_core.pydantic_v1 import Field
 
 from langchain.memory.utils import get_prompt_input_key
 
 
 class BaseChatMemory(BaseMemory, ABC):
     """Abstract base class for chat memory."""
 
-    chat_memory: BaseChatMessageHistory = Field(default_factory=ChatMessageHistory)
+    chat_memory: BaseChatMessageHistory = Field(
+        default_factory=InMemoryChatMessageHistory
+    )
     output_key: Optional[str] = None
     input_key: Optional[str] = None
     return_messages: bool = False
 
     def _get_input_output(
         self, inputs: Dict[str, Any], outputs: Dict[str, str]
     ) -> Tuple[str, str]:
         if self.input_key is None:
             prompt_input_key = get_prompt_input_key(inputs, self.memory_variables)
         else:
             prompt_input_key = self.input_key
         if self.output_key is None:
-            if len(outputs) != 1:
-                raise ValueError(f"One output key expected, got {outputs.keys()}")
-            output_key = list(outputs.keys())[0]
+            if len(outputs) == 1:
+                output_key = list(outputs.keys())[0]
+            elif "output" in outputs:
+                output_key = "output"
+                warnings.warn(
+                    f"'{self.__class__.__name__}' got multiple output keys:"
+                    f" {outputs.keys()}. The default 'output' key is being used."
+                    f" If this is not desired, please manually set 'output_key'."
+                )
+            else:
+                raise ValueError(
+                    f"Got multiple output keys: {outputs.keys()}, cannot "
+                    f"determine which to store in memory. Please set the "
+                    f"'output_key' explicitly."
+                )
         else:
             output_key = self.output_key
         return inputs[prompt_input_key], outputs[output_key]
 
     def save_context(self, inputs: Dict[str, Any], outputs: Dict[str, str]) -> None:
         """Save context from this conversation to buffer."""
         input_str, output_str = self._get_input_output(inputs, outputs)
```

### Comparing `gigachain-0.1.9/langchain/memory/combined.py` & `gigachain-0.2.0/langchain/memory/combined.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/memory/entity.py` & `gigachain-0.2.0/langchain/memory/entity.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 from abc import ABC, abstractmethod
 from itertools import islice
 from typing import Any, Dict, Iterable, List, Optional
 
-from langchain_community.utilities.redis import get_client
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.messages import BaseMessage, get_buffer_string
 from langchain_core.prompts import BasePromptTemplate
 from langchain_core.pydantic_v1 import BaseModel, Field
 
 from langchain.chains.llm import LLMChain
 from langchain.memory.chat_memory import BaseChatMemory
@@ -178,14 +177,22 @@
                 "Could not import redis python package. "
                 "Please install it with `pip install redis`."
             )
 
         super().__init__(*args, **kwargs)
 
         try:
+            from langchain_community.utilities.redis import get_client
+        except ImportError:
+            raise ImportError(
+                "Could not import langchain_community.utilities.redis.get_client. "
+                "Please install it with `pip install langchain-community`."
+            )
+
+        try:
             self.redis_client = get_client(redis_url=url, decode_responses=True)
         except redis.exceptions.ConnectionError as error:
             logger.error(error)
 
         self.session_id = session_id
         self.key_prefix = key_prefix
         self.ttl = ttl
```

### Comparing `gigachain-0.1.9/langchain/memory/kg.py` & `gigachain-0.2.0/langchain/memory/vectorstore.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,133 +1,101 @@
-from typing import Any, Dict, List, Type, Union
+"""Class for a VectorStore-backed memory object."""
 
-from langchain_community.graphs import NetworkxEntityGraph
-from langchain_community.graphs.networkx_graph import (
-    KnowledgeTriple,
-    get_entities,
-    parse_triples,
-)
-from langchain_core.language_models import BaseLanguageModel
-from langchain_core.messages import BaseMessage, SystemMessage, get_buffer_string
-from langchain_core.prompts import BasePromptTemplate
+from typing import Any, Dict, List, Optional, Sequence, Union
+
+from langchain_core.documents import Document
 from langchain_core.pydantic_v1 import Field
+from langchain_core.vectorstores import VectorStoreRetriever
 
-from langchain.chains.llm import LLMChain
-from langchain.memory.chat_memory import BaseChatMemory
-from langchain.memory.prompt import (
-    ENTITY_EXTRACTION_PROMPT,
-    KNOWLEDGE_TRIPLE_EXTRACTION_PROMPT,
-)
+from langchain.memory.chat_memory import BaseMemory
 from langchain.memory.utils import get_prompt_input_key
 
 
-class ConversationKGMemory(BaseChatMemory):
-    """Knowledge graph conversation memory.
+class VectorStoreRetrieverMemory(BaseMemory):
+    """VectorStoreRetriever-backed memory."""
+
+    retriever: VectorStoreRetriever = Field(exclude=True)
+    """VectorStoreRetriever object to connect to."""
 
-    Integrates with external knowledge graph to store and retrieve
-    information about knowledge triples in the conversation.
-    """
-
-    k: int = 2
-    human_prefix: str = "Human"
-    ai_prefix: str = "AI"
-    kg: NetworkxEntityGraph = Field(default_factory=NetworkxEntityGraph)
-    knowledge_extraction_prompt: BasePromptTemplate = KNOWLEDGE_TRIPLE_EXTRACTION_PROMPT
-    entity_extraction_prompt: BasePromptTemplate = ENTITY_EXTRACTION_PROMPT
-    llm: BaseLanguageModel
-    summary_message_cls: Type[BaseMessage] = SystemMessage
-    """Number of previous utterances to include in the context."""
     memory_key: str = "history"  #: :meta private:
+    """Key name to locate the memories in the result of load_memory_variables."""
 
-    def load_memory_variables(self, inputs: Dict[str, Any]) -> Dict[str, Any]:
-        """Return history buffer."""
-        entities = self._get_current_entities(inputs)
+    input_key: Optional[str] = None
+    """Key name to index the inputs to load_memory_variables."""
 
-        summary_strings = []
-        for entity in entities:
-            knowledge = self.kg.get_entity_knowledge(entity)
-            if knowledge:
-                summary = f"On {entity}: {'. '.join(knowledge)}."
-                summary_strings.append(summary)
-        context: Union[str, List]
-        if not summary_strings:
-            context = [] if self.return_messages else ""
-        elif self.return_messages:
-            context = [
-                self.summary_message_cls(content=text) for text in summary_strings
-            ]
-        else:
-            context = "\n".join(summary_strings)
+    return_docs: bool = False
+    """Whether or not to return the result of querying the database directly."""
 
-        return {self.memory_key: context}
+    exclude_input_keys: Sequence[str] = Field(default_factory=tuple)
+    """Input keys to exclude in addition to memory key when constructing the document"""
 
     @property
     def memory_variables(self) -> List[str]:
-        """Will always return list of memory variables.
-
-        :meta private:
-        """
+        """The list of keys emitted from the load_memory_variables method."""
         return [self.memory_key]
 
     def _get_prompt_input_key(self, inputs: Dict[str, Any]) -> str:
         """Get the input key for the prompt."""
         if self.input_key is None:
             return get_prompt_input_key(inputs, self.memory_variables)
         return self.input_key
 
-    def _get_prompt_output_key(self, outputs: Dict[str, Any]) -> str:
-        """Get the output key for the prompt."""
-        if self.output_key is None:
-            if len(outputs) != 1:
-                raise ValueError(f"One output key expected, got {outputs.keys()}")
-            return list(outputs.keys())[0]
-        return self.output_key
-
-    def get_current_entities(self, input_string: str) -> List[str]:
-        chain = LLMChain(llm=self.llm, prompt=self.entity_extraction_prompt)
-        buffer_string = get_buffer_string(
-            self.chat_memory.messages[-self.k * 2 :],
-            human_prefix=self.human_prefix,
-            ai_prefix=self.ai_prefix,
-        )
-        output = chain.predict(
-            history=buffer_string,
-            input=input_string,
-        )
-        return get_entities(output)
-
-    def _get_current_entities(self, inputs: Dict[str, Any]) -> List[str]:
-        """Get the current entities in the conversation."""
-        prompt_input_key = self._get_prompt_input_key(inputs)
-        return self.get_current_entities(inputs[prompt_input_key])
-
-    def get_knowledge_triplets(self, input_string: str) -> List[KnowledgeTriple]:
-        chain = LLMChain(llm=self.llm, prompt=self.knowledge_extraction_prompt)
-        buffer_string = get_buffer_string(
-            self.chat_memory.messages[-self.k * 2 :],
-            human_prefix=self.human_prefix,
-            ai_prefix=self.ai_prefix,
-        )
-        output = chain.predict(
-            history=buffer_string,
-            input=input_string,
-            verbose=True,
-        )
-        knowledge = parse_triples(output)
-        return knowledge
-
-    def _get_and_update_kg(self, inputs: Dict[str, Any]) -> None:
-        """Get and update knowledge graph from the conversation history."""
-        prompt_input_key = self._get_prompt_input_key(inputs)
-        knowledge = self.get_knowledge_triplets(inputs[prompt_input_key])
-        for triple in knowledge:
-            self.kg.add_triple(triple)
+    def _documents_to_memory_variables(
+        self, docs: List[Document]
+    ) -> Dict[str, Union[List[Document], str]]:
+        result: Union[List[Document], str]
+        if not self.return_docs:
+            result = "\n".join([doc.page_content for doc in docs])
+        else:
+            result = docs
+        return {self.memory_key: result}
+
+    def load_memory_variables(
+        self, inputs: Dict[str, Any]
+    ) -> Dict[str, Union[List[Document], str]]:
+        """Return history buffer."""
+        input_key = self._get_prompt_input_key(inputs)
+        query = inputs[input_key]
+        docs = self.retriever.invoke(query)
+        return self._documents_to_memory_variables(docs)
+
+    async def aload_memory_variables(
+        self, inputs: Dict[str, Any]
+    ) -> Dict[str, Union[List[Document], str]]:
+        """Return history buffer."""
+        input_key = self._get_prompt_input_key(inputs)
+        query = inputs[input_key]
+        docs = await self.retriever.ainvoke(query)
+        return self._documents_to_memory_variables(docs)
+
+    def _form_documents(
+        self, inputs: Dict[str, Any], outputs: Dict[str, str]
+    ) -> List[Document]:
+        """Format context from this conversation to buffer."""
+        # Each document should only include the current turn, not the chat history
+        exclude = set(self.exclude_input_keys)
+        exclude.add(self.memory_key)
+        filtered_inputs = {k: v for k, v in inputs.items() if k not in exclude}
+        texts = [
+            f"{k}: {v}"
+            for k, v in list(filtered_inputs.items()) + list(outputs.items())
+        ]
+        page_content = "\n".join(texts)
+        return [Document(page_content=page_content)]
 
     def save_context(self, inputs: Dict[str, Any], outputs: Dict[str, str]) -> None:
         """Save context from this conversation to buffer."""
-        super().save_context(inputs, outputs)
-        self._get_and_update_kg(inputs)
+        documents = self._form_documents(inputs, outputs)
+        self.retriever.add_documents(documents)
+
+    async def asave_context(
+        self, inputs: Dict[str, Any], outputs: Dict[str, str]
+    ) -> None:
+        """Save context from this conversation to buffer."""
+        documents = self._form_documents(inputs, outputs)
+        await self.retriever.aadd_documents(documents)
 
     def clear(self) -> None:
-        """Clear memory contents."""
-        super().clear()
-        self.kg.clear()
+        """Nothing to clear."""
+
+    async def aclear(self) -> None:
+        """Nothing to clear."""
```

### Comparing `gigachain-0.1.9/langchain/memory/motorhead_memory.py` & `gigachain-0.2.0/langchain/memory/summary.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,94 +1,98 @@
-from typing import Any, Dict, List, Optional
+from __future__ import annotations
 
-import requests
-from langchain_core.messages import get_buffer_string
+from typing import Any, Dict, List, Type
 
-from langchain.memory.chat_memory import BaseChatMemory
+from langchain_core.chat_history import BaseChatMessageHistory
+from langchain_core.language_models import BaseLanguageModel
+from langchain_core.messages import BaseMessage, SystemMessage, get_buffer_string
+from langchain_core.prompts import BasePromptTemplate
+from langchain_core.pydantic_v1 import BaseModel, root_validator
 
-MANAGED_URL = "https://api.getmetal.io/v1/motorhead"
-# LOCAL_URL = "http://localhost:8080"
+from langchain.chains.llm import LLMChain
+from langchain.memory.chat_memory import BaseChatMemory
+from langchain.memory.prompt import SUMMARY_PROMPT
 
 
-class MotorheadMemory(BaseChatMemory):
-    """Chat message memory backed by Motorhead service."""
+class SummarizerMixin(BaseModel):
+    """Mixin for summarizer."""
 
-    url: str = MANAGED_URL
-    timeout: int = 3000
-    memory_key: str = "history"
-    session_id: str
-    context: Optional[str] = None
+    human_prefix: str = "Human"
+    ai_prefix: str = "AI"
+    llm: BaseLanguageModel
+    prompt: BasePromptTemplate = SUMMARY_PROMPT
+    summary_message_cls: Type[BaseMessage] = SystemMessage
+
+    def predict_new_summary(
+        self, messages: List[BaseMessage], existing_summary: str
+    ) -> str:
+        new_lines = get_buffer_string(
+            messages,
+            human_prefix=self.human_prefix,
+            ai_prefix=self.ai_prefix,
+        )
 
-    # Managed Params
-    api_key: Optional[str] = None
-    client_id: Optional[str] = None
+        chain = LLMChain(llm=self.llm, prompt=self.prompt)
+        return chain.predict(summary=existing_summary, new_lines=new_lines)
 
-    def __get_headers(self) -> Dict[str, str]:
-        is_managed = self.url == MANAGED_URL
 
-        headers = {
-            "Content-Type": "application/json",
-        }
+class ConversationSummaryMemory(BaseChatMemory, SummarizerMixin):
+    """Conversation summarizer to chat memory."""
 
-        if is_managed and not (self.api_key and self.client_id):
-            raise ValueError(
-                """
-                You must provide an API key or a client ID to use the managed
-                version of Motorhead. Visit https://getmetal.io for more information.
-                """
+    buffer: str = ""
+    memory_key: str = "history"  #: :meta private:
+
+    @classmethod
+    def from_messages(
+        cls,
+        llm: BaseLanguageModel,
+        chat_memory: BaseChatMessageHistory,
+        *,
+        summarize_step: int = 2,
+        **kwargs: Any,
+    ) -> ConversationSummaryMemory:
+        obj = cls(llm=llm, chat_memory=chat_memory, **kwargs)
+        for i in range(0, len(obj.chat_memory.messages), summarize_step):
+            obj.buffer = obj.predict_new_summary(
+                obj.chat_memory.messages[i : i + summarize_step], obj.buffer
             )
+        return obj
 
-        if is_managed and self.api_key and self.client_id:
-            headers["x-metal-api-key"] = self.api_key
-            headers["x-metal-client-id"] = self.client_id
-
-        return headers
-
-    async def init(self) -> None:
-        res = requests.get(
-            f"{self.url}/sessions/{self.session_id}/memory",
-            timeout=self.timeout,
-            headers=self.__get_headers(),
-        )
-        res_data = res.json()
-        res_data = res_data.get("data", res_data)  # Handle Managed Version
-
-        messages = res_data.get("messages", [])
-        context = res_data.get("context", "NONE")
-
-        for message in reversed(messages):
-            if message["role"] == "AI":
-                self.chat_memory.add_ai_message(message["content"])
-            else:
-                self.chat_memory.add_user_message(message["content"])
+    @property
+    def memory_variables(self) -> List[str]:
+        """Will always return list of memory variables.
 
-        if context and context != "NONE":
-            self.context = context
+        :meta private:
+        """
+        return [self.memory_key]
 
-    def load_memory_variables(self, values: Dict[str, Any]) -> Dict[str, Any]:
+    def load_memory_variables(self, inputs: Dict[str, Any]) -> Dict[str, Any]:
+        """Return history buffer."""
         if self.return_messages:
-            return {self.memory_key: self.chat_memory.messages}
+            buffer: Any = [self.summary_message_cls(content=self.buffer)]
         else:
-            return {self.memory_key: get_buffer_string(self.chat_memory.messages)}
+            buffer = self.buffer
+        return {self.memory_key: buffer}
 
-    @property
-    def memory_variables(self) -> List[str]:
-        return [self.memory_key]
+    @root_validator()
+    def validate_prompt_input_variables(cls, values: Dict) -> Dict:
+        """Validate that prompt input variables are consistent."""
+        prompt_variables = values["prompt"].input_variables
+        expected_keys = {"summary", "new_lines"}
+        if expected_keys != set(prompt_variables):
+            raise ValueError(
+                "Got unexpected prompt input variables. The prompt expects "
+                f"{prompt_variables}, but it should have {expected_keys}."
+            )
+        return values
 
     def save_context(self, inputs: Dict[str, Any], outputs: Dict[str, str]) -> None:
-        input_str, output_str = self._get_input_output(inputs, outputs)
-        requests.post(
-            f"{self.url}/sessions/{self.session_id}/memory",
-            timeout=self.timeout,
-            json={
-                "messages": [
-                    {"role": "Human", "content": f"{input_str}"},
-                    {"role": "AI", "content": f"{output_str}"},
-                ]
-            },
-            headers=self.__get_headers(),
-        )
+        """Save context from this conversation to buffer."""
         super().save_context(inputs, outputs)
+        self.buffer = self.predict_new_summary(
+            self.chat_memory.messages[-2:], self.buffer
+        )
 
-    def delete_session(self) -> None:
-        """Delete a session"""
-        requests.delete(f"{self.url}/sessions/{self.session_id}/memory")
+    def clear(self) -> None:
+        """Clear memory contents."""
+        super().clear()
+        self.buffer = ""
```

### Comparing `gigachain-0.1.9/langchain/memory/prompt.py` & `gigachain-0.2.0/langchain/memory/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/memory/readonly.py` & `gigachain-0.2.0/langchain/memory/readonly.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List
 
 from langchain_core.memory import BaseMemory
 
 
 class ReadOnlySharedMemory(BaseMemory):
-    """A memory wrapper that is read-only and cannot be changed."""
+    """Memory wrapper that is read-only and cannot be changed."""
 
     memory: BaseMemory
 
     @property
     def memory_variables(self) -> List[str]:
         """Return memory variables."""
         return self.memory.memory_variables
```

### Comparing `gigachain-0.1.9/langchain/memory/simple.py` & `gigachain-0.2.0/langchain/memory/simple.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/memory/summary.py` & `gigachain-0.2.0/langchain/memory/summary_buffer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,51 @@
-from __future__ import annotations
+from typing import Any, Dict, List, Union
 
-from typing import Any, Dict, List, Type
+from langchain_core.messages import BaseMessage, get_buffer_string
+from langchain_core.pydantic_v1 import root_validator
 
-from langchain_core.chat_history import BaseChatMessageHistory
-from langchain_core.language_models import BaseLanguageModel
-from langchain_core.messages import BaseMessage, SystemMessage, get_buffer_string
-from langchain_core.prompts import BasePromptTemplate
-from langchain_core.pydantic_v1 import BaseModel, root_validator
-
-from langchain.chains.llm import LLMChain
 from langchain.memory.chat_memory import BaseChatMemory
-from langchain.memory.prompt import SUMMARY_PROMPT
+from langchain.memory.summary import SummarizerMixin
 
 
-class SummarizerMixin(BaseModel):
-    """Mixin for summarizer."""
+class ConversationSummaryBufferMemory(BaseChatMemory, SummarizerMixin):
+    """Buffer with summarizer for storing conversation memory."""
 
-    human_prefix: str = "Human"
-    ai_prefix: str = "AI"
-    llm: BaseLanguageModel
-    prompt: BasePromptTemplate = SUMMARY_PROMPT
-    summary_message_cls: Type[BaseMessage] = SystemMessage
-
-    def predict_new_summary(
-        self, messages: List[BaseMessage], existing_summary: str
-    ) -> str:
-        new_lines = get_buffer_string(
-            messages,
-            human_prefix=self.human_prefix,
-            ai_prefix=self.ai_prefix,
-        )
-
-        chain = LLMChain(llm=self.llm, prompt=self.prompt)
-        return chain.predict(summary=existing_summary, new_lines=new_lines)
-
-
-class ConversationSummaryMemory(BaseChatMemory, SummarizerMixin):
-    """Conversation summarizer to chat memory."""
-
-    buffer: str = ""
-    memory_key: str = "history"  #: :meta private:
-
-    @classmethod
-    def from_messages(
-        cls,
-        llm: BaseLanguageModel,
-        chat_memory: BaseChatMessageHistory,
-        *,
-        summarize_step: int = 2,
-        **kwargs: Any,
-    ) -> ConversationSummaryMemory:
-        obj = cls(llm=llm, chat_memory=chat_memory, **kwargs)
-        for i in range(0, len(obj.chat_memory.messages), summarize_step):
-            obj.buffer = obj.predict_new_summary(
-                obj.chat_memory.messages[i : i + summarize_step], obj.buffer
-            )
-        return obj
+    max_token_limit: int = 2000
+    moving_summary_buffer: str = ""
+    memory_key: str = "history"
+
+    @property
+    def buffer(self) -> Union[str, List[BaseMessage]]:
+        """String buffer of memory."""
+        return self.load_memory_variables({})[self.memory_key]
 
     @property
     def memory_variables(self) -> List[str]:
         """Will always return list of memory variables.
 
         :meta private:
         """
         return [self.memory_key]
 
     def load_memory_variables(self, inputs: Dict[str, Any]) -> Dict[str, Any]:
         """Return history buffer."""
+        buffer = self.chat_memory.messages
+        if self.moving_summary_buffer != "":
+            first_messages: List[BaseMessage] = [
+                self.summary_message_cls(content=self.moving_summary_buffer)
+            ]
+            buffer = first_messages + buffer
         if self.return_messages:
-            buffer: Any = [self.summary_message_cls(content=self.buffer)]
+            final_buffer: Any = buffer
         else:
-            buffer = self.buffer
-        return {self.memory_key: buffer}
+            final_buffer = get_buffer_string(
+                buffer, human_prefix=self.human_prefix, ai_prefix=self.ai_prefix
+            )
+        return {self.memory_key: final_buffer}
 
     @root_validator()
     def validate_prompt_input_variables(cls, values: Dict) -> Dict:
         """Validate that prompt input variables are consistent."""
         prompt_variables = values["prompt"].input_variables
         expected_keys = {"summary", "new_lines"}
         if expected_keys != set(prompt_variables):
@@ -84,15 +54,26 @@
                 f"{prompt_variables}, but it should have {expected_keys}."
             )
         return values
 
     def save_context(self, inputs: Dict[str, Any], outputs: Dict[str, str]) -> None:
         """Save context from this conversation to buffer."""
         super().save_context(inputs, outputs)
-        self.buffer = self.predict_new_summary(
-            self.chat_memory.messages[-2:], self.buffer
-        )
+        self.prune()
+
+    def prune(self) -> None:
+        """Prune buffer if it exceeds max token limit"""
+        buffer = self.chat_memory.messages
+        curr_buffer_length = self.llm.get_num_tokens_from_messages(buffer)
+        if curr_buffer_length > self.max_token_limit:
+            pruned_memory = []
+            while curr_buffer_length > self.max_token_limit:
+                pruned_memory.append(buffer.pop(0))
+                curr_buffer_length = self.llm.get_num_tokens_from_messages(buffer)
+            self.moving_summary_buffer = self.predict_new_summary(
+                pruned_memory, self.moving_summary_buffer
+            )
 
     def clear(self) -> None:
         """Clear memory contents."""
         super().clear()
-        self.buffer = ""
+        self.moving_summary_buffer = ""
```

### Comparing `gigachain-0.1.9/langchain/memory/summary_buffer.py` & `gigachain-0.2.0/langchain/memory/token_buffer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,78 +1,59 @@
 from typing import Any, Dict, List
 
+from langchain_core.language_models import BaseLanguageModel
 from langchain_core.messages import BaseMessage, get_buffer_string
-from langchain_core.pydantic_v1 import root_validator
 
 from langchain.memory.chat_memory import BaseChatMemory
-from langchain.memory.summary import SummarizerMixin
 
 
-class ConversationSummaryBufferMemory(BaseChatMemory, SummarizerMixin):
-    """Buffer with summarizer for storing conversation memory."""
+class ConversationTokenBufferMemory(BaseChatMemory):
+    """Conversation chat memory with token limit."""
 
-    max_token_limit: int = 2000
-    moving_summary_buffer: str = ""
+    human_prefix: str = "Human"
+    ai_prefix: str = "AI"
+    llm: BaseLanguageModel
     memory_key: str = "history"
+    max_token_limit: int = 2000
+
+    @property
+    def buffer(self) -> Any:
+        """String buffer of memory."""
+        return self.buffer_as_messages if self.return_messages else self.buffer_as_str
 
     @property
-    def buffer(self) -> List[BaseMessage]:
+    def buffer_as_str(self) -> str:
+        """Exposes the buffer as a string in case return_messages is False."""
+        return get_buffer_string(
+            self.chat_memory.messages,
+            human_prefix=self.human_prefix,
+            ai_prefix=self.ai_prefix,
+        )
+
+    @property
+    def buffer_as_messages(self) -> List[BaseMessage]:
+        """Exposes the buffer as a list of messages in case return_messages is True."""
         return self.chat_memory.messages
 
     @property
     def memory_variables(self) -> List[str]:
         """Will always return list of memory variables.
 
         :meta private:
         """
         return [self.memory_key]
 
     def load_memory_variables(self, inputs: Dict[str, Any]) -> Dict[str, Any]:
         """Return history buffer."""
-        buffer = self.buffer
-        if self.moving_summary_buffer != "":
-            first_messages: List[BaseMessage] = [
-                self.summary_message_cls(content=self.moving_summary_buffer)
-            ]
-            buffer = first_messages + buffer
-        if self.return_messages:
-            final_buffer: Any = buffer
-        else:
-            final_buffer = get_buffer_string(
-                buffer, human_prefix=self.human_prefix, ai_prefix=self.ai_prefix
-            )
-        return {self.memory_key: final_buffer}
-
-    @root_validator()
-    def validate_prompt_input_variables(cls, values: Dict) -> Dict:
-        """Validate that prompt input variables are consistent."""
-        prompt_variables = values["prompt"].input_variables
-        expected_keys = {"summary", "new_lines"}
-        if expected_keys != set(prompt_variables):
-            raise ValueError(
-                "Got unexpected prompt input variables. The prompt expects "
-                f"{prompt_variables}, but it should have {expected_keys}."
-            )
-        return values
+        return {self.memory_key: self.buffer}
 
     def save_context(self, inputs: Dict[str, Any], outputs: Dict[str, str]) -> None:
-        """Save context from this conversation to buffer."""
+        """Save context from this conversation to buffer. Pruned."""
         super().save_context(inputs, outputs)
-        self.prune()
-
-    def prune(self) -> None:
-        """Prune buffer if it exceeds max token limit"""
+        # Prune buffer if it exceeds max token limit
         buffer = self.chat_memory.messages
         curr_buffer_length = self.llm.get_num_tokens_from_messages(buffer)
         if curr_buffer_length > self.max_token_limit:
             pruned_memory = []
             while curr_buffer_length > self.max_token_limit:
                 pruned_memory.append(buffer.pop(0))
                 curr_buffer_length = self.llm.get_num_tokens_from_messages(buffer)
-            self.moving_summary_buffer = self.predict_new_summary(
-                pruned_memory, self.moving_summary_buffer
-            )
-
-    def clear(self) -> None:
-        """Clear memory contents."""
-        super().clear()
-        self.moving_summary_buffer = ""
```

### Comparing `gigachain-0.1.9/langchain/memory/utils.py` & `gigachain-0.2.0/langchain/memory/utils.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/model_laboratory.py` & `gigachain-0.2.0/langchain/model_laboratory.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/output_parsers/boolean.py` & `gigachain-0.2.0/langchain/output_parsers/boolean.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import re
+
 from langchain_core.output_parsers import BaseOutputParser
 
 
 class BooleanOutputParser(BaseOutputParser[bool]):
     """Parse the output of an LLM call to a boolean."""
 
     true_val: str = "YES"
@@ -13,32 +15,37 @@
         """Parse the output of an LLM call to a boolean.
 
         Args:
             text: output of a language model
 
         Returns:
             boolean
-
         """
-        cleaned_upper_text = text.strip().upper()
-        if (
-            self.true_val.upper() in cleaned_upper_text
-            and self.false_val.upper() in cleaned_upper_text
-        ):
-            raise ValueError(
-                f"Ambiguous response. Both {self.true_val} and {self.false_val} in "
-                f"received: {text}."
-            )
-        elif self.true_val.upper() in cleaned_upper_text:
+        regexp = rf"\b({self.true_val}|{self.false_val})\b"
+
+        truthy = {
+            val.upper()
+            for val in re.findall(regexp, text, flags=re.IGNORECASE | re.MULTILINE)
+        }
+        if self.true_val.upper() in truthy:
+            if self.false_val.upper() in truthy:
+                raise ValueError(
+                    f"Ambiguous response. Both {self.true_val} and {self.false_val} "
+                    f"in received: {text}."
+                )
             return True
-        elif self.false_val.upper() in cleaned_upper_text:
+        elif self.false_val.upper() in truthy:
+            if self.true_val.upper() in truthy:
+                raise ValueError(
+                    f"Ambiguous response. Both {self.true_val} and {self.false_val} "
+                    f"in received: {text}."
+                )
             return False
-        else:
-            raise ValueError(
-                f"BooleanOutputParser expected output value to include either "
-                f"{self.true_val} or {self.false_val}. Received {text}."
-            )
+        raise ValueError(
+            f"BooleanOutputParser expected output value to include either "
+            f"{self.true_val} or {self.false_val}. Received {text}."
+        )
 
     @property
     def _type(self) -> str:
         """Snake-case string identifier for an output parser type."""
         return "boolean_output_parser"
```

### Comparing `gigachain-0.1.9/langchain/output_parsers/combining.py` & `gigachain-0.2.0/langchain/output_parsers/combining.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/output_parsers/datetime.py` & `gigachain-0.2.0/langchain/output_parsers/datetime.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/output_parsers/enum.py` & `gigachain-0.2.0/langchain/output_parsers/enum.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/output_parsers/fix.py` & `gigachain-0.2.0/langchain/output_parsers/fix.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from langchain.output_parsers.prompts import NAIVE_FIX_PROMPT
 
 T = TypeVar("T")
 
 
 class OutputFixingParser(BaseOutputParser[T]):
-    """Wraps a parser and tries to fix parsing errors."""
+    """Wrap a parser and try to fix parsing errors."""
 
     @classmethod
     def is_lc_serializable(cls) -> bool:
         return True
 
     parser: BaseOutputParser[T]
     """The parser to use to parse the output."""
```

### Comparing `gigachain-0.1.9/langchain/output_parsers/format_instructions.py` & `gigachain-0.2.0/langchain/output_parsers/format_instructions.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/output_parsers/loading.py` & `gigachain-0.2.0/langchain/output_parsers/loading.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/output_parsers/pandas_dataframe.py` & `gigachain-0.2.0/langchain/output_parsers/pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/output_parsers/prompts.py` & `gigachain-0.2.0/langchain/output_parsers/prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/output_parsers/regex.py` & `gigachain-0.2.0/langchain/output_parsers/regex.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/output_parsers/regex_dict.py` & `gigachain-0.2.0/langchain/output_parsers/regex_dict.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/output_parsers/retry.py` & `gigachain-0.2.0/langchain/output_parsers/retry.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     NAIVE_COMPLETION_RETRY_WITH_ERROR
 )
 
 T = TypeVar("T")
 
 
 class RetryOutputParser(BaseOutputParser[T]):
-    """Wraps a parser and tries to fix parsing errors.
+    """Wrap a parser and try to fix parsing errors.
 
     Does this by passing the original prompt and the completion to another
     LLM, and telling it the completion did not satisfy criteria in the prompt.
     """
 
     parser: BaseOutputParser[T]
     """The parser to use to parse the output."""
@@ -134,15 +134,15 @@
 
     @property
     def _type(self) -> str:
         return "retry"
 
 
 class RetryWithErrorOutputParser(BaseOutputParser[T]):
-    """Wraps a parser and tries to fix parsing errors.
+    """Wrap a parser and try to fix parsing errors.
 
     Does this by passing the original prompt, the completion, AND the error
     that was raised to another language model and telling it that the completion
     did not work, and raised the given error. Differs from RetryOutputParser
     in that this implementation provides the error that was raised back to the
     LLM, which in theory should give it more information on how to fix it.
     """
```

### Comparing `gigachain-0.1.9/langchain/output_parsers/structured.py` & `gigachain-0.2.0/langchain/output_parsers/structured.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     STRUCTURED_FORMAT_SIMPLE_INSTRUCTIONS,
 )
 
 line_template = '\t"{name}": {type}  // {description}'
 
 
 class ResponseSchema(BaseModel):
-    """A schema for a response from a structured output parser."""
+    """Schema for a response from a structured output parser."""
 
     name: str
     """The name of the schema."""
     description: str
     """The description of the schema."""
     type: str = "string"
     """The type of the response."""
```

### Comparing `gigachain-0.1.9/langchain/output_parsers/yaml.py` & `gigachain-0.2.0/langchain/output_parsers/yaml.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/prompts/base.py` & `gigachain-0.2.0/langchain/prompts/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/prompts/chat.py` & `gigachain-0.2.0/langchain/prompts/chat.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/prompts/loading.py` & `gigachain-0.2.0/langchain/prompts/loading.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/pydantic_v1/__init__.py` & `gigachain-0.2.0/langchain/pydantic_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/retrievers/contextual_compression.py` & `gigachain-0.2.0/langchain/retrievers/contextual_compression.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 
         Args:
             query: string to find relevant documents for
 
         Returns:
             Sequence of relevant documents
         """
-        docs = self.base_retriever.get_relevant_documents(
-            query, callbacks=run_manager.get_child(), **kwargs
+        docs = self.base_retriever.invoke(
+            query, config={"callbacks": run_manager.get_child()}, **kwargs
         )
         if docs:
             compressed_docs = self.base_compressor.compress_documents(
                 docs, query, callbacks=run_manager.get_child()
             )
             return list(compressed_docs)
         else:
@@ -63,16 +63,16 @@
 
         Args:
             query: string to find relevant documents for
 
         Returns:
             List of relevant documents
         """
-        docs = await self.base_retriever.aget_relevant_documents(
-            query, callbacks=run_manager.get_child(), **kwargs
+        docs = await self.base_retriever.ainvoke(
+            query, config={"callbacks": run_manager.get_child()}, **kwargs
         )
         if docs:
             compressed_docs = await self.base_compressor.acompress_documents(
                 docs, query, callbacks=run_manager.get_child()
             )
             return list(compressed_docs)
         else:
```

### Comparing `gigachain-0.1.9/langchain/retrievers/document_compressors/base.py` & `gigachain-0.2.0/langchain/retrievers/document_compressors/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from inspect import signature
 from typing import List, Optional, Sequence, Union
 
+from langchain_core.callbacks.manager import Callbacks
 from langchain_core.documents import (
     BaseDocumentCompressor,
     BaseDocumentTransformer,
     Document,
 )
 
-from langchain.callbacks.manager import Callbacks
-
 
 class DocumentCompressorPipeline(BaseDocumentCompressor):
     """Document compressor that uses a pipeline of Transformers."""
 
     transformers: List[Union[BaseDocumentTransformer, BaseDocumentCompressor]]
     """List of document filters that are chained together and run in sequence."""
```

### Comparing `gigachain-0.1.9/langchain/retrievers/document_compressors/chain_extract.py` & `gigachain-0.2.0/langchain/retrievers/document_compressors/chain_extract.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """DocumentFilter that uses an LLM chain to extract the relevant parts of documents."""
+
 from __future__ import annotations
 
 import asyncio
 from typing import Any, Callable, Dict, Optional, Sequence, cast
 
+from langchain_core.callbacks.manager import Callbacks
 from langchain_core.documents import Document
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.output_parsers import BaseOutputParser
 from langchain_core.prompts import PromptTemplate
 
-from langchain.callbacks.manager import Callbacks
 from langchain.chains.llm import LLMChain
 from langchain.retrievers.document_compressors.base import BaseDocumentCompressor
 from langchain.retrievers.document_compressors.chain_extract_prompt import (
     prompt_template,
 )
 
 
@@ -60,15 +61,18 @@
         query: str,
         callbacks: Optional[Callbacks] = None,
     ) -> Sequence[Document]:
         """Compress page content of raw documents."""
         compressed_docs = []
         for doc in documents:
             _input = self.get_input(query, doc)
-            output = self.llm_chain.predict_and_parse(**_input, callbacks=callbacks)
+            output_dict = self.llm_chain.invoke(_input, config={"callbacks": callbacks})
+            output = output_dict[self.llm_chain.output_key]
+            if self.llm_chain.prompt.output_parser is not None:
+                output = self.llm_chain.prompt.output_parser.parse(output)
             if len(output) == 0:
                 continue
             compressed_docs.append(
                 Document(page_content=cast(str, output), metadata=doc.metadata)
             )
         return compressed_docs
 
@@ -88,15 +92,15 @@
             ]
         )
         compressed_docs = []
         for i, doc in enumerate(documents):
             if len(outputs[i]) == 0:
                 continue
             compressed_docs.append(
-                Document(page_content=outputs[i], metadata=doc.metadata)
+                Document(page_content=outputs[i], metadata=doc.metadata)  # type: ignore[arg-type]
             )
         return compressed_docs
 
     @classmethod
     def from_llm(
         cls,
         llm: BaseLanguageModel,
@@ -104,8 +108,8 @@
         get_input: Optional[Callable[[str, Document], str]] = None,
         llm_chain_kwargs: Optional[dict] = None,
     ) -> LLMChainExtractor:
         """Initialize from LLM."""
         _prompt = prompt if prompt is not None else _get_default_chain_prompt()
         _get_input = get_input if get_input is not None else default_get_input
         llm_chain = LLMChain(llm=llm, prompt=_prompt, **(llm_chain_kwargs or {}))
-        return cls(llm_chain=llm_chain, get_input=_get_input)
+        return cls(llm_chain=llm_chain, get_input=_get_input)  # type: ignore[arg-type]
```

### Comparing `gigachain-0.1.9/langchain/retrievers/document_compressors/chain_extract_prompt.py` & `gigachain-0.2.0/langchain/retrievers/document_compressors/chain_extract_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/retrievers/document_compressors/chain_filter.py` & `gigachain-0.2.0/langchain/retrievers/document_compressors/chain_filter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Filter that uses an LLM to drop documents that aren't relevant to the query."""
+
 from typing import Any, Callable, Dict, Optional, Sequence
 
+from langchain_core.callbacks.manager import Callbacks
 from langchain_core.documents import Document
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.prompts import BasePromptTemplate, PromptTemplate
 
-from langchain.callbacks.manager import Callbacks
 from langchain.chains import LLMChain
 from langchain.output_parsers.boolean import BooleanOutputParser
 from langchain.retrievers.document_compressors.base import BaseDocumentCompressor
 from langchain.retrievers.document_compressors.chain_filter_prompt import (
     prompt_template,
 )
 
@@ -43,17 +44,18 @@
         query: str,
         callbacks: Optional[Callbacks] = None,
     ) -> Sequence[Document]:
         """Filter down documents based on their relevance to the query."""
         filtered_docs = []
         for doc in documents:
             _input = self.get_input(query, doc)
-            include_doc = self.llm_chain.predict_and_parse(
-                **_input, callbacks=callbacks
-            )
+            output_dict = self.llm_chain.invoke(_input, config={"callbacks": callbacks})
+            output = output_dict[self.llm_chain.output_key]
+            if self.llm_chain.prompt.output_parser is not None:
+                include_doc = self.llm_chain.prompt.output_parser.parse(output)
             if include_doc:
                 filtered_docs.append(doc)
         return filtered_docs
 
     @classmethod
     def from_llm(
         cls,
```

### Comparing `gigachain-0.1.9/langchain/retrievers/document_compressors/cohere_rerank.py` & `gigachain-0.2.0/langchain/retrievers/document_compressors/cohere_rerank.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from __future__ import annotations
 
 from copy import deepcopy
 from typing import Any, Dict, List, Optional, Sequence, Union
 
+from langchain_core._api.deprecation import deprecated
+from langchain_core.callbacks.manager import Callbacks
 from langchain_core.documents import Document
 from langchain_core.pydantic_v1 import Extra, root_validator
+from langchain_core.utils import get_from_dict_or_env
 
-from langchain.callbacks.manager import Callbacks
 from langchain.retrievers.document_compressors.base import BaseDocumentCompressor
-from langchain.utils import get_from_dict_or_env
 
 
+@deprecated(
+    since="0.0.30", removal="0.3.0", alternative_import="langchain_cohere.CohereRerank"
+)
 class CohereRerank(BaseDocumentCompressor):
     """Document compressor that uses `Cohere Rerank API`."""
 
     client: Any = None
     """Cohere client to use for compressing documents."""
     top_n: Optional[int] = 3
     """Number of documents to return."""
@@ -73,16 +77,22 @@
             return []
         docs = [
             doc.page_content if isinstance(doc, Document) else doc for doc in documents
         ]
         model = model or self.model
         top_n = top_n if (top_n is None or top_n > 0) else self.top_n
         results = self.client.rerank(
-            query, docs, model, top_n=top_n, max_chunks_per_doc=max_chunks_per_doc
+            query=query,
+            documents=docs,
+            model=model,
+            top_n=top_n,
+            max_chunks_per_doc=max_chunks_per_doc,
         )
+        if hasattr(results, "results"):
+            results = getattr(results, "results")
         result_dicts = []
         for res in results:
             result_dicts.append(
                 {"index": res.index, "relevance_score": res.relevance_score}
             )
         return result_dicts
```

### Comparing `gigachain-0.1.9/langchain/retrievers/document_compressors/embeddings_filter.py` & `gigachain-0.2.0/langchain/retrievers/document_compressors/embeddings_filter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 from typing import Callable, Dict, Optional, Sequence
 
 import numpy as np
-from langchain_community.document_transformers.embeddings_redundant_filter import (
-    _get_embeddings_from_stateful_docs,
-    get_stateful_documents,
-)
+from langchain_core.callbacks.manager import Callbacks
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
-from langchain_core.pydantic_v1 import root_validator
+from langchain_core.pydantic_v1 import Field, root_validator
 
-from langchain.callbacks.manager import Callbacks
 from langchain.retrievers.document_compressors.base import (
     BaseDocumentCompressor,
 )
-from langchain.utils.math import cosine_similarity
+
+
+def _get_similarity_function() -> Callable:
+    try:
+        from langchain_community.utils.math import cosine_similarity
+    except ImportError:
+        raise ImportError(
+            "To use please install langchain-community "
+            "with `pip install langchain-community`."
+        )
+    return cosine_similarity
 
 
 class EmbeddingsFilter(BaseDocumentCompressor):
     """Document compressor that uses embeddings to drop documents
     unrelated to the query."""
 
     embeddings: Embeddings
     """Embeddings to use for embedding document contents and queries."""
-    similarity_fn: Callable = cosine_similarity
+    similarity_fn: Callable = Field(default_factory=_get_similarity_function)
     """Similarity function for comparing documents. Function expected to take as input
     two matrices (List[List[float]]) and return a matrix of scores where higher values
     indicate greater similarity."""
     k: Optional[int] = 20
     """The number of relevant documents to return. Can be set to None, in which case
     `similarity_threshold` must be specified. Defaults to 20."""
     similarity_threshold: Optional[float]
@@ -49,14 +55,24 @@
     def compress_documents(
         self,
         documents: Sequence[Document],
         query: str,
         callbacks: Optional[Callbacks] = None,
     ) -> Sequence[Document]:
         """Filter documents based on similarity of their embeddings to the query."""
+        try:
+            from langchain_community.document_transformers.embeddings_redundant_filter import (  # noqa: E501
+                _get_embeddings_from_stateful_docs,
+                get_stateful_documents,
+            )
+        except ImportError:
+            raise ImportError(
+                "To use please install langchain-community "
+                "with `pip install langchain-community`."
+            )
         stateful_documents = get_stateful_documents(documents)
         embedded_documents = _get_embeddings_from_stateful_docs(
             self.embeddings, stateful_documents
         )
         embedded_query = self.embeddings.embed_query(query)
         similarity = self.similarity_fn([embedded_query], embedded_documents)[0]
         included_idxs = np.arange(len(embedded_documents))
```

### Comparing `gigachain-0.1.9/langchain/retrievers/ensemble.py` & `gigachain-0.2.0/langchain/retrievers/ensemble.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,27 @@
 """
-Ensemble retriever that ensemble the results of 
+Ensemble retriever that ensemble the results of
 multiple retrievers by using weighted  Reciprocal Rank Fusion
 """
+
 import asyncio
-from typing import Any, Dict, List, Optional, cast
+from collections import defaultdict
+from collections.abc import Hashable
+from itertools import chain
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    TypeVar,
+    cast,
+)
 
 from langchain_core.callbacks import (
     AsyncCallbackManagerForRetrieverRun,
     CallbackManagerForRetrieverRun,
 )
 from langchain_core.documents import Document
 from langchain_core.load.dump import dumpd
@@ -16,14 +30,34 @@
 from langchain_core.runnables import RunnableConfig
 from langchain_core.runnables.config import ensure_config, patch_config
 from langchain_core.runnables.utils import (
     ConfigurableFieldSpec,
     get_unique_config_specs,
 )
 
+T = TypeVar("T")
+H = TypeVar("H", bound=Hashable)
+
+
+def unique_by_key(iterable: Iterable[T], key: Callable[[T], H]) -> Iterator[T]:
+    """Yield unique elements of an iterable based on a key function.
+
+    Args:
+        iterable: The iterable to filter.
+        key: A function that returns a hashable key for each element.
+
+    Yields:
+        Unique elements of the iterable based on the key function.
+    """
+    seen = set()
+    for e in iterable:
+        if (k := key(e)) not in seen:
+            seen.add(k)
+            yield e
+
 
 class EnsembleRetriever(BaseRetriever):
     """Retriever that ensembles the multiple retrievers.
 
     It uses a rank fusion.
 
     Args:
@@ -234,15 +268,15 @@
                 for i, retriever in enumerate(self.retrievers)
             ]
         )
 
         # Enforce that retrieved docs are Documents for each list in retriever_docs
         for i in range(len(retriever_docs)):
             retriever_docs[i] = [
-                Document(page_content=doc) if not isinstance(doc, Document) else doc
+                Document(page_content=doc) if not isinstance(doc, Document) else doc  # type: ignore[arg-type]
                 for doc in retriever_docs[i]
             ]
 
         # apply rank fusion
         fused_documents = self.weighted_reciprocal_rank(retriever_docs)
 
         return fused_documents
@@ -263,36 +297,22 @@
                     scores in descending order.
         """
         if len(doc_lists) != len(self.weights):
             raise ValueError(
                 "Number of rank lists must be equal to the number of weights."
             )
 
-        # Create a union of all unique documents in the input doc_lists
-        all_documents = set()
-        for doc_list in doc_lists:
-            for doc in doc_list:
-                all_documents.add(doc.page_content)
-
-        # Initialize the RRF score dictionary for each document
-        rrf_score_dic = {doc: 0.0 for doc in all_documents}
-
-        # Calculate RRF scores for each document
+        # Associate each doc's content with its RRF score for later sorting by it
+        # Duplicated contents across retrievers are collapsed & scored cumulatively
+        rrf_score: Dict[str, float] = defaultdict(float)
         for doc_list, weight in zip(doc_lists, self.weights):
             for rank, doc in enumerate(doc_list, start=1):
-                rrf_score = weight * (1 / (rank + self.c))
-                rrf_score_dic[doc.page_content] += rrf_score
+                rrf_score[doc.page_content] += weight / (rank + self.c)
 
-        # Sort documents by their RRF scores in descending order
-        sorted_documents = sorted(
-            rrf_score_dic.keys(), key=lambda x: rrf_score_dic[x], reverse=True
+        # Docs are deduplicated by their contents then sorted by their scores
+        all_docs = chain.from_iterable(doc_lists)
+        sorted_docs = sorted(
+            unique_by_key(all_docs, lambda doc: doc.page_content),
+            reverse=True,
+            key=lambda doc: rrf_score[doc.page_content],
         )
-
-        # Map the sorted page_content back to the original document objects
-        page_content_to_doc_map = {
-            doc.page_content: doc for doc_list in doc_lists for doc in doc_list
-        }
-        sorted_docs = [
-            page_content_to_doc_map[page_content] for page_content in sorted_documents
-        ]
-
         return sorted_docs
```

### Comparing `gigachain-0.1.9/langchain/retrievers/merger_retriever.py` & `gigachain-0.2.0/langchain/retrievers/merger_retriever.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,23 +68,26 @@
 
         Returns:
             A list of merged documents.
         """
 
         # Get the results of all retrievers.
         retriever_docs = [
-            retriever.get_relevant_documents(
-                query, callbacks=run_manager.get_child("retriever_{}".format(i + 1))
+            retriever.invoke(
+                query,
+                config={
+                    "callbacks": run_manager.get_child("retriever_{}".format(i + 1))
+                },
             )
             for i, retriever in enumerate(self.retrievers)
         ]
 
         # Merge the results of the retrievers.
         merged_documents = []
-        max_docs = max(len(docs) for docs in retriever_docs)
+        max_docs = max(map(len, retriever_docs), default=0)
         for i in range(max_docs):
             for retriever, doc in zip(self.retrievers, retriever_docs):
                 if i < len(doc):
                     merged_documents.append(doc[i])
 
         return merged_documents
 
@@ -100,23 +103,26 @@
         Returns:
             A list of merged documents.
         """
 
         # Get the results of all retrievers.
         retriever_docs = await asyncio.gather(
             *(
-                retriever.aget_relevant_documents(
-                    query, callbacks=run_manager.get_child("retriever_{}".format(i + 1))
+                retriever.ainvoke(
+                    query,
+                    config={
+                        "callbacks": run_manager.get_child("retriever_{}".format(i + 1))
+                    },
                 )
                 for i, retriever in enumerate(self.retrievers)
             )
         )
 
         # Merge the results of the retrievers.
         merged_documents = []
-        max_docs = max(len(docs) for docs in retriever_docs)
+        max_docs = max(map(len, retriever_docs), default=0)
         for i in range(max_docs):
             for retriever, doc in zip(self.retrievers, retriever_docs):
                 if i < len(doc):
                     merged_documents.append(doc[i])
 
         return merged_documents
```

### Comparing `gigachain-0.1.9/langchain/retrievers/multi_query.py` & `gigachain-0.2.0/langchain/retrievers/multi_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,16 +132,16 @@
             queries: query list
 
         Returns:
             List of retrieved Documents
         """
         document_lists = await asyncio.gather(
             *(
-                self.retriever.aget_relevant_documents(
-                    query, callbacks=run_manager.get_child()
+                self.retriever.ainvoke(
+                    query, config={"callbacks": run_manager.get_child()}
                 )
                 for query in queries
             )
         )
         return [doc for docs in document_lists for doc in docs]
 
     def _get_relevant_documents(
@@ -192,16 +192,16 @@
             queries: query list
 
         Returns:
             List of retrieved Documents
         """
         documents = []
         for query in queries:
-            docs = self.retriever.get_relevant_documents(
-                query, callbacks=run_manager.get_child()
+            docs = self.retriever.invoke(
+                query, config={"callbacks": run_manager.get_child()}
             )
             documents.extend(docs)
         return documents
 
     def unique_union(self, documents: List[Document]) -> List[Document]:
         """Get unique Documents.
```

### Comparing `gigachain-0.1.9/langchain/retrievers/multi_vector.py` & `gigachain-0.2.0/langchain/retrievers/multi_vector.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/retrievers/parent_document_retriever.py` & `gigachain-0.2.0/langchain/retrievers/parent_document_retriever.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import uuid
 from typing import List, Optional, Sequence
 
 from langchain_core.documents import Document
+from langchain_text_splitters import TextSplitter
 
 from langchain.retrievers import MultiVectorRetriever
-from langchain.text_splitter import TextSplitter
 
 
 class ParentDocumentRetriever(MultiVectorRetriever):
     """Retrieve small chunks then retrieve their parent documents.
 
     When splitting documents for retrieval, there are often conflicting desires:
 
@@ -29,15 +29,15 @@
 
     Examples:
 
         .. code-block:: python
 
             from langchain_community.embeddings import OpenAIEmbeddings
             from langchain_community.vectorstores import Chroma
-            from langchain.text_splitter import RecursiveCharacterTextSplitter
+            from langchain_text_splitters import RecursiveCharacterTextSplitter
             from langchain.storage import InMemoryStore
 
             # This text splitter is used to create the parent documents
             parent_splitter = RecursiveCharacterTextSplitter(chunk_size=2000, add_start_index=True)
             # This text splitter is used to create the child documents
             # It should create documents smaller than the parent
             child_splitter = RecursiveCharacterTextSplitter(chunk_size=400, add_start_index=True)
```

### Comparing `gigachain-0.1.9/langchain/retrievers/re_phraser.py` & `gigachain-0.2.0/langchain/retrievers/re_phraser.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,16 +71,16 @@
 
         Returns:
             Relevant documents for re-phrased question
         """
         response = self.llm_chain(query, callbacks=run_manager.get_child())
         re_phrased_question = response["text"]
         logger.info(f"Re-phrased question: {re_phrased_question}")
-        docs = self.retriever.get_relevant_documents(
-            re_phrased_question, callbacks=run_manager.get_child()
+        docs = self.retriever.invoke(
+            re_phrased_question, config={"callbacks": run_manager.get_child()}
         )
         return docs
 
     async def _aget_relevant_documents(
         self,
         query: str,
         *,
```

### Comparing `gigachain-0.1.9/langchain/retrievers/time_weighted_retriever.py` & `gigachain-0.2.0/langchain/retrievers/time_weighted_retriever.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import datetime
 from copy import deepcopy
 from typing import Any, Dict, List, Optional, Tuple
 
-from langchain_core.callbacks import CallbackManagerForRetrieverRun
+from langchain_core.callbacks import (
+    AsyncCallbackManagerForRetrieverRun,
+    CallbackManagerForRetrieverRun,
+)
 from langchain_core.documents import Document
 from langchain_core.pydantic_v1 import Field
 from langchain_core.retrievers import BaseRetriever
 from langchain_core.vectorstores import VectorStore
 
 
 def _get_hours_passed(time: datetime.datetime, ref_time: datetime.datetime) -> float:
@@ -85,39 +88,70 @@
         for fetched_doc, relevance in docs_and_scores:
             if "buffer_idx" in fetched_doc.metadata:
                 buffer_idx = fetched_doc.metadata["buffer_idx"]
                 doc = self.memory_stream[buffer_idx]
                 results[buffer_idx] = (doc, relevance)
         return results
 
-    def _get_relevant_documents(
-        self, query: str, *, run_manager: CallbackManagerForRetrieverRun
+    async def aget_salient_docs(self, query: str) -> Dict[int, Tuple[Document, float]]:
+        """Return documents that are salient to the query."""
+        docs_and_scores: List[Tuple[Document, float]]
+        docs_and_scores = (
+            await self.vectorstore.asimilarity_search_with_relevance_scores(
+                query, **self.search_kwargs
+            )
+        )
+        results = {}
+        for fetched_doc, relevance in docs_and_scores:
+            if "buffer_idx" in fetched_doc.metadata:
+                buffer_idx = fetched_doc.metadata["buffer_idx"]
+                doc = self.memory_stream[buffer_idx]
+                results[buffer_idx] = (doc, relevance)
+        return results
+
+    def _get_rescored_docs(
+        self, docs_and_scores: Dict[Any, Tuple[Document, Optional[float]]]
     ) -> List[Document]:
-        """Return documents that are relevant to the query."""
         current_time = datetime.datetime.now()
-        docs_and_scores = {
-            doc.metadata["buffer_idx"]: (doc, self.default_salience)
-            for doc in self.memory_stream[-self.k :]
-        }
-        # If a doc is considered salient, update the salience score
-        docs_and_scores.update(self.get_salient_docs(query))
         rescored_docs = [
             (doc, self._get_combined_score(doc, relevance, current_time))
             for doc, relevance in docs_and_scores.values()
         ]
         rescored_docs.sort(key=lambda x: x[1], reverse=True)
         result = []
         # Ensure frequently accessed memories aren't forgotten
         for doc, _ in rescored_docs[: self.k]:
             # TODO: Update vector store doc once `update` method is exposed.
             buffered_doc = self.memory_stream[doc.metadata["buffer_idx"]]
             buffered_doc.metadata["last_accessed_at"] = current_time
             result.append(buffered_doc)
         return result
 
+    def _get_relevant_documents(
+        self, query: str, *, run_manager: CallbackManagerForRetrieverRun
+    ) -> List[Document]:
+        docs_and_scores = {
+            doc.metadata["buffer_idx"]: (doc, self.default_salience)
+            for doc in self.memory_stream[-self.k :]
+        }
+        # If a doc is considered salient, update the salience score
+        docs_and_scores.update(self.get_salient_docs(query))
+        return self._get_rescored_docs(docs_and_scores)
+
+    async def _aget_relevant_documents(
+        self, query: str, *, run_manager: AsyncCallbackManagerForRetrieverRun
+    ) -> List[Document]:
+        docs_and_scores = {
+            doc.metadata["buffer_idx"]: (doc, self.default_salience)
+            for doc in self.memory_stream[-self.k :]
+        }
+        # If a doc is considered salient, update the salience score
+        docs_and_scores.update(await self.aget_salient_docs(query))
+        return self._get_rescored_docs(docs_and_scores)
+
     def add_documents(self, documents: List[Document], **kwargs: Any) -> List[str]:
         """Add documents to vectorstore."""
         current_time = kwargs.get("current_time")
         if current_time is None:
             current_time = datetime.datetime.now()
         # Avoid mutating input documents
         dup_docs = [deepcopy(d) for d in documents]
```

### Comparing `gigachain-0.1.9/langchain/runnables/hub.py` & `gigachain-0.2.0/langchain/runnables/hub.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/runnables/openai_functions.py` & `gigachain-0.2.0/langchain/runnables/openai_functions.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/schema/__init__.py` & `gigachain-0.2.0/langchain/schema/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """**Schemas** are the LangChain Base Classes and Interfaces."""
+
 from langchain_core.agents import AgentAction, AgentFinish
 from langchain_core.caches import BaseCache
 from langchain_core.chat_history import BaseChatMessageHistory
 from langchain_core.documents import BaseDocumentTransformer, Document
 from langchain_core.exceptions import LangChainException, OutputParserException
 from langchain_core.memory import BaseMemory
 from langchain_core.messages import (
```

### Comparing `gigachain-0.1.9/langchain/schema/callbacks/manager.py` & `gigachain-0.2.0/langchain/callbacks/manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Any
+
 from langchain_core.callbacks.manager import (
     AsyncCallbackManager,
     AsyncCallbackManagerForChainGroup,
     AsyncCallbackManagerForChainRun,
     AsyncCallbackManagerForLLMRun,
     AsyncCallbackManagerForRetrieverRun,
     AsyncCallbackManagerForToolRun,
@@ -10,46 +14,76 @@
     BaseRunManager,
     CallbackManager,
     CallbackManagerForChainGroup,
     CallbackManagerForChainRun,
     CallbackManagerForLLMRun,
     CallbackManagerForRetrieverRun,
     CallbackManagerForToolRun,
+    Callbacks,
     ParentRunManager,
     RunManager,
+    ahandle_event,
+    atrace_as_chain_group,
     handle_event,
     trace_as_chain_group,
 )
 from langchain_core.tracers.context import (
     collect_runs,
-    register_configure_hook,
     tracing_enabled,
     tracing_v2_enabled,
 )
 from langchain_core.utils.env import env_var_is_set
 
+from langchain._api import create_importer
+
+if TYPE_CHECKING:
+    from langchain_community.callbacks.manager import (
+        get_openai_callback,
+        wandb_tracing_enabled,
+    )
+
+# Create a way to dynamically look up deprecated imports.
+# Used to consolidate logic for raising deprecation warnings and
+# handling optional imports.
+DEPRECATED_LOOKUP = {
+    "get_openai_callback": "langchain_community.callbacks.manager",
+    "wandb_tracing_enabled": "langchain_community.callbacks.manager",
+}
+
+_import_attribute = create_importer(__file__, deprecated_lookups=DEPRECATED_LOOKUP)
+
+
+def __getattr__(name: str) -> Any:
+    """Look up attributes dynamically."""
+    return _import_attribute(name)
+
+
 __all__ = [
-    "tracing_enabled",
-    "tracing_v2_enabled",
-    "collect_runs",
-    "trace_as_chain_group",
-    "handle_event",
-    "BaseRunManager",
-    "RunManager",
-    "ParentRunManager",
-    "AsyncRunManager",
-    "AsyncParentRunManager",
-    "CallbackManagerForLLMRun",
-    "AsyncCallbackManagerForLLMRun",
-    "CallbackManagerForChainRun",
+    "ahandle_event",
+    "AsyncCallbackManagerForChainGroup",
     "AsyncCallbackManagerForChainRun",
-    "CallbackManagerForToolRun",
-    "AsyncCallbackManagerForToolRun",
-    "CallbackManagerForRetrieverRun",
+    "AsyncCallbackManagerForLLMRun",
     "AsyncCallbackManagerForRetrieverRun",
+    "AsyncCallbackManagerForToolRun",
+    "AsyncParentRunManager",
+    "AsyncRunManager",
+    "atrace_as_chain_group",
+    "BaseRunManager",
     "CallbackManager",
     "CallbackManagerForChainGroup",
+    "CallbackManagerForChainRun",
+    "CallbackManagerForLLMRun",
+    "CallbackManagerForRetrieverRun",
+    "CallbackManagerForToolRun",
+    "Callbacks",
     "AsyncCallbackManager",
-    "AsyncCallbackManagerForChainGroup",
-    "register_configure_hook",
+    "collect_runs",
     "env_var_is_set",
+    "get_openai_callback",
+    "handle_event",
+    "ParentRunManager",
+    "RunManager",
+    "trace_as_chain_group",
+    "tracing_enabled",
+    "tracing_v2_enabled",
+    "wandb_tracing_enabled",
 ]
```

### Comparing `gigachain-0.1.9/langchain/schema/messages.py` & `gigachain-0.2.0/langchain/schema/messages.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/schema/output_parser.py` & `gigachain-0.2.0/langchain/schema/output_parser.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/schema/runnable/__init__.py` & `gigachain-0.2.0/langchain/schema/runnable/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 for higher concurrent loads.
 
 **Streaming** of intermediate outputs as they're being generated allows for
 creating more responsive UX.
 
 This module contains schema and implementation of LangChain Runnables primitives.
 """
+
 from langchain_core.runnables.base import (
     Runnable,
     RunnableBinding,
     RunnableGenerator,
     RunnableLambda,
     RunnableMap,
     RunnableParallel,
```

### Comparing `gigachain-0.1.9/langchain/schema/runnable/base.py` & `gigachain-0.2.0/langchain/schema/runnable/base.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/schema/runnable/config.py` & `gigachain-0.2.0/langchain/schema/runnable/config.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/schema/runnable/utils.py` & `gigachain-0.2.0/langchain/schema/runnable/utils.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/smith/__init__.py` & `gigachain-0.2.0/langchain/smith/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,48 +50,49 @@
 
 .. code-block:: python
 
     from typing import Optional
     from langchain.evaluation import StringEvaluator
 
     class MyStringEvaluator(StringEvaluator):
-        
+
         @property
         def requires_input(self) -> bool:
             return False
-        
+
         @property
         def requires_reference(self) -> bool:
             return True
-        
+
         @property
         def evaluation_name(self) -> str:
             return "exact_match"
-        
+
         def _evaluate_strings(self, prediction, reference=None, input=None, **kwargs) -> dict:
             return {"score": prediction == reference}
 
 
     evaluation_config = RunEvalConfig(
         custom_evaluators = [MyStringEvaluator()],
     )
 
     run_on_dataset(
         client,
         "<my_dataset_name>",
         construct_chain,
         evaluation=evaluation_config,
-    )    
+    )
 
 **Primary Functions**
 
 - :func:`arun_on_dataset <langchain.smith.evaluation.runner_utils.arun_on_dataset>`: Asynchronous function to evaluate a chain, agent, or other LangChain component over a dataset.
 - :func:`run_on_dataset <langchain.smith.evaluation.runner_utils.run_on_dataset>`: Function to evaluate a chain, agent, or other LangChain component over a dataset.
 - :class:`RunEvalConfig <langchain.smith.evaluation.config.RunEvalConfig>`: Class representing the configuration for running evaluation. You can select evaluators by :class:`EvaluatorType <langchain.evaluation.schema.EvaluatorType>` or config, or you can pass in `custom_evaluators`
 """  # noqa: E501
+
 from langchain.smith.evaluation import (
     RunEvalConfig,
     arun_on_dataset,
     run_on_dataset,
 )
 
 __all__ = [
```

### Comparing `gigachain-0.1.9/langchain/smith/evaluation/__init__.py` & `gigachain-0.2.0/langchain/smith/evaluation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 - ``run_on_dataset``: Function to evaluate a chain or other LangChain component over a dataset.
 - ``RunEvalConfig``: Class representing the configuration for running evaluation.
 - ``StringRunEvaluatorChain``: Class representing a string run evaluator chain.
 - ``InputFormatError``: Exception raised when the input format is incorrect.
 
 """  # noqa: E501
 
-
 from langchain.smith.evaluation.config import RunEvalConfig
 from langchain.smith.evaluation.runner_utils import (
     InputFormatError,
     arun_on_dataset,
     run_on_dataset,
 )
 from langchain.smith.evaluation.string_run_evaluator import StringRunEvaluatorChain
```

### Comparing `gigachain-0.1.9/langchain/smith/evaluation/config.py` & `gigachain-0.2.0/langchain/smith/evaluation/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 """Configuration for run evaluators."""
 
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Sequence, Union
 
 from langchain_core.embeddings import Embeddings
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.prompts import BasePromptTemplate
 from langchain_core.pydantic_v1 import BaseModel, Field
 from langsmith import RunEvaluator
+from langsmith.evaluation.evaluator import EvaluationResult, EvaluationResults
+from langsmith.schemas import Example, Run
 
 from langchain.evaluation.criteria.eval_chain import CRITERIA_TYPE
 from langchain.evaluation.embedding_distance.base import (
     EmbeddingDistance as EmbeddingDistanceEnum,
 )
 from langchain.evaluation.schema import EvaluatorType, StringEvaluator
 from langchain.evaluation.string_distance.base import (
     StringDistance as StringDistanceEnum,
 )
 
+RUN_EVALUATOR_LIKE = Callable[
+    [Run, Optional[Example]], Union[EvaluationResult, EvaluationResults, dict]
+]
+BATCH_EVALUATOR_LIKE = Callable[
+    [Sequence[Run], Optional[Sequence[Example]]],
+    Union[EvaluationResult, EvaluationResults, dict],
+]
+
 
 class EvalConfig(BaseModel):
     """Configuration for a given run evaluator.
 
     Parameters
     ----------
     evaluator_type : EvaluatorType
@@ -72,20 +82,24 @@
         kwargs = super().get_kwargs()
         # Filer out the keys that are not needed for the evaluator.
         for key in ["reference_key", "prediction_key", "input_key"]:
             kwargs.pop(key, None)
         return kwargs
 
 
+CUSTOM_EVALUATOR_TYPE = Union[RUN_EVALUATOR_LIKE, RunEvaluator, StringEvaluator]
+SINGLE_EVAL_CONFIG_TYPE = Union[EvaluatorType, str, EvalConfig]
+
+
 class RunEvalConfig(BaseModel):
     """Configuration for a run evaluation.
 
     Parameters
     ----------
-    evaluators : List[Union[EvaluatorType, EvalConfig]]
+    evaluators : List[Union[EvaluatorType, EvalConfig, RunEvaluator, Callable]]
         Configurations for which evaluators to apply to the dataset run.
         Each can be the string of an :class:`EvaluatorType <langchain.evaluation.schema.EvaluatorType>`, such
         as EvaluatorType.QA, the evaluator type string ("qa"), or a configuration for a
         given evaluator (e.g., :class:`RunEvalConfig.QA <langchain.smith.evaluation.config.RunEvalConfig.QA>`).
 
     custom_evaluators : Optional[List[Union[RunEvaluator, StringEvaluator]]]
         Custom evaluators to apply to the dataset run.
@@ -103,26 +117,36 @@
         The key from the traced run's inputs dictionary to use to represent the
         input. If not provided, it will be inferred automatically.
 
     eval_llm : Optional[BaseLanguageModel]
         The language model to pass to any evaluators that use a language model.
     """  # noqa: E501
 
-    evaluators: List[Union[EvaluatorType, str, EvalConfig]] = Field(
-        default_factory=list
-    )
+    evaluators: List[
+        Union[
+            SINGLE_EVAL_CONFIG_TYPE,
+            CUSTOM_EVALUATOR_TYPE,
+        ]
+    ] = Field(default_factory=list)
     """Configurations for which evaluators to apply to the dataset run.
     Each can be the string of an
     :class:`EvaluatorType <langchain.evaluation.schema.EvaluatorType>`, such
     as `EvaluatorType.QA`, the evaluator type string ("qa"), or a configuration for a
     given evaluator
     (e.g., 
     :class:`RunEvalConfig.QA <langchain.smith.evaluation.config.RunEvalConfig.QA>`)."""  # noqa: E501
-    custom_evaluators: Optional[List[Union[RunEvaluator, StringEvaluator]]] = None
+    custom_evaluators: Optional[List[CUSTOM_EVALUATOR_TYPE]] = None
     """Custom evaluators to apply to the dataset run."""
+    batch_evaluators: Optional[List[BATCH_EVALUATOR_LIKE]] = None
+    """Evaluators that run on an aggregate/batch level.
+
+    These generate 1 or more metrics that are assigned to the full test run.
+    As a result, they are not associated with individual traces.
+    """
+
     reference_key: Optional[str] = None
     """The key in the dataset run to use as the reference string.
     If not provided, we will attempt to infer automatically."""
     prediction_key: Optional[str] = None
     """The key from the traced run's outputs dictionary to use to
     represent the prediction. If not provided, it will be inferred
     automatically."""
@@ -150,15 +174,15 @@
         criteria: Optional[CRITERIA_TYPE] = None
         llm: Optional[BaseLanguageModel] = None
         evaluator_type: EvaluatorType = EvaluatorType.CRITERIA
 
         def __init__(
             self, criteria: Optional[CRITERIA_TYPE] = None, **kwargs: Any
         ) -> None:
-            super().__init__(criteria=criteria, **kwargs)
+            super().__init__(criteria=criteria, **kwargs)  # type: ignore[call-arg]
 
     class LabeledCriteria(SingleKeyEvalConfig):
         """Configuration for a labeled (with references) criteria evaluator.
 
         Parameters
         ----------
         criteria : Optional[CRITERIA_TYPE]
@@ -170,15 +194,15 @@
         criteria: Optional[CRITERIA_TYPE] = None
         llm: Optional[BaseLanguageModel] = None
         evaluator_type: EvaluatorType = EvaluatorType.LABELED_CRITERIA
 
         def __init__(
             self, criteria: Optional[CRITERIA_TYPE] = None, **kwargs: Any
         ) -> None:
-            super().__init__(criteria=criteria, **kwargs)
+            super().__init__(criteria=criteria, **kwargs)  # type: ignore[call-arg]
 
     class EmbeddingDistance(SingleKeyEvalConfig):
         """Configuration for an embedding distance evaluator.
 
         Parameters
         ----------
         embeddings : Optional[Embeddings]
@@ -292,15 +316,15 @@
             Whether to ignore case when comparing strings.
         ignore_punctuation : bool
             Whether to ignore punctuation when comparing strings.
         ignore_numbers : bool
             Whether to ignore numbers when comparing strings.
         """
 
-        evaluator_type: EvaluatorType = EvaluatorType.STRING_DISTANCE
+        evaluator_type: EvaluatorType = EvaluatorType.EXACT_MATCH
         ignore_case: bool = False
         ignore_punctuation: bool = False
         ignore_numbers: bool = False
 
     class RegexMatch(SingleKeyEvalConfig):
         """Configuration for a regex match string evaluator.
 
@@ -342,11 +366,11 @@
 
         def __init__(
             self,
             criteria: Optional[CRITERIA_TYPE] = None,
             normalize_by: Optional[float] = None,
             **kwargs: Any,
         ) -> None:
-            super().__init__(criteria=criteria, normalize_by=normalize_by, **kwargs)
+            super().__init__(criteria=criteria, normalize_by=normalize_by, **kwargs)  # type: ignore[call-arg]
 
     class LabeledScoreString(ScoreString):
         evaluator_type: EvaluatorType = EvaluatorType.LABELED_SCORE_STRING
```

### Comparing `gigachain-0.1.9/langchain/smith/evaluation/name_generation.py` & `gigachain-0.2.0/langchain/smith/evaluation/name_generation.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/smith/evaluation/progress.py` & `gigachain-0.2.0/langchain/smith/evaluation/progress.py`

 * *Files identical despite different names*

### Comparing `gigachain-0.1.9/langchain/smith/evaluation/runner_utils.py` & `gigachain-0.2.0/langchain/smith/evaluation/runner_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 """Utilities for running language models or Chains over datasets."""
 
 from __future__ import annotations
 
+import concurrent.futures
 import dataclasses
 import functools
 import inspect
 import logging
 import uuid
 from datetime import datetime, timezone
-from enum import Enum
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     List,
     Optional,
     Tuple,
     Union,
     cast,
 )
 
 from langchain_core._api import warn_deprecated
+from langchain_core.callbacks.manager import Callbacks
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.messages import BaseMessage, messages_from_dict
 from langchain_core.outputs import ChatResult, LLMResult
 from langchain_core.runnables import Runnable, RunnableConfig, RunnableLambda
 from langchain_core.runnables import config as runnable_config
 from langchain_core.runnables import utils as runnable_utils
 from langchain_core.tracers.evaluation import (
     EvaluatorCallbackHandler,
     wait_for_all_evaluators,
 )
 from langchain_core.tracers.langchain import LangChainTracer
 from langsmith.client import Client
 from langsmith.env import get_git_info, get_langchain_env_var_metadata
-from langsmith.evaluation import EvaluationResult, RunEvaluator
+from langsmith.evaluation import (
+    EvaluationResult,
+    RunEvaluator,
+)
+from langsmith.evaluation import (
+    run_evaluator as run_evaluator_dec,
+)
 from langsmith.run_helpers import as_runnable, is_traceable_function
-from langsmith.schemas import Dataset, DataType, Example, TracerSession
+from langsmith.schemas import Dataset, DataType, Example, Run, TracerSession
 from langsmith.utils import LangSmithError
 from requests import HTTPError
 from typing_extensions import TypedDict
 
-from langchain.callbacks.manager import Callbacks
 from langchain.chains.base import Chain
 from langchain.evaluation.loading import load_evaluator
 from langchain.evaluation.schema import (
     EvaluatorType,
     PairwiseStringEvaluator,
     StringEvaluator,
 )
@@ -270,56 +276,60 @@
         return prompts[0]
     else:
         raise InputFormatError(
             f"LLM Run expects single prompt input. Got {len(prompts)} prompts."
         )
 
 
-def _get_messages(inputs: Dict[str, Any]) -> List[BaseMessage]:
+class ChatModelInput(TypedDict):
+    """Input for a chat model.
+
+    Parameters:
+        messages: List of chat messages.
+    """
+
+    messages: List[BaseMessage]
+
+
+def _get_messages(inputs: Dict[str, Any]) -> dict:
     """Get Chat Messages from inputs.
 
     Args:
         inputs: The input dictionary.
 
     Returns:
         A list of chat messages.
     Raises:
         InputFormatError: If the input format is invalid.
     """
     if not inputs:
         raise InputFormatError("Inputs should not be empty.")
-
+    input_copy = inputs.copy()
     if "messages" in inputs:
-        single_input = inputs["messages"]
+        input_copy["input"] = input_copy.pop("messages")
     elif len(inputs) == 1:
-        single_input = next(iter(inputs.values()))
-    else:
-        raise InputFormatError(
-            f"Chat Run expects 'messages' in inputs when example has multiple"
-            f" input keys. Got {inputs}"
-        )
-    if isinstance(single_input, list) and all(
-        isinstance(i, dict) for i in single_input
-    ):
-        raw_messages = [single_input]
-    elif isinstance(single_input, list) and all(
-        isinstance(i, list) for i in single_input
-    ):
-        raw_messages = single_input
-    else:
-        raise InputFormatError(
-            f"Chat Run expects List[dict] or List[List[dict]] values for"
-            f" 'messages' key input. Got {inputs}"
-        )
-    if len(raw_messages) == 1:
-        return messages_from_dict(raw_messages[0])
+        input_copy["input"] = next(iter(inputs.values()))
+    if "input" in input_copy:
+        raw_messages = input_copy["input"]
+        if isinstance(raw_messages, list) and all(
+            isinstance(i, dict) for i in raw_messages
+        ):
+            raw_messages = [raw_messages]
+        if len(raw_messages) == 1:
+            input_copy["input"] = messages_from_dict(raw_messages[0])
+        else:
+            raise InputFormatError(
+                "Batch messages not supported. Please provide a"
+                " single list of messages."
+            )
+        return input_copy
     else:
         raise InputFormatError(
             f"Chat Run expects single List[dict] or List[List[dict]] 'messages'"
-            f" input. Got {len(raw_messages)} messages from inputs {inputs}"
+            f" input. Got {inputs}"
         )
 
 
 ## Shared data validation utilities
 def _validate_example_inputs_for_language_model(
     first_example: Example,
     input_mapper: Optional[Callable[[Dict], Any]],
@@ -419,21 +429,14 @@
     """Configure the evaluators to run on the results of the chain."""
     if evaluation:
         if isinstance(llm_or_chain_factory, BaseLanguageModel):
             run_inputs, run_outputs = None, None
             run_type = "llm"
         else:
             run_type = "chain"
-            if data_type in (DataType.chat, DataType.llm):
-                val = data_type.value if isinstance(data_type, Enum) else data_type
-                raise ValueError(
-                    "Cannot evaluate a chain on dataset with "
-                    f"data_type={val}. "
-                    "Please specify a dataset with the default 'kv' data type."
-                )
             chain = llm_or_chain_factory()
             run_inputs = chain.input_keys if isinstance(chain, Chain) else None
             run_outputs = chain.output_keys if isinstance(chain, Chain) else None
         run_evaluators = _load_run_evaluators(
             evaluation,
             run_type,
             data_type,
@@ -509,37 +512,47 @@
         reference_key = list(example_outputs)[0]
     else:
         reference_key = None
     return reference_key
 
 
 def _construct_run_evaluator(
-    eval_config: Union[EvaluatorType, str, smith_eval_config.EvalConfig],
+    eval_config: Union[
+        smith_eval_config.SINGLE_EVAL_CONFIG_TYPE,
+        smith_eval_config.CUSTOM_EVALUATOR_TYPE,
+    ],
     eval_llm: Optional[BaseLanguageModel],
     run_type: str,
     data_type: DataType,
     example_outputs: Optional[List[str]],
     reference_key: Optional[str],
     input_key: Optional[str],
     prediction_key: Optional[str],
 ) -> RunEvaluator:
+    if isinstance(eval_config, RunEvaluator):
+        return eval_config
     if isinstance(eval_config, (EvaluatorType, str)):
         if not isinstance(eval_config, EvaluatorType):
             eval_config = EvaluatorType(eval_config)
         evaluator_ = load_evaluator(eval_config, llm=eval_llm)
         eval_type_tag = eval_config.value
-    else:
+    elif isinstance(eval_config, smith_eval_config.EvalConfig):
         kwargs = {"llm": eval_llm, **eval_config.get_kwargs()}
         evaluator_ = load_evaluator(eval_config.evaluator_type, **kwargs)
         eval_type_tag = eval_config.evaluator_type.value
         # Override keys if specified in the config
         if isinstance(eval_config, smith_eval_config.SingleKeyEvalConfig):
             input_key = eval_config.input_key or input_key
             prediction_key = eval_config.prediction_key or prediction_key
             reference_key = eval_config.reference_key or reference_key
+    elif callable(eval_config):
+        # Assume we can decorate
+        return run_evaluator_dec(eval_config)
+    else:
+        raise ValueError(f"Unknown evaluator type: {type(eval_config)}")
 
     if isinstance(evaluator_, StringEvaluator):
         if evaluator_.requires_reference and reference_key is None:
             raise ValueError(
                 f"Must specify reference_key in smith_eval.RunEvalConfig to use"
                 f" evaluator of type {eval_type_tag} with"
                 f" dataset with multiple output keys: {example_outputs}."
@@ -596,21 +609,17 @@
         config: Configuration for the run evaluators.
 
     Returns:
         A list of run evaluators.
     """
     run_evaluators = []
     input_key, prediction_key, reference_key = None, None, None
-    if (
-        config.evaluators
-        or any([isinstance(e, EvaluatorType) for e in config.evaluators])
-        or (
-            config.custom_evaluators
-            and any([isinstance(e, StringEvaluator) for e in config.custom_evaluators])
-        )
+    if config.evaluators or (
+        config.custom_evaluators
+        and any([isinstance(e, StringEvaluator) for e in config.custom_evaluators])
     ):
         input_key, prediction_key, reference_key = _get_keys(
             config, run_inputs, run_outputs, example_outputs
         )
     for eval_config in config.evaluators:
         run_evaluator = _construct_run_evaluator(
             eval_config,
@@ -634,14 +643,16 @@
                     run_type,
                     data_type,
                     input_key=input_key,
                     prediction_key=prediction_key,
                     reference_key=reference_key,
                 )
             )
+        elif callable(custom_evaluator):
+            run_evaluators.append(run_evaluator_dec(custom_evaluator))
         else:
             raise ValueError(
                 f"Unsupported custom evaluator: {custom_evaluator}."
                 f" Expected RunEvaluator or StringEvaluator."
             )
 
     return run_evaluators
@@ -700,17 +711,17 @@
             llm_output: Union[str, BaseMessage] = await llm.ainvoke(
                 prompt,
                 config=RunnableConfig(
                     callbacks=callbacks, tags=tags or [], metadata=metadata or {}
                 ),
             )
         except InputFormatError:
-            messages = _get_messages(inputs)
+            llm_inputs = _get_messages(inputs)
             llm_output = await llm.ainvoke(
-                messages,
+                **llm_inputs,
                 config=RunnableConfig(
                     callbacks=callbacks, tags=tags or [], metadata=metadata or {}
                 ),
             )
     return llm_output
 
 
@@ -853,17 +864,17 @@
             llm_output = llm.invoke(
                 llm_prompts,
                 config=RunnableConfig(
                     callbacks=callbacks, tags=tags or [], metadata=metadata or {}
                 ),
             )
         except InputFormatError:
-            llm_messages = _get_messages(inputs)
+            llm_inputs = _get_messages(inputs)
             llm_output = llm.invoke(
-                llm_messages,
+                **llm_inputs,
                 config=RunnableConfig(callbacks=callbacks, metadata=metadata or {}),
             )
     return llm_output
 
 
 def _run_chain(
     chain: Union[Chain, Runnable],
@@ -949,39 +960,45 @@
             f"with inputs {example.inputs}"
             f"\nError Type: {error_type}, Message: {e}"
         )
         result = EvalError(Error=e)
     return result
 
 
-## Public API
-
-
 def _prepare_eval_run(
     client: Client,
     dataset_name: str,
     llm_or_chain_factory: MODEL_OR_CHAIN_FACTORY,
     project_name: str,
     project_metadata: Optional[Dict[str, Any]] = None,
     tags: Optional[List[str]] = None,
+    dataset_version: Optional[Union[str, datetime]] = None,
 ) -> Tuple[MCF, TracerSession, Dataset, List[Example]]:
     wrapped_model = _wrap_in_chain_factory(llm_or_chain_factory, dataset_name)
     dataset = client.read_dataset(dataset_name=dataset_name)
-    examples = list(client.list_examples(dataset_id=dataset.id))
+
+    examples = list(client.list_examples(dataset_id=dataset.id, as_of=dataset_version))
     if not examples:
         raise ValueError(f"Dataset {dataset_name} has no example rows.")
+    modified_at = [ex.modified_at for ex in examples if ex.modified_at]
+    # Should always be defined in practice when fetched,
+    # but the typing permits None
+    max_modified_at = max(modified_at) if modified_at else None
+    inferred_version = max_modified_at.isoformat() if max_modified_at else None
 
     try:
+        project_metadata = project_metadata or {}
         git_info = get_git_info()
         if git_info:
-            project_metadata = project_metadata or {}
             project_metadata = {
                 **project_metadata,
                 "git": git_info,
             }
+
+        project_metadata["dataset_version"] = inferred_version
         project = client.create_project(
             project_name,
             reference_dataset_id=dataset.id,
             project_extra={"tags": tags} if tags else {},
             metadata=project_metadata,
         )
     except (HTTPError, ValueError, LangSmithError) as e:
@@ -1021,14 +1038,15 @@
     """A container to help manage the state of a eval run."""
 
     client: Client
     project: TracerSession
     wrapped_model: MCF
     examples: List[Example]
     configs: List[RunnableConfig]
+    batch_evaluators: Optional[List[smith_eval_config.BATCH_EVALUATOR_LIKE]] = None
 
     def _merge_test_outputs(
         self,
         batch_results: list,
         all_eval_results: Dict[str, _RowResult],
     ) -> dict:
         results: dict = {}
@@ -1044,16 +1062,42 @@
                 results[str(example.id)]["Error"] = output.Error
             else:
                 results[str(example.id)]["output"] = output
             if example.outputs:
                 results[str(example.id)]["reference"] = example.outputs
         return results
 
-    def _collect_metrics(self) -> Dict[str, _RowResult]:
+    def _run_batch_evaluators(self, runs: Dict[str, Run]) -> List[dict]:
+        evaluators = self.batch_evaluators
+        if not evaluators:
+            return []
+        runs_list = [runs[str(example.id)] for example in self.examples]
+        aggregate_feedback = []
+        with concurrent.futures.ThreadPoolExecutor() as executor:
+            for evaluator in evaluators:
+                try:
+                    result = evaluator(runs_list, self.examples)
+                    if isinstance(result, EvaluationResult):
+                        result = result.dict()
+                    aggregate_feedback.append(cast(dict, result))
+                    executor.submit(
+                        self.client.create_feedback,
+                        **result,
+                        run_id=None,
+                        project_id=self.project.id,
+                    )
+                except Exception as e:
+                    logger.error(
+                        f"Error running batch evaluator {repr(evaluator)}: {e}"
+                    )
+        return aggregate_feedback
+
+    def _collect_metrics(self) -> Tuple[Dict[str, _RowResult], Dict[str, Run]]:
         all_eval_results: dict = {}
+        all_runs: dict = {}
         for c in self.configs:
             for callback in cast(list, c["callbacks"]):
                 if isinstance(callback, EvaluatorCallbackHandler):
                     eval_results = callback.logged_eval_results
                     for (_, example_id), v in eval_results.items():
                         all_eval_results.setdefault(str(example_id), {}).update(
                             {"feedback": v}
@@ -1066,28 +1110,36 @@
                         else None
                     )
                     run_id = str(run.id) if run else None
                     all_eval_results.setdefault(str(callback.example_id), {}).update(
                         {
                             "execution_time": execution_time,
                             "run_id": run_id,
+                            "run": run,
                         }
                     )
-        return cast(Dict[str, _RowResult], all_eval_results)
+                    all_runs[str(callback.example_id)] = run
+        return cast(Dict[str, _RowResult], all_eval_results), all_runs
 
     def _collect_test_results(
         self,
         batch_results: List[Union[dict, str, LLMResult, ChatResult]],
     ) -> TestResult:
+        logger.info("Waiting for evaluators to complete.")
         wait_for_all_evaluators()
-        all_eval_results = self._collect_metrics()
+        all_eval_results, all_runs = self._collect_metrics()
+        aggregate_feedback = None
+        if self.batch_evaluators:
+            logger.info("Running session evaluators.")
+            aggregate_feedback = self._run_batch_evaluators(all_runs)
         results = self._merge_test_outputs(batch_results, all_eval_results)
         return TestResult(
             project_name=self.project.name,
             results=results,
+            aggregate_metrics=aggregate_feedback,
         )
 
     def finish(self, batch_results: list, verbose: bool = False) -> TestResult:
         results = self._collect_test_results(batch_results)
         if verbose:
             try:
                 agg_feedback = results.get_aggregate_feedback()
@@ -1112,31 +1164,36 @@
         project_name: Optional[str],
         evaluation: Optional[smith_eval.RunEvalConfig] = None,
         tags: Optional[List[str]] = None,
         input_mapper: Optional[Callable[[Dict], Any]] = None,
         concurrency_level: int = 5,
         project_metadata: Optional[Dict[str, Any]] = None,
         revision_id: Optional[str] = None,
+        dataset_version: Optional[Union[datetime, str]] = None,
     ) -> _DatasetRunContainer:
         project_name = project_name or name_generation.random_name()
         if revision_id:
             if not project_metadata:
                 project_metadata = {}
             project_metadata.update({"revision_id": revision_id})
         wrapped_model, project, dataset, examples = _prepare_eval_run(
             client,
             dataset_name,
             llm_or_chain_factory,
             project_name,
             project_metadata=project_metadata,
             tags=tags,
+            dataset_version=dataset_version,
         )
         tags = tags or []
         for k, v in (project.metadata.get("git") or {}).items():
             tags.append(f"git:{k}={v}")
+        run_metadata = {"dataset_version": project.metadata["dataset_version"]}
+        if revision_id:
+            run_metadata["revision_id"] = revision_id
         wrapped_model = _wrap_in_chain_factory(llm_or_chain_factory)
         run_evaluators = _setup_evaluation(
             wrapped_model, examples, evaluation, dataset.data_type or DataType.kv
         )
         _validate_example_inputs(examples[0], wrapped_model, input_mapper)
         progress_bar = progress.ProgressBarCallback(len(examples))
         configs = [
@@ -1153,24 +1210,25 @@
                         example_id=example.id,
                         max_concurrency=0,
                     ),
                     progress_bar,
                 ],
                 tags=tags,
                 max_concurrency=concurrency_level,
-                metadata={"revision_id": revision_id} if revision_id else {},
+                metadata=run_metadata,
             )
             for example in examples
         ]
         return cls(
             client=client,
             project=project,
             wrapped_model=wrapped_model,
             examples=examples,
             configs=configs,
+            batch_evaluators=evaluation.batch_evaluators if evaluation else None,
         )
 
 
 def _is_jupyter_environment() -> bool:
     try:
         from IPython import get_ipython
 
@@ -1204,34 +1262,44 @@
     "    input_mapper = {'other_key': 'MyOtherInput', 'my_input_key': x}\n"
     "    return input_mapper | my_chain\n"
     "run_on_dataset(..., llm_or_chain_factory=construct_chain)\n"
     "(See https://api.python.langchain.com/en/latest/schema/"
     "langchain.schema.runnable.base.RunnableLambda.html)"
 )
 
+## Public API
+
 
 async def arun_on_dataset(
     client: Optional[Client],
     dataset_name: str,
     llm_or_chain_factory: MODEL_OR_CHAIN_FACTORY,
     *,
     evaluation: Optional[smith_eval.RunEvalConfig] = None,
+    dataset_version: Optional[Union[datetime, str]] = None,
     concurrency_level: int = 5,
     project_name: Optional[str] = None,
     project_metadata: Optional[Dict[str, Any]] = None,
     verbose: bool = False,
-    tags: Optional[List[str]] = None,
     revision_id: Optional[str] = None,
     **kwargs: Any,
 ) -> Dict[str, Any]:
     input_mapper = kwargs.pop("input_mapper", None)
     if input_mapper:
         warn_deprecated("0.0.305", message=_INPUT_MAPPER_DEP_WARNING, pending=True)
     if revision_id is None:
         revision_id = get_langchain_env_var_metadata().get("revision_id")
+    tags = kwargs.pop("tags", None)
+    if tags:
+        warn_deprecated(
+            "0.1.9",
+            message="The tags argument is deprecated and will be"
+            " removed in a future release. Please specify project_metadata instead.",
+            pending=True,
+        )
 
     if kwargs:
         warn_deprecated(
             "0.0.305",
             message="The following arguments are deprecated and "
             "will be removed in a future release: "
             f"{kwargs.keys()}.",
@@ -1245,14 +1313,15 @@
         project_name,
         evaluation,
         tags,
         input_mapper,
         concurrency_level,
         project_metadata=project_metadata,
         revision_id=revision_id,
+        dataset_version=dataset_version,
     )
     batch_results = await runnable_utils.gather_with_concurrency(
         container.configs[0].get("max_concurrency"),
         *map(
             functools.partial(
                 _arun_llm_or_chain,
                 llm_or_chain_factory=container.wrapped_model,
@@ -1267,25 +1336,33 @@
 
 def run_on_dataset(
     client: Optional[Client],
     dataset_name: str,
     llm_or_chain_factory: MODEL_OR_CHAIN_FACTORY,
     *,
     evaluation: Optional[smith_eval.RunEvalConfig] = None,
+    dataset_version: Optional[Union[datetime, str]] = None,
     concurrency_level: int = 5,
     project_name: Optional[str] = None,
     project_metadata: Optional[Dict[str, Any]] = None,
     verbose: bool = False,
-    tags: Optional[List[str]] = None,
     revision_id: Optional[str] = None,
     **kwargs: Any,
 ) -> Dict[str, Any]:
     input_mapper = kwargs.pop("input_mapper", None)
     if input_mapper:
         warn_deprecated("0.0.305", message=_INPUT_MAPPER_DEP_WARNING, pending=True)
+    tags = kwargs.pop("tags", None)
+    if tags:
+        warn_deprecated(
+            "0.1.9",
+            message="The tags argument is deprecated and will be"
+            " removed in a future release. Please specify project_metadata instead.",
+            pending=True,
+        )
     if revision_id is None:
         revision_id = get_langchain_env_var_metadata().get("revision_id")
 
     if kwargs:
         warn_deprecated(
             "0.0.305",
             message="The following arguments are deprecated and "
@@ -1301,14 +1378,15 @@
         project_name,
         evaluation,
         tags,
         input_mapper,
         concurrency_level,
         project_metadata=project_metadata,
         revision_id=revision_id,
+        dataset_version=dataset_version,
     )
     if concurrency_level == 0:
         batch_results = [
             _run_llm_or_chain(
                 example,
                 config,
                 llm_or_chain_factory=container.wrapped_model,
@@ -1393,16 +1471,16 @@
             }),
         ]
     )
 
     client = Client()
     run_on_dataset(
         client,
-        "<my_dataset_name>",
-        construct_chain,
+        dataset_name="<my_dataset_name>",
+        llm_or_chain_factory=construct_chain,
         evaluation=evaluation_config,
     )
 
 You can also create custom evaluators by subclassing the
 :class:`StringEvaluator <langchain.evaluation.schema.StringEvaluator>`
 or LangSmith's `RunEvaluator` classes.
 
@@ -1431,16 +1509,16 @@
 
     evaluation_config = smith_eval.RunEvalConfig(
         custom_evaluators = [MyStringEvaluator()],
     )
 
     run_on_dataset(
         client,
-        "<my_dataset_name>",
-        construct_chain,
+        dataset_name="<my_dataset_name>",
+        llm_or_chain_factory=construct_chain,
         evaluation=evaluation_config,
     )
 """  # noqa: E501
 run_on_dataset.__doc__ = _RUN_ON_DATASET_DOCSTRING
 arun_on_dataset.__doc__ = _RUN_ON_DATASET_DOCSTRING.replace(
     "run_on_dataset(", "await arun_on_dataset("
 )
```

### Comparing `gigachain-0.1.9/langchain/smith/evaluation/string_run_evaluator.py` & `gigachain-0.2.0/langchain/smith/evaluation/string_run_evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Run evaluator wrapper for string evaluators."""
+
 from __future__ import annotations
 
 from abc import abstractmethod
 from typing import Any, Dict, List, Optional
 
+from langchain_core.callbacks.manager import (
+    AsyncCallbackManagerForChainRun,
+    CallbackManagerForChainRun,
+)
 from langchain_core.load.dump import dumpd
 from langchain_core.load.load import load
 from langchain_core.load.serializable import Serializable
 from langchain_core.messages import BaseMessage, get_buffer_string, messages_from_dict
 from langsmith import EvaluationResult, RunEvaluator
 from langsmith.schemas import DataType, Example, Run
 
-from langchain.callbacks.manager import (
-    AsyncCallbackManagerForChainRun,
-    CallbackManagerForChainRun,
-)
 from langchain.chains.base import Chain
 from langchain.evaluation.schema import StringEvaluator
 from langchain.schema import RUN_KEY
 
 
 def _get_messages_from_run_dict(messages: List[dict]) -> List[BaseMessage]:
     if not messages:
```

### Comparing `gigachain-0.1.9/langchain/storage/__init__.py` & `gigachain-0.2.0/langchain/storage/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,56 @@
 """Implementations of key-value stores and storage helpers.
 
 Module provides implementations of various key-value stores that conform
 to a simple key-value interface.
 
 The primary goal of these storages is to support implementation of caching.
 """
-import warnings
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
-from langchain_core._api import LangChainDeprecationWarning
+from langchain_core.stores import (
+    InMemoryByteStore,
+    InMemoryStore,
+    InvalidKeyException,
+)
 
+from langchain._api import create_importer
 from langchain.storage._lc_store import create_kv_docstore, create_lc_store
 from langchain.storage.encoder_backed import EncoderBackedStore
 from langchain.storage.file_system import LocalFileStore
-from langchain.storage.in_memory import InMemoryByteStore, InMemoryStore
-from langchain.utils.interactive_env import is_interactive_env
 
+if TYPE_CHECKING:
+    from langchain_community.storage import (
+        RedisStore,
+        UpstashRedisByteStore,
+        UpstashRedisStore,
+    )
+
+# Create a way to dynamically look up deprecated imports.
+# Used to consolidate logic for raising deprecation warnings and
+# handling optional imports.
+DEPRECATED_LOOKUP = {
+    "RedisStore": "langchain_community.storage",
+    "UpstashRedisByteStore": "langchain_community.storage",
+    "UpstashRedisStore": "langchain_community.storage",
+}
 
-def __getattr__(name: str) -> Any:
-    from langchain_community import storage
+_import_attribute = create_importer(__package__, deprecated_lookups=DEPRECATED_LOOKUP)
 
-    # If not in interactive env, raise warning.
-    if not is_interactive_env():
-        warnings.warn(
-            "Importing stores from langchain is deprecated. Importing from "
-            "langchain will no longer be supported as of langchain==0.2.0. "
-            "Please import from langchain-community instead:\n\n"
-            f"`from langchain_community.storage import {name}`.\n\n"
-            "To install gigachain-community run `pip install -U gigachain-community`.",
-            category=LangChainDeprecationWarning,
-        )
 
-    return getattr(storage, name)
+def __getattr__(name: str) -> Any:
+    """Look up attributes dynamically."""
+    return _import_attribute(name)
 
 
 __all__ = [
+    "create_kv_docstore",
+    "create_lc_store",
     "EncoderBackedStore",
-    "InMemoryStore",
     "InMemoryByteStore",
+    "InMemoryStore",
+    "InvalidKeyException",
     "LocalFileStore",
     "RedisStore",
-    "create_lc_store",
-    "create_kv_docstore",
     "UpstashRedisByteStore",
     "UpstashRedisStore",
 ]
```

### Comparing `gigachain-0.1.9/langchain/storage/_lc_store.py` & `gigachain-0.2.0/langchain/storage/_lc_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Create a key-value store for any langchain serializable object."""
+
 from typing import Callable, Optional
 
 from langchain_core.documents import Document
 from langchain_core.load import Serializable, dumps, loads
 from langchain_core.stores import BaseStore, ByteStore
 
 from langchain.storage.encoder_backed import EncoderBackedStore
```

### Comparing `gigachain-0.1.9/langchain/storage/encoder_backed.py` & `gigachain-0.2.0/langchain/storage/encoder_backed.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import (
     Any,
+    AsyncIterator,
     Callable,
     Iterator,
     List,
     Optional,
     Sequence,
     Tuple,
     TypeVar,
@@ -69,27 +70,58 @@
         encoded_keys: List[str] = [self.key_encoder(key) for key in keys]
         values = self.store.mget(encoded_keys)
         return [
             self.value_deserializer(value) if value is not None else value
             for value in values
         ]
 
+    async def amget(self, keys: Sequence[K]) -> List[Optional[V]]:
+        """Get the values associated with the given keys."""
+        encoded_keys: List[str] = [self.key_encoder(key) for key in keys]
+        values = await self.store.amget(encoded_keys)
+        return [
+            self.value_deserializer(value) if value is not None else value
+            for value in values
+        ]
+
     def mset(self, key_value_pairs: Sequence[Tuple[K, V]]) -> None:
         """Set the values for the given keys."""
         encoded_pairs = [
             (self.key_encoder(key), self.value_serializer(value))
             for key, value in key_value_pairs
         ]
         self.store.mset(encoded_pairs)
 
+    async def amset(self, key_value_pairs: Sequence[Tuple[K, V]]) -> None:
+        """Set the values for the given keys."""
+        encoded_pairs = [
+            (self.key_encoder(key), self.value_serializer(value))
+            for key, value in key_value_pairs
+        ]
+        await self.store.amset(encoded_pairs)
+
     def mdelete(self, keys: Sequence[K]) -> None:
         """Delete the given keys and their associated values."""
         encoded_keys = [self.key_encoder(key) for key in keys]
         self.store.mdelete(encoded_keys)
 
+    async def amdelete(self, keys: Sequence[K]) -> None:
+        """Delete the given keys and their associated values."""
+        encoded_keys = [self.key_encoder(key) for key in keys]
+        await self.store.amdelete(encoded_keys)
+
     def yield_keys(
         self, *, prefix: Optional[str] = None
     ) -> Union[Iterator[K], Iterator[str]]:
         """Get an iterator over keys that match the given prefix."""
         # For the time being this does not return K, but str
         # it's for debugging purposes. Should fix this.
         yield from self.store.yield_keys(prefix=prefix)
+
+    async def ayield_keys(
+        self, *, prefix: Optional[str] = None
+    ) -> Union[AsyncIterator[K], AsyncIterator[str]]:
+        """Get an iterator over keys that match the given prefix."""
+        # For the time being this does not return K, but str
+        # it's for debugging purposes. Should fix this.
+        async for key in self.store.ayield_keys(prefix=prefix):
+            yield key
```

### Comparing `gigachain-0.1.9/langchain/storage/file_system.py` & `gigachain-0.2.0/langchain/storage/file_system.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import re
+import time
 from pathlib import Path
 from typing import Iterator, List, Optional, Sequence, Tuple, Union
 
 from langchain_core.stores import ByteStore
 
 from langchain.storage.exceptions import InvalidKeyException
 
@@ -32,22 +33,40 @@
 
             # Iterate over keys
             for key in file_store.yield_keys():
                 print(key)  # noqa: T201
 
     """
 
-    def __init__(self, root_path: Union[str, Path]) -> None:
+    def __init__(
+        self,
+        root_path: Union[str, Path],
+        *,
+        chmod_file: Optional[int] = None,
+        chmod_dir: Optional[int] = None,
+        update_atime: bool = False,
+    ) -> None:
         """Implement the BaseStore interface for the local file system.
 
         Args:
             root_path (Union[str, Path]): The root path of the file store. All keys are
                 interpreted as paths relative to this root.
+            chmod_file: (optional, defaults to `None`) If specified, sets permissions
+                for newly created files, overriding the current `umask` if needed.
+            chmod_dir: (optional, defaults to `None`) If specified, sets permissions
+                for newly created dirs, overriding the current `umask` if needed.
+            update_atime: (optional, defaults to `False`) If `True`, updates the
+                filesystem access time (but not the modified time) when a file is read.
+                This allows MRU/LRU cache policies to be implemented for filesystems
+                where access time updates are disabled.
         """
         self.root_path = Path(root_path).absolute()
+        self.chmod_file = chmod_file
+        self.chmod_dir = chmod_dir
+        self.update_atime = update_atime
 
     def _get_full_path(self, key: str) -> Path:
         """Get the full path for a given key relative to the root path.
 
         Args:
             key (str): The key relative to the root path.
 
@@ -62,14 +81,32 @@
             raise InvalidKeyException(
                 f"Invalid key: {key}. Key should be relative to the full path."
                 f"{self.root_path} vs. {common_path} and full path of {full_path}"
             )
 
         return Path(full_path)
 
+    def _mkdir_for_store(self, dir: Path) -> None:
+        """Makes a store directory path (including parents) with specified permissions
+
+        This is needed because `Path.mkdir()` is restricted by the current `umask`,
+        whereas the explicit `os.chmod()` used here is not.
+
+        Args:
+            dir: (Path) The store directory to make
+
+        Returns:
+            None
+        """
+        if not dir.exists():
+            self._mkdir_for_store(dir.parent)
+            dir.mkdir(exist_ok=True)
+            if self.chmod_dir is not None:
+                os.chmod(dir, self.chmod_dir)
+
     def mget(self, keys: Sequence[str]) -> List[Optional[bytes]]:
         """Get the values associated with the given keys.
 
         Args:
             keys: A sequence of keys.
 
         Returns:
@@ -78,14 +115,17 @@
         """
         values: List[Optional[bytes]] = []
         for key in keys:
             full_path = self._get_full_path(key)
             if full_path.exists():
                 value = full_path.read_bytes()
                 values.append(value)
+                if self.update_atime:
+                    # update access time only; preserve modified time
+                    os.utime(full_path, (time.time(), os.stat(full_path).st_mtime))
             else:
                 values.append(None)
         return values
 
     def mset(self, key_value_pairs: Sequence[Tuple[str, bytes]]) -> None:
         """Set the values for the given keys.
 
@@ -93,16 +133,18 @@
             key_value_pairs: A sequence of key-value pairs.
 
         Returns:
             None
         """
         for key, value in key_value_pairs:
             full_path = self._get_full_path(key)
-            full_path.parent.mkdir(parents=True, exist_ok=True)
+            self._mkdir_for_store(full_path.parent)
             full_path.write_bytes(value)
+            if self.chmod_file is not None:
+                os.chmod(full_path, self.chmod_file)
 
     def mdelete(self, keys: Sequence[str]) -> None:
         """Delete the given keys and their associated values.
 
         Args:
             keys (Sequence[str]): A sequence of keys to delete.
```

### Comparing `gigachain-0.1.9/langchain/tools/__init__.py` & `gigachain-0.2.0/langchain/tools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 
 **Main helpers:**
 
 .. code-block::
 
     CallbackManagerForToolRun, AsyncCallbackManagerForToolRun
 """
+
 import warnings
 from typing import Any
 
 from langchain_core._api import LangChainDeprecationWarning
 from langchain_core.tools import BaseTool, StructuredTool, Tool, tool
 
-from langchain.utils.interactive_env import is_interactive_env
+from langchain._api.interactive_env import is_interactive_env
 
 # Used for internal purposes
 _DEPRECATED_TOOLS = {"PythonAstREPLTool", "PythonREPLTool"}
 
 
 def _import_python_tool_PythonAstREPLTool() -> Any:
     raise ImportError(
@@ -61,15 +62,15 @@
         # If not in interactive env, raise warning.
         if not is_interactive_env():
             warnings.warn(
                 "Importing tools from langchain is deprecated. Importing from "
                 "langchain will no longer be supported as of langchain==0.2.0. "
                 "Please import from langchain-community instead:\n\n"
                 f"`from langchain_community.tools import {name}`.\n\n"
-                "To install langchain-community run "
+                "To install gigachain-community run "
                 "`pip install -U langchain-community`.",
                 category=LangChainDeprecationWarning,
             )
 
         return getattr(tools, name)
```

### Comparing `gigachain-0.1.9/langchain/tools/python/__init__.py` & `gigachain-0.2.0/langchain/tools/python/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any
 
 
 def __getattr__(name: str = "") -> Any:
-    raise ImportError(
+    raise AttributeError(
         "This tool has been moved to langchain experiment. "
         "This tool has access to a python REPL. "
         "For best practices make sure to sandbox this tool. "
         "Read https://github.com/langchain-ai/langchain/blob/master/SECURITY.md "
         "To keep using this code as is, install langchain experimental and "
         "update relevant imports replacing 'langchain' with 'langchain_experimental'"
     )
```

### Comparing `gigachain-0.1.9/langchain/utils/__init__.py` & `gigachain-0.2.0/langchain/utils/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 """
 **Utility functions** for LangChain.
 
 These functions do not depend on any other LangChain module.
 """
 
+from typing import TYPE_CHECKING, Any
+
+from langchain_core.utils import (
+    comma_list,
+    get_from_dict_or_env,
+    get_from_env,
+    stringify_dict,
+    stringify_value,
+)
 from langchain_core.utils.formatting import StrictFormatter, formatter
 from langchain_core.utils.input import (
     get_bolded_text,
     get_color_mapping,
     get_colored_text,
     print_text,
 )
@@ -17,31 +26,50 @@
     get_pydantic_field_names,
     guard_import,
     mock_now,
     raise_for_status_with_text,
     xor_args,
 )
 
-from langchain.utils.env import get_from_dict_or_env, get_from_env
-from langchain.utils.math import cosine_similarity, cosine_similarity_top_k
-from langchain.utils.strings import comma_list, stringify_dict, stringify_value
+from langchain._api import create_importer
+
+if TYPE_CHECKING:
+    from langchain_community.utils.math import (
+        cosine_similarity,
+        cosine_similarity_top_k,
+    )
+
+# Not deprecated right now because we will likely need to move these functions
+# back into langchain (as long as we're OK with the dependency on numpy).
+_MODULE_LOOKUP = {
+    "cosine_similarity": "langchain_community.utils.math",
+    "cosine_similarity_top_k": "langchain_community.utils.math",
+}
+
+_import_attribute = create_importer(__package__, module_lookup=_MODULE_LOOKUP)
+
+
+def __getattr__(name: str) -> Any:
+    """Look up attributes dynamically."""
+    return _import_attribute(name)
+
 
 __all__ = [
     "StrictFormatter",
     "check_package_version",
     "comma_list",
     "convert_to_secret_str",
     "cosine_similarity",
     "cosine_similarity_top_k",
-    "formatter",
     "get_bolded_text",
     "get_color_mapping",
     "get_colored_text",
     "get_from_dict_or_env",
     "get_from_env",
+    "formatter",
     "get_pydantic_field_names",
     "guard_import",
     "mock_now",
     "print_text",
     "raise_for_status_with_text",
     "stringify_dict",
     "stringify_value",
```

### Comparing `gigachain-0.1.9/pyproject.toml` & `gigachain-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 [tool.poetry]
 name = "gigachain"
-version = "0.1.9"
+version = "0.2.0"
 description = "Building applications with LLMs through composability"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ai-forever/gigachain"
 packages = [
     {include = "langchain"}
 ]
 
 [tool.poetry.scripts]
 langchain-server = "langchain.server:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-gigachain-core = ">=0.1.26,<0.2"
-gigachain-community = ">=0.0.21,<0.1"
-langsmith = "^0.1.0"
-gigachat = ">=0.1.17"
+gigachain-core = "^0.2.0"
+gigachain-text-splitters = "^0.2.0"
+langsmith = "^0.1.17"
 pydantic = ">=1,<3"
 SQLAlchemy = ">=1.4,<3"
 requests = "^2"
 PyYAML = ">=5.3"
 numpy = "^1"
 aiohttp = "^3.8.3"
 tenacity = "^8.1.0"
-jsonpatch = "^1.33"
+gigachat = "^0.1.27"
 azure-core = {version = "^1.26.4", optional=true}
 tqdm = {version = ">=4.48.0", optional = true}
 openapi-pydantic = {version = "^0.3.2", optional = true}
 faiss-cpu = {version = "^1", optional = true}
 manifest-ml = {version = "^0.0.1", optional = true}
 transformers = {version = "^4", optional = true}
 beautifulsoup4 = {version = "^4", optional = true}
 torch = {version = ">=1,<3", optional = true}
 jinja2 = {version = "^3", optional = true}
-tiktoken = {version = ">=0.3.2,<0.6.0", optional = true, python=">=3.9"}
+tiktoken = {version = ">=0.7,<1.0", optional = true, python=">=3.9"}
 qdrant-client = {version = "^1.3.1", optional = true, python = ">=3.8.1,<3.12"}
 dataclasses-json = ">= 0.5.7, < 0.7"
-cohere = {version = "^4", optional = true}
+cohere = {version = ">=4,<6", optional = true}
 openai = {version = "<2", optional = true}
 nlpcloud = {version = "^1", optional = true}
 huggingface_hub = {version = "^0", optional = true}
 sentence-transformers = {version = "^2", optional = true}
 arxiv = {version = "^1.4", optional = true}
 pypdf = {version = "^3.4.0", optional = true}
 aleph-alpha-client = {version="^2.15.0", optional = true}
@@ -53,27 +52,26 @@
 atlassian-python-api = {version = "^3.36.0", optional=true}
 html2text = {version="^2020.1.16", optional=true}
 numexpr = {version="^2.8.6", optional=true}
 azure-cosmos = {version="^4.4.0b1", optional=true}
 jq = {version = "^1.4.1", optional = true}
 pdfminer-six = {version = "^20221105", optional = true}
 docarray = {version="^0.32.0", extras=["hnswlib"], optional=true}
-lxml = {version = "^4.9.2", optional = true}
+lxml = {version = ">=4.9.3,<6.0", optional = true}
 pymupdf = {version = "^1.22.3", optional = true}
 rapidocr-onnxruntime = {version = "^1.3.2", optional = true, python = ">=3.8.1,<3.12"}
 pypdfium2 = {version = "^4.10.0", optional = true}
 gql = {version = "^3.4.1", optional = true}
 pandas = {version = "^2.0.1", optional = true}
 telethon = {version = "^1.28.5", optional = true}
 chardet = {version="^5.1.0", optional=true}
 requests-toolbelt = {version = "^1.0.0", optional = true}
 openlm = {version = "^0.0.5", optional = true}
 scikit-learn = {version = "^1.2.2", optional = true}
 azure-ai-formrecognizer = {version = "^3.2.1", optional = true}
-azure-ai-vision = {version = "0.15.1b1", optional = true}
 azure-cognitiveservices-speech = {version = "^1.28.0", optional = true}
 py-trello = {version = "^0.19.0", optional = true}
 bibtexparser = {version = "^1.4.0", optional = true}
 pyspark = {version = "^3.4.0", optional = true}
 clarifai = {version = ">=9.1.0", optional = true}
 mwparserfromhell = {version = "^0.6.4", optional = true}
 mwxml = {version = "^0.3.3", optional = true}
@@ -110,15 +108,15 @@
 hologres-vector = {version = "^0.0.6", optional = true}
 praw = {version = "^7.7.1", optional = true}
 msal = {version = "^1.25.0", optional = true}
 databricks-vectorsearch = {version = "^0.21", optional = true}
 couchbase = {version = "^4.1.9", optional = true}
 dgml-utils = {version = "^0.3.0", optional = true}
 datasets = {version = "^2.15.0", optional = true}
-gigachain-openai = {version = ">=0.0.2,<0.1", optional = true}
+gigachain-openai = {version = "^0.1", optional = true}
 rdflib = {version = "7.0.0", optional = true}
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 # The only dependencies that should be added are
@@ -135,14 +133,16 @@
 lark = "^1.1.5"
 pandas = "^2.0.0"
 pytest-mock  = "^3.10.0"
 pytest-socket = "^0.6.0"
 syrupy = "^4.0.2"
 requests-mock = "^1.11.0"
 gigachain-core = {path = "../core", develop = true}
+gigachain-text-splitters = {path = "../text-splitters", develop = true}
+gigachain-openai = {path = "../partners/openai", optional = true, develop = true}
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
 
@@ -166,49 +166,50 @@
 # See the Contributing Guide for more instructions on working with optional dependencies.
 # https://python.langchain.com/docs/contributing/code#working-with-optional-dependencies
 pytest-vcr = "^1.0.2"
 wrapt = "^1.15.0"
 openai = "^1"
 python-dotenv = "^1.0.0"
 cassio = "^0.1.0"
-tiktoken = ">=0.3.2,<0.6.0"
+tiktoken = ">=0.7,<1"
 anthropic = "^0.3.11"
 gigachain-core = {path = "../core", develop = true}
-gigachain-community = {path = "../community", develop = true}
+gigachain-text-splitters = {path = "../text-splitters", develop = true}
+langchainhub = "^0.1.15"
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
 
 [tool.poetry.group.typing]
 optional = true
 
 [tool.poetry.group.typing.dependencies]
-mypy = "^0.991"
+mypy = "^1"
 types-pyyaml = "^6.0.12.2"
 types-requests = "^2.28.11.5"
 types-toml = "^0.10.8.1"
 types-redis = "^4.3.21.6"
 types-pytz = "^2023.3.0.0"
 types-chardet = "^5.0.4.6"
 mypy-protobuf = "^3.0.0"
 gigachain-core = {path = "../core", develop = true}
-gigachain-community = {path = "../community", develop = true}
+gigachain-text-splitters = {path = "../text-splitters", develop = true}
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 playwright = "^1.28.0"
 setuptools = "^67.6.1"
 gigachain-core = {path = "../core", develop = true}
-gigachain-community = {path = "../community", develop = true}
+gigachain-text-splitters = {path = "../text-splitters", develop = true}
 
 [tool.poetry.extras]
 llms = ["clarifai", "cohere", "openai", "openlm", "nlpcloud", "huggingface_hub", "manifest-ml", "torch", "transformers"]
 qdrant = ["qdrant-client"]
 openai = ["openai", "tiktoken"]
 text_helpers = ["chardet"]
 clarifai = ["clarifai"]
@@ -218,15 +219,14 @@
 javascript = ["esprima"]
 azure = [
     "azure-identity",
     "azure-cosmos",
     "openai",
     "azure-core",
     "azure-ai-formrecognizer",
-    "azure-ai-vision",
     "azure-cognitiveservices-speech",
     "azure-search-documents",
     "azure-ai-textanalytics",
 ]
 all = []
 cli = ["typer"]
```

### Comparing `gigachain-0.1.9/PKG-INFO` & `gigachain-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigachain
-Version: 0.1.9
+Version: 0.2.0
 Summary: Building applications with LLMs through composability
 Home-page: https://github.com/ai-forever/gigachain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -32,55 +32,53 @@
 Requires-Dist: anthropic (>=0.3.11,<0.4.0) ; extra == "extended-testing"
 Requires-Dist: arxiv (>=1.4,<2.0) ; extra == "extended-testing"
 Requires-Dist: assemblyai (>=0.17.0,<0.18.0) ; extra == "extended-testing"
 Requires-Dist: async-timeout (>=4.0.0,<5.0.0) ; python_version < "3.11"
 Requires-Dist: atlassian-python-api (>=3.36.0,<4.0.0) ; extra == "extended-testing"
 Requires-Dist: azure-ai-formrecognizer (>=3.2.1,<4.0.0) ; extra == "azure"
 Requires-Dist: azure-ai-textanalytics (>=5.3.0,<6.0.0) ; extra == "azure"
-Requires-Dist: azure-ai-vision (==0.15.1b1) ; extra == "azure"
 Requires-Dist: azure-cognitiveservices-speech (>=1.28.0,<2.0.0) ; extra == "azure"
 Requires-Dist: azure-core (>=1.26.4,<2.0.0) ; extra == "azure"
 Requires-Dist: azure-cosmos (>=4.4.0b1,<5.0.0) ; extra == "azure"
 Requires-Dist: azure-identity (>=1.12.0,<2.0.0) ; extra == "azure"
 Requires-Dist: azure-search-documents (==11.4.0b8) ; extra == "azure"
 Requires-Dist: beautifulsoup4 (>=4,<5) ; extra == "extended-testing"
 Requires-Dist: bibtexparser (>=1.4.0,<2.0.0) ; extra == "extended-testing"
 Requires-Dist: cassio (>=0.1.0,<0.2.0) ; extra == "extended-testing"
 Requires-Dist: chardet (>=5.1.0,<6.0.0) ; extra == "text-helpers" or extra == "extended-testing"
 Requires-Dist: clarifai (>=9.1.0) ; extra == "llms" or extra == "clarifai"
-Requires-Dist: cohere (>=4,<5) ; extra == "llms" or extra == "cohere" or extra == "extended-testing"
+Requires-Dist: cohere (>=4,<6) ; extra == "llms" or extra == "cohere" or extra == "extended-testing"
 Requires-Dist: couchbase (>=4.1.9,<5.0.0) ; extra == "extended-testing"
 Requires-Dist: dashvector (>=1.0.1,<2.0.0) ; extra == "extended-testing"
 Requires-Dist: databricks-vectorsearch (>=0.21,<0.22) ; extra == "extended-testing"
 Requires-Dist: dataclasses-json (>=0.5.7,<0.7)
 Requires-Dist: datasets (>=2.15.0,<3.0.0) ; extra == "extended-testing"
 Requires-Dist: dgml-utils (>=0.3.0,<0.4.0) ; extra == "extended-testing"
 Requires-Dist: docarray[hnswlib] (>=0.32.0,<0.33.0) ; extra == "docarray"
 Requires-Dist: esprima (>=4.0.1,<5.0.0) ; extra == "javascript" or extra == "extended-testing"
 Requires-Dist: faiss-cpu (>=1,<2) ; extra == "extended-testing"
 Requires-Dist: feedparser (>=6.0.10,<7.0.0) ; extra == "extended-testing"
 Requires-Dist: fireworks-ai (>=0.9.0,<0.10.0) ; extra == "extended-testing"
 Requires-Dist: geopandas (>=0.13.1,<0.14.0) ; extra == "extended-testing"
-Requires-Dist: gigachain-community (>=0.0.21,<0.1)
-Requires-Dist: gigachain-core (>=0.1.26,<0.2)
-Requires-Dist: gigachain-openai (>=0.0.2,<0.1) ; extra == "extended-testing"
-Requires-Dist: gigachat (>=0.1.17)
+Requires-Dist: gigachain-core (>=0.2.0,<0.3.0)
+Requires-Dist: gigachain-openai (>=0.1,<0.2) ; extra == "extended-testing"
+Requires-Dist: gigachain-text-splitters (>=0.2.0,<0.3.0)
+Requires-Dist: gigachat (>=0.1.27,<0.2.0)
 Requires-Dist: gitpython (>=3.1.32,<4.0.0) ; extra == "extended-testing"
 Requires-Dist: google-cloud-documentai (>=2.20.1,<3.0.0) ; extra == "extended-testing"
 Requires-Dist: gql (>=3.4.1,<4.0.0) ; extra == "extended-testing"
 Requires-Dist: hologres-vector (>=0.0.6,<0.0.7) ; extra == "extended-testing"
 Requires-Dist: html2text (>=2020.1.16,<2021.0.0) ; extra == "extended-testing"
 Requires-Dist: huggingface_hub (>=0,<1) ; extra == "llms"
 Requires-Dist: javelin-sdk (>=0.1.8,<0.2.0) ; extra == "extended-testing"
 Requires-Dist: jinja2 (>=3,<4) ; extra == "extended-testing"
 Requires-Dist: jq (>=1.4.1,<2.0.0) ; extra == "extended-testing"
-Requires-Dist: jsonpatch (>=1.33,<2.0)
 Requires-Dist: jsonschema (>1) ; extra == "extended-testing"
-Requires-Dist: langsmith (>=0.1.0,<0.2.0)
-Requires-Dist: lxml (>=4.9.2,<5.0.0) ; extra == "extended-testing"
+Requires-Dist: langsmith (>=0.1.17,<0.2.0)
+Requires-Dist: lxml (>=4.9.3,<6.0) ; extra == "extended-testing"
 Requires-Dist: manifest-ml (>=0.0.1,<0.0.2) ; extra == "llms"
 Requires-Dist: markdownify (>=0.11.6,<0.12.0) ; extra == "extended-testing"
 Requires-Dist: motor (>=3.3.1,<4.0.0) ; extra == "extended-testing"
 Requires-Dist: msal (>=1.25.0,<2.0.0) ; extra == "extended-testing"
 Requires-Dist: mwparserfromhell (>=0.6.4,<0.7.0) ; extra == "extended-testing"
 Requires-Dist: mwxml (>=0.3.3,<0.4.0) ; extra == "extended-testing"
 Requires-Dist: newspaper3k (>=0.2.8,<0.3.0) ; extra == "extended-testing"
@@ -112,15 +110,15 @@
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0) ; extra == "extended-testing"
 Requires-Dist: sentence-transformers (>=2,<3) ; extra == "embeddings"
 Requires-Dist: sqlite-vss (>=0.1.2,<0.2.0) ; extra == "extended-testing"
 Requires-Dist: streamlit (>=1.18.0,<2.0.0) ; (python_full_version >= "3.8.1" and python_full_version != "3.9.7" and python_version < "4.0") and (extra == "extended-testing")
 Requires-Dist: sympy (>=1.12,<2.0) ; extra == "extended-testing"
 Requires-Dist: telethon (>=1.28.5,<2.0.0) ; extra == "extended-testing"
 Requires-Dist: tenacity (>=8.1.0,<9.0.0)
-Requires-Dist: tiktoken (>=0.3.2,<0.6.0) ; (python_version >= "3.9") and (extra == "openai")
+Requires-Dist: tiktoken (>=0.7,<1.0) ; (python_version >= "3.9") and (extra == "openai")
 Requires-Dist: timescale-vector (>=0.0.1,<0.0.2) ; extra == "extended-testing"
 Requires-Dist: torch (>=1,<3) ; extra == "llms"
 Requires-Dist: tqdm (>=4.48.0) ; extra == "extended-testing"
 Requires-Dist: transformers (>=4,<5) ; extra == "llms"
 Requires-Dist: typer (>=0.9.0,<0.10.0) ; extra == "cli"
 Requires-Dist: upstash-redis (>=0.15.0,<0.16.0) ; extra == "extended-testing"
 Requires-Dist: xata (>=1.0.0a7,<2.0.0) ; extra == "extended-testing"
@@ -160,63 +158,59 @@
 
 ## 🤔 What is this?
 
 Large language models (LLMs) are emerging as a transformative technology, enabling developers to build applications that they previously could not. However, using these LLMs in isolation is often insufficient for creating a truly powerful app - the real power comes when you can combine them with other sources of computation or knowledge.
 
 This library aims to assist in the development of those types of applications. Common examples of these applications include:
 
-**❓ Question Answering over specific documents**
+**❓ Question answering with RAG**
 
 - [Documentation](https://python.langchain.com/docs/use_cases/question_answering/)
-- End-to-end Example: [Question Answering over Notion Database](https://github.com/hwchase17/notion-qa)
+- End-to-end Example: [Chat LangChain](https://chat.langchain.com) and [repo](https://github.com/langchain-ai/chat-langchain)
 
-**💬 Chatbots**
+**🧱 Extracting structured output**
 
-- [Documentation](https://python.langchain.com/docs/use_cases/chatbots/)
-- End-to-end Example: [Chat-LangChain](https://github.com/langchain-ai/chat-langchain)
+- [Documentation](https://python.langchain.com/docs/use_cases/extraction/)
+- End-to-end Example: [SQL Llama2 Template](https://github.com/langchain-ai/langchain-extract/)
 
-**🤖 Agents**
+**🤖 Chatbots**
 
-- [Documentation](https://python.langchain.com/docs/modules/agents/)
-- End-to-end Example: [GPT+WolframAlpha](https://huggingface.co/spaces/JavaFXpert/Chat-GPT-LangChain)
+- [Documentation](https://python.langchain.com/docs/use_cases/chatbots)
+- End-to-end Example: [Web LangChain (web researcher chatbot)](https://weblangchain.vercel.app) and [repo](https://github.com/langchain-ai/weblangchain)
 
 ## 📖 Documentation
 
 Please see [here](https://python.langchain.com) for full documentation on:
 
 - Getting started (installation, setting up the environment, simple examples)
 - How-To examples (demos, integrations, helper functions)
 - Reference (full API docs)
 - Resources (high-level explanation of core concepts)
 
 ## 🚀 What can this help with?
 
-There are six main areas that LangChain is designed to help with.
+There are five main areas that LangChain is designed to help with.
 These are, in increasing order of complexity:
 
-**📃 LLMs and Prompts:**
+**📃 Models and Prompts:**
 
-This includes prompt management, prompt optimization, a generic interface for all LLMs, and common utilities for working with LLMs.
+This includes prompt management, prompt optimization, a generic interface for all LLMs, and common utilities for working with chat models and LLMs.
 
 **🔗 Chains:**
 
 Chains go beyond a single LLM call and involve sequences of calls (whether to an LLM or a different utility). LangChain provides a standard interface for chains, lots of integrations with other tools, and end-to-end chains for common applications.
 
-**📚 Data Augmented Generation:**
+**📚 Retrieval Augmented Generation:**
 
-Data Augmented Generation involves specific types of chains that first interact with an external data source to fetch data for use in the generation step. Examples include summarization of long pieces of text and question/answering over specific data sources.
+Retrieval Augmented Generation involves specific types of chains that first interact with an external data source to fetch data for use in the generation step. Examples include summarization of long pieces of text and question/answering over specific data sources.
 
 **🤖 Agents:**
 
 Agents involve an LLM making decisions about which Actions to take, taking that Action, seeing an Observation, and repeating that until done. LangChain provides a standard interface for agents, a selection of agents to choose from, and examples of end-to-end agents.
 
-**🧠 Memory:**
-
-Memory refers to persisting state between calls of a chain/agent. LangChain provides a standard interface for memory, a collection of memory implementations, and examples of chains/agents that use memory.
-
 **🧐 Evaluation:**
 
 [BETA] Generative models are notoriously hard to evaluate with traditional metrics. One new way of evaluating them is using language models themselves to do the evaluation. LangChain provides some prompts/chains for assisting in this.
 
 For more information on these concepts, please see our [full documentation](https://python.langchain.com).
 
 ## 💁 Contributing
```

