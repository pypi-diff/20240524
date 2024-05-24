# Comparing `tmp/openagi-0.2.0b2.tar.gz` & `tmp/openagi-0.2.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openagi-0.2.0b2.tar", max compression
+gzip compressed data, was "openagi-0.2.1b2.tar", max compression
```

## Comparing `openagi-0.2.0b2.tar` & `openagi-0.2.1b2.tar`

### file list

```diff
@@ -1,78 +1,80 @@
--rw-r--r--   0        0        0     8953 2024-05-21 17:32:13.916710 openagi-0.2.0b2/README.md
--rw-r--r--   0        0        0     1197 2024-05-21 17:37:51.570525 openagi-0.2.0b2/pyproject.toml
--rw-r--r--   0        0        0     1499 2024-04-19 10:30:02.396089 openagi-0.2.0b2/src/Readme.md
--rw-r--r--   0        0        0      558 2024-05-21 17:32:13.930709 openagi-0.2.0b2/src/openagi/__init__.py
--rw-r--r--   0        0        0      183 2024-05-21 17:32:13.930709 openagi-0.2.0b2/src/openagi/actions/__init__.py
--rw-r--r--   0        0        0     1667 2024-05-21 17:32:13.931710 openagi-0.2.0b2/src/openagi/actions/base.py
--rw-r--r--   0        0        0      511 2024-05-21 17:32:13.931710 openagi-0.2.0b2/src/openagi/actions/compressor.py
--rw-r--r--   0        0        0      381 2024-05-21 17:32:13.931710 openagi-0.2.0b2/src/openagi/actions/console.py
--rw-r--r--   0        0        0     1990 2024-05-21 17:32:13.933709 openagi-0.2.0b2/src/openagi/actions/files.py
--rw-r--r--   0        0        0      724 2024-05-21 17:32:13.933709 openagi-0.2.0b2/src/openagi/actions/formatter.py
--rw-r--r--   0        0        0      404 2024-05-21 17:32:13.934710 openagi-0.2.0b2/src/openagi/actions/human_input.py
--rw-r--r--   0        0        0     1114 2024-05-21 17:32:13.934710 openagi-0.2.0b2/src/openagi/actions/obs_rag.py
--rw-r--r--   0        0        0       80 2024-05-21 17:32:13.934710 openagi-0.2.0b2/src/openagi/actions/tools/__init__.py
--rw-r--r--   0        0        0     1052 2024-05-21 17:32:13.935710 openagi-0.2.0b2/src/openagi/actions/tools/ddg_search.py
--rw-r--r--   0        0        0     1925 2024-05-21 17:32:13.935710 openagi-0.2.0b2/src/openagi/actions/tools/serp_search.py
--rw-r--r--   0        0        0      948 2024-05-21 17:32:13.936710 openagi-0.2.0b2/src/openagi/actions/tools/serper_search.py
--rw-r--r--   0        0        0        0 2024-05-21 17:32:13.936710 openagi-0.2.0b2/src/openagi/actions/utils.py
--rw-r--r--   0        0        0     7702 2024-05-21 17:32:13.939710 openagi-0.2.0b2/src/openagi/agent.py
--rw-r--r--   0        0        0      117 2024-05-21 17:32:13.942710 openagi-0.2.0b2/src/openagi/exception.py
--rw-r--r--   0        0        0     3398 2024-04-19 10:30:02.397089 openagi-0.2.0b2/src/openagi/init_agent.py
--rw-r--r--   0        0        0      196 2024-04-19 10:30:02.397089 openagi-0.2.0b2/src/openagi/llms/__init__.py
--rw-r--r--   0        0        0     2356 2024-05-21 17:32:13.943709 openagi-0.2.0b2/src/openagi/llms/azure.py
--rw-r--r--   0        0        0     1272 2024-05-21 17:32:13.943709 openagi-0.2.0b2/src/openagi/llms/base.py
--rw-r--r--   0        0        0     1609 2024-05-21 17:32:13.943709 openagi-0.2.0b2/src/openagi/llms/hf.py
--rw-r--r--   0        0        0      713 2024-05-21 17:32:13.944709 openagi-0.2.0b2/src/openagi/llms/openagi_main.py
--rw-r--r--   0        0        0     1754 2024-05-21 17:32:13.944709 openagi-0.2.0b2/src/openagi/llms/openai.py
--rw-r--r--   0        0        0       27 2024-05-21 17:32:13.944709 openagi-0.2.0b2/src/openagi/memory/__init__.py
--rw-r--r--   0        0        0     2132 2024-05-21 17:32:13.944709 openagi-0.2.0b2/src/openagi/memory/base.py
--rw-r--r--   0        0        0       80 2024-05-21 17:32:13.944709 openagi-0.2.0b2/src/openagi/memory/memory.py
--rw-r--r--   0        0        0        0 2024-05-21 17:32:13.944709 openagi-0.2.0b2/src/openagi/planner/LATS.py
--rw-r--r--   0        0        0       45 2024-05-01 10:04:19.838349 openagi-0.2.0b2/src/openagi/planner/__init__.py
--rw-r--r--   0        0        0      914 2024-05-21 17:32:13.945710 openagi-0.2.0b2/src/openagi/planner/base.py
--rw-r--r--   0        0        0        0 2024-05-21 17:32:13.945710 openagi-0.2.0b2/src/openagi/planner/reflexion.py
--rw-r--r--   0        0        0     2165 2024-05-21 17:32:13.945710 openagi-0.2.0b2/src/openagi/planner/task_decomposer.py
--rw-r--r--   0        0        0        0 2024-05-01 09:44:08.540909 openagi-0.2.0b2/src/openagi/prompts/__init__.py
--rw-r--r--   0        0        0     1005 2024-05-21 17:32:13.945710 openagi-0.2.0b2/src/openagi/prompts/base.py
--rw-r--r--   0        0        0      145 2024-05-21 17:32:13.946709 openagi-0.2.0b2/src/openagi/prompts/constants.py
--rw-r--r--   0        0        0     2940 2024-05-21 17:32:13.946709 openagi-0.2.0b2/src/openagi/prompts/execution.py
--rw-r--r--   0        0        0     3034 2024-05-21 17:32:13.946709 openagi-0.2.0b2/src/openagi/prompts/task_creator.py
--rw-r--r--   0        0        0        0 2024-05-21 17:32:13.946709 openagi-0.2.0b2/src/openagi/storage/__init__.py
--rw-r--r--   0        0        0      943 2024-05-21 17:32:13.946709 openagi-0.2.0b2/src/openagi/storage/base.py
--rw-r--r--   0        0        0     2339 2024-05-21 17:32:13.947709 openagi-0.2.0b2/src/openagi/storage/chroma.py
--rw-r--r--   0        0        0       78 2024-05-02 13:26:09.326553 openagi-0.2.0b2/src/openagi/tasks/__init__.py
--rw-r--r--   0        0        0     1236 2024-05-21 17:32:13.947709 openagi-0.2.0b2/src/openagi/tasks/lists.py
--rw-r--r--   0        0        0      787 2024-05-21 17:32:13.947709 openagi-0.2.0b2/src/openagi/tasks/task.py
--rw-r--r--   0        0        0       28 2024-04-19 10:30:02.398089 openagi-0.2.0b2/src/openagi/tools/__init__.py
--rw-r--r--   0        0        0     2078 2024-04-23 06:32:39.897436 openagi-0.2.0b2/src/openagi/tools/base.py
--rw-r--r--   0        0        0      762 2024-04-19 10:30:02.398089 openagi-0.2.0b2/src/openagi/tools/custom_tools/ProxyTool.py
--rw-r--r--   0        0        0      212 2024-04-19 10:30:02.398089 openagi-0.2.0b2/src/openagi/tools/custom_tools/custom_tool_db.py
--rw-r--r--   0        0        0     1292 2024-04-19 10:30:02.398089 openagi-0.2.0b2/src/openagi/tools/integrations/__init__.py
--rw-r--r--   0        0        0      581 2024-04-19 10:30:02.398089 openagi-0.2.0b2/src/openagi/tools/integrations/dalle_image_generator.py
--rw-r--r--   0        0        0     2806 2024-05-21 17:32:13.947709 openagi-0.2.0b2/src/openagi/tools/integrations/document_compare.py
--rw-r--r--   0        0        0     1045 2024-04-23 06:32:39.899436 openagi-0.2.0b2/src/openagi/tools/integrations/duckducksearch.py
--rw-r--r--   0        0        0     1527 2024-04-19 10:30:02.399089 openagi-0.2.0b2/src/openagi/tools/integrations/exa_search_tool.py
--rw-r--r--   0        0        0     1733 2024-05-21 17:32:13.948710 openagi-0.2.0b2/src/openagi/tools/integrations/github.py
--rw-r--r--   0        0        0     1589 2024-05-21 17:32:13.948710 openagi-0.2.0b2/src/openagi/tools/integrations/gmail.py
--rw-r--r--   0        0        0      277 2024-05-21 17:32:13.948710 openagi-0.2.0b2/src/openagi/tools/integrations/google.py
--rw-r--r--   0        0        0     1424 2024-05-21 17:32:13.948710 openagi-0.2.0b2/src/openagi/tools/integrations/google_finance_search.py
--rw-r--r--   0        0        0     1351 2024-05-21 17:32:13.949710 openagi-0.2.0b2/src/openagi/tools/integrations/google_serper_specific.py
--rw-r--r--   0        0        0     1160 2024-04-19 10:30:02.399089 openagi-0.2.0b2/src/openagi/tools/integrations/googlejobsearch.py
--rw-r--r--   0        0        0      841 2024-04-19 10:30:02.399089 openagi-0.2.0b2/src/openagi/tools/integrations/googleserpersearch.py
--rw-r--r--   0        0        0     1350 2024-04-19 10:30:02.399089 openagi-0.2.0b2/src/openagi/tools/integrations/nasa.py
--rw-r--r--   0        0        0      844 2024-04-19 10:30:02.399089 openagi-0.2.0b2/src/openagi/tools/integrations/open_weathermap.py
--rw-r--r--   0        0        0     1743 2024-04-19 10:30:02.399089 openagi-0.2.0b2/src/openagi/tools/integrations/polygon.py
--rw-r--r--   0        0        0     1444 2024-04-19 10:30:02.400089 openagi-0.2.0b2/src/openagi/tools/integrations/serper_intermediate.py
--rw-r--r--   0        0        0     1351 2024-05-21 17:32:13.950709 openagi-0.2.0b2/src/openagi/tools/integrations/sql.py
--rw-r--r--   0        0        0     1141 2024-04-19 10:30:02.400089 openagi-0.2.0b2/src/openagi/tools/integrations/wikipedia_tool.py
--rw-r--r--   0        0        0     1242 2024-05-21 17:32:13.950709 openagi-0.2.0b2/src/openagi/tools/integrations/xorbits.py
--rw-r--r--   0        0        0     1315 2024-04-19 10:30:02.400089 openagi-0.2.0b2/src/openagi/tools/integrations/yahoofinancenews.py
--rw-r--r--   0        0        0      945 2024-04-19 10:30:02.400089 openagi-0.2.0b2/src/openagi/tools/integrations/youtubesearch.py
--rw-r--r--   0        0        0     3198 2024-04-19 10:30:02.400089 openagi-0.2.0b2/src/openagi/tools/tools_db.py
--rw-r--r--   0        0        0     3246 2024-05-21 17:32:13.950709 openagi-0.2.0b2/src/openagi/tools/utils.py
--rw-r--r--   0        0        0     3017 2024-05-21 17:32:13.951709 openagi-0.2.0b2/src/openagi/utils/extraction.py
--rw-r--r--   0        0        0    13792 2024-04-30 05:51:06.030343 openagi-0.2.0b2/src/openagi/utils/llmTasks.py
--rw-r--r--   0        0        0      260 2024-05-21 17:32:13.951709 openagi-0.2.0b2/src/openagi/utils/yamlParse.py
--rw-r--r--   0        0        0        0 2024-05-21 17:32:13.951709 openagi-0.2.0b2/src/openagi/worker/__init__.py
--rw-r--r--   0        0        0      589 2024-05-21 17:32:13.951709 openagi-0.2.0b2/src/openagi/worker/worker.py
--rw-r--r--   0        0        0    10730 1970-01-01 00:00:00.000000 openagi-0.2.0b2/PKG-INFO
+-rw-r--r--   0        0        0     8967 2024-05-24 06:07:38.633561 openagi-0.2.1b2/README.md
+-rw-r--r--   0        0        0     1240 2024-05-24 11:12:29.946358 openagi-0.2.1b2/pyproject.toml
+-rw-r--r--   0        0        0     1499 2024-04-19 10:30:02.396089 openagi-0.2.1b2/src/Readme.md
+-rw-r--r--   0        0        0      558 2024-05-21 17:32:13.930709 openagi-0.2.1b2/src/openagi/__init__.py
+-rw-r--r--   0        0        0      183 2024-05-21 17:32:13.930709 openagi-0.2.1b2/src/openagi/actions/__init__.py
+-rw-r--r--   0        0        0     1533 2024-05-24 11:12:22.653358 openagi-0.2.1b2/src/openagi/actions/base.py
+-rw-r--r--   0        0        0      511 2024-05-24 06:07:38.642561 openagi-0.2.1b2/src/openagi/actions/compressor.py
+-rw-r--r--   0        0        0      381 2024-05-21 17:32:13.931710 openagi-0.2.1b2/src/openagi/actions/console.py
+-rw-r--r--   0        0        0     1990 2024-05-21 17:32:13.933709 openagi-0.2.1b2/src/openagi/actions/files.py
+-rw-r--r--   0        0        0      724 2024-05-24 06:07:38.642561 openagi-0.2.1b2/src/openagi/actions/formatter.py
+-rw-r--r--   0        0        0      404 2024-05-21 17:32:13.934710 openagi-0.2.1b2/src/openagi/actions/human_input.py
+-rw-r--r--   0        0        0      847 2024-05-22 09:24:08.834622 openagi-0.2.1b2/src/openagi/actions/obs_rag.py
+-rw-r--r--   0        0        0      168 2024-05-24 06:03:09.214412 openagi-0.2.1b2/src/openagi/actions/tools/__init__.py
+-rw-r--r--   0        0        0     1430 2024-05-22 09:23:19.372839 openagi-0.2.1b2/src/openagi/actions/tools/ddg_search.py
+-rw-r--r--   0        0        0     1925 2024-05-21 17:32:13.935710 openagi-0.2.1b2/src/openagi/actions/tools/serp_search.py
+-rw-r--r--   0        0        0      948 2024-05-21 17:32:13.936710 openagi-0.2.1b2/src/openagi/actions/tools/serper_search.py
+-rw-r--r--   0        0        0     1598 2024-05-24 11:12:22.653358 openagi-0.2.1b2/src/openagi/actions/tools/webloader.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:07:38.642561 openagi-0.2.1b2/src/openagi/actions/utils.py
+-rw-r--r--   0        0        0     7807 2024-05-24 06:07:38.645561 openagi-0.2.1b2/src/openagi/agent.py
+-rw-r--r--   0        0        0      117 2024-05-21 17:32:13.942710 openagi-0.2.1b2/src/openagi/exception.py
+-rw-r--r--   0        0        0     3398 2024-04-19 10:30:02.397089 openagi-0.2.1b2/src/openagi/init_agent.py
+-rw-r--r--   0        0        0      196 2024-04-19 10:30:02.397089 openagi-0.2.1b2/src/openagi/llms/__init__.py
+-rw-r--r--   0        0        0     2356 2024-05-21 17:32:13.943709 openagi-0.2.1b2/src/openagi/llms/azure.py
+-rw-r--r--   0        0        0     1272 2024-05-21 17:32:13.943709 openagi-0.2.1b2/src/openagi/llms/base.py
+-rw-r--r--   0        0        0     1609 2024-05-21 17:32:13.943709 openagi-0.2.1b2/src/openagi/llms/hf.py
+-rw-r--r--   0        0        0      713 2024-05-21 17:32:13.944709 openagi-0.2.1b2/src/openagi/llms/openagi_main.py
+-rw-r--r--   0        0        0     1754 2024-05-21 17:32:13.944709 openagi-0.2.1b2/src/openagi/llms/openai.py
+-rw-r--r--   0        0        0       27 2024-05-21 17:32:13.944709 openagi-0.2.1b2/src/openagi/memory/__init__.py
+-rw-r--r--   0        0        0     3160 2024-05-22 10:04:24.213949 openagi-0.2.1b2/src/openagi/memory/base.py
+-rw-r--r--   0        0        0       80 2024-05-21 17:32:13.944709 openagi-0.2.1b2/src/openagi/memory/memory.py
+-rw-r--r--   0        0        0        0 2024-05-21 17:32:13.944709 openagi-0.2.1b2/src/openagi/planner/LATS.py
+-rw-r--r--   0        0        0       45 2024-05-01 10:04:19.838349 openagi-0.2.1b2/src/openagi/planner/__init__.py
+-rw-r--r--   0        0        0      914 2024-05-21 17:32:13.945710 openagi-0.2.1b2/src/openagi/planner/base.py
+-rw-r--r--   0        0        0        0 2024-05-21 17:32:13.945710 openagi-0.2.1b2/src/openagi/planner/reflexion.py
+-rw-r--r--   0        0        0     2150 2024-05-22 10:04:31.900914 openagi-0.2.1b2/src/openagi/planner/task_decomposer.py
+-rw-r--r--   0        0        0        0 2024-05-01 09:44:08.540909 openagi-0.2.1b2/src/openagi/prompts/__init__.py
+-rw-r--r--   0        0        0     1005 2024-05-21 17:32:13.945710 openagi-0.2.1b2/src/openagi/prompts/base.py
+-rw-r--r--   0        0        0      145 2024-05-21 17:32:13.946709 openagi-0.2.1b2/src/openagi/prompts/constants.py
+-rw-r--r--   0        0        0     2940 2024-05-21 17:32:13.946709 openagi-0.2.1b2/src/openagi/prompts/execution.py
+-rw-r--r--   0        0        0     3333 2024-05-22 09:37:18.000151 openagi-0.2.1b2/src/openagi/prompts/task_creator.py
+-rw-r--r--   0        0        0        0 2024-05-21 17:32:13.946709 openagi-0.2.1b2/src/openagi/storage/__init__.py
+-rw-r--r--   0        0        0      943 2024-05-21 17:32:13.946709 openagi-0.2.1b2/src/openagi/storage/base.py
+-rw-r--r--   0        0        0     2175 2024-05-22 09:59:06.159369 openagi-0.2.1b2/src/openagi/storage/chroma.py
+-rw-r--r--   0        0        0       78 2024-05-02 13:26:09.326553 openagi-0.2.1b2/src/openagi/tasks/__init__.py
+-rw-r--r--   0        0        0     1236 2024-05-21 17:32:13.947709 openagi-0.2.1b2/src/openagi/tasks/lists.py
+-rw-r--r--   0        0        0      787 2024-05-21 17:32:13.947709 openagi-0.2.1b2/src/openagi/tasks/task.py
+-rw-r--r--   0        0        0       28 2024-04-19 10:30:02.398089 openagi-0.2.1b2/src/openagi/tools/__init__.py
+-rw-r--r--   0        0        0     2078 2024-04-23 06:32:39.897436 openagi-0.2.1b2/src/openagi/tools/base.py
+-rw-r--r--   0        0        0      762 2024-04-19 10:30:02.398089 openagi-0.2.1b2/src/openagi/tools/custom_tools/ProxyTool.py
+-rw-r--r--   0        0        0      212 2024-04-19 10:30:02.398089 openagi-0.2.1b2/src/openagi/tools/custom_tools/custom_tool_db.py
+-rw-r--r--   0        0        0     1292 2024-04-19 10:30:02.398089 openagi-0.2.1b2/src/openagi/tools/integrations/__init__.py
+-rw-r--r--   0        0        0      581 2024-04-19 10:30:02.398089 openagi-0.2.1b2/src/openagi/tools/integrations/dalle_image_generator.py
+-rw-r--r--   0        0        0     2806 2024-05-21 17:32:13.947709 openagi-0.2.1b2/src/openagi/tools/integrations/document_compare.py
+-rw-r--r--   0        0        0     1045 2024-04-23 06:32:39.899436 openagi-0.2.1b2/src/openagi/tools/integrations/duckducksearch.py
+-rw-r--r--   0        0        0     1527 2024-04-19 10:30:02.399089 openagi-0.2.1b2/src/openagi/tools/integrations/exa_search_tool.py
+-rw-r--r--   0        0        0     1733 2024-05-21 17:32:13.948710 openagi-0.2.1b2/src/openagi/tools/integrations/github.py
+-rw-r--r--   0        0        0     1589 2024-05-21 17:32:13.948710 openagi-0.2.1b2/src/openagi/tools/integrations/gmail.py
+-rw-r--r--   0        0        0      277 2024-05-21 17:32:13.948710 openagi-0.2.1b2/src/openagi/tools/integrations/google.py
+-rw-r--r--   0        0        0     1424 2024-05-21 17:32:13.948710 openagi-0.2.1b2/src/openagi/tools/integrations/google_finance_search.py
+-rw-r--r--   0        0        0     1351 2024-05-21 17:32:13.949710 openagi-0.2.1b2/src/openagi/tools/integrations/google_serper_specific.py
+-rw-r--r--   0        0        0     1160 2024-04-19 10:30:02.399089 openagi-0.2.1b2/src/openagi/tools/integrations/googlejobsearch.py
+-rw-r--r--   0        0        0      841 2024-04-19 10:30:02.399089 openagi-0.2.1b2/src/openagi/tools/integrations/googleserpersearch.py
+-rw-r--r--   0        0        0     1350 2024-04-19 10:30:02.399089 openagi-0.2.1b2/src/openagi/tools/integrations/nasa.py
+-rw-r--r--   0        0        0      844 2024-04-19 10:30:02.399089 openagi-0.2.1b2/src/openagi/tools/integrations/open_weathermap.py
+-rw-r--r--   0        0        0     1743 2024-04-19 10:30:02.399089 openagi-0.2.1b2/src/openagi/tools/integrations/polygon.py
+-rw-r--r--   0        0        0     1444 2024-04-19 10:30:02.400089 openagi-0.2.1b2/src/openagi/tools/integrations/serper_intermediate.py
+-rw-r--r--   0        0        0     1351 2024-05-21 17:32:13.950709 openagi-0.2.1b2/src/openagi/tools/integrations/sql.py
+-rw-r--r--   0        0        0     1141 2024-04-19 10:30:02.400089 openagi-0.2.1b2/src/openagi/tools/integrations/wikipedia_tool.py
+-rw-r--r--   0        0        0     1242 2024-05-21 17:32:13.950709 openagi-0.2.1b2/src/openagi/tools/integrations/xorbits.py
+-rw-r--r--   0        0        0     1315 2024-04-19 10:30:02.400089 openagi-0.2.1b2/src/openagi/tools/integrations/yahoofinancenews.py
+-rw-r--r--   0        0        0      945 2024-04-19 10:30:02.400089 openagi-0.2.1b2/src/openagi/tools/integrations/youtubesearch.py
+-rw-r--r--   0        0        0     3198 2024-04-19 10:30:02.400089 openagi-0.2.1b2/src/openagi/tools/tools_db.py
+-rw-r--r--   0        0        0     3246 2024-05-21 17:32:13.950709 openagi-0.2.1b2/src/openagi/tools/utils.py
+-rw-r--r--   0        0        0     3017 2024-05-21 17:32:13.951709 openagi-0.2.1b2/src/openagi/utils/extraction.py
+-rw-r--r--   0        0        0      155 2024-05-24 06:07:38.645561 openagi-0.2.1b2/src/openagi/utils/helper.py
+-rw-r--r--   0        0        0    13792 2024-04-30 05:51:06.030343 openagi-0.2.1b2/src/openagi/utils/llmTasks.py
+-rw-r--r--   0        0        0      260 2024-05-21 17:32:13.951709 openagi-0.2.1b2/src/openagi/utils/yamlParse.py
+-rw-r--r--   0        0        0        0 2024-05-21 17:32:13.951709 openagi-0.2.1b2/src/openagi/worker/__init__.py
+-rw-r--r--   0        0        0      589 2024-05-21 17:32:13.951709 openagi-0.2.1b2/src/openagi/worker/worker.py
+-rw-r--r--   0        0        0    10830 1970-01-01 00:00:00.000000 openagi-0.2.1b2/PKG-INFO
```

### Comparing `openagi-0.2.0b2/README.md` & `openagi-0.2.1b2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 <div align="center">
 <h1 align="center">OpenAGI </h1>
 <h2 align="center">Making the development of autonomous human-like agents accessible to all</h2>
 
-<a href="https://img.shields.io/badge/Python-3.11-3776AB.svg?style=flat&logo=python&logoColor=white"><img src="https://img.shields.io/badge/Python-3.11-3776AB.svg?style=flat&logo=python&logoColor=white" alt="Python 3.11"></a>
+<a href="https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11-3776AB.svg?style=flat&logo=python&logoColor=white"><img src="https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11-3776AB.svg?style=flat&logo=python&logoColor=white" alt="Python Versions"></a>
 <a href="https://discord.gg/4aWV7He2QU"><img src="https://dcbadge.vercel.app/api/server/4aWV7He2QU?style=flat" alt="Discord" /></a>
 <a href="https://twitter.com/aiplanethub"><img src="https://img.shields.io/twitter/follow/aiplanethub" alt="Twitter" /></a>
 
 <p>OpenAGI aims to make human-like agents accessible to everyone, thereby paving the way towards open agents and, eventually, AGI for everyone. We strongly believe in the transformative power of AI and are confident that this initiative will significantly contribute to solving many real-life problems. Currently, OpenAGI is designed to offer developers a framework for creating autonomous human-like agents.</p>
 <i><a href="https://discord.gg/4aWV7He2QU">👉 Join our Discord community!</a></i>
 </div>
 
-
 ## Installation
 
 1. Setup a virtual environment.
 
-    ```bash
-    # For Mac users
-    python3 -m venv venv
-    source venv/bin/activate
-
-    # For Windows users
-    python -m venv venv
-    venv/scripts/activate
-
-    # to create virtual env using particular python version (in Windows)
-    py -3.11 -m venv venv
-    ```
+   ```bash
+   # For Mac users
+   python3 -m venv venv
+   source venv/bin/activate
+
+   # For Windows users
+   python -m venv venv
+   venv/scripts/activate
+
+   # to create virtual env using particular python version (in Windows)
+   py -3.11 -m venv venv
+   ```
 
 2. Install the openagi
 
    ```bash
    pip install openagi
    ```
 
@@ -44,16 +43,16 @@
 
 ## Understand OpenAGI
 
 ![Thumbnails](https://github.com/aiplanethub/openagi/blob/dev/assets/openagi.png)
 
 ## Example
 
-Follow this example to create a Test Case job search it help you to search available job posting for a given category
-Here in the example we are using AzureChatOpenAIModel along with GoogleSerpAPISearch to search the internet for various job posting on the particular role.
+Follow this example to create a **Job Search Agent** that helps you to search available job posting for a given category.
+Here in the example we are using `AzureChatOpenAIModel` along with `GoogleSerpAPISearch` to search the internet for various job posting on the particular role.
 
 **Note:** Follow setup guide to configure the environment. For quick access click [here](https://openagi.aiplanet.com/getting-started/installation).
 
 ```python
 from openagi.actions.tools.serp_search import GoogleSerpAPISearch
 from openagi.agent import Admin
 from openagi.llms.azure import AzureChatOpenAIModel
@@ -93,18 +92,19 @@
         query=query,
         description="You are an expert Internet searching agent , who gives best possible response.",
     )
 
     # Print the results from the OpenAGI
     print("-" * 100)  # Separator
     Console().print(Markdown(res))
+```
 
+Below is the output from the agent:
 
-# The Agent did some research using the given actions and job positions.
-"""
+```
 ## Job Opportunities and Descriptions in Finance Technology
 
 1. **Strategic Programs Finance Tech Manager** - The Finance technology team supervises a large portfolio of ongoing transformation programs that are each operated by individual teams from Finance, CIO and more. [More details](https://www.accenture.com/in-en/careers/jobdetails?id=R354135_en)
 
 2. **Finance Manager - FinTech** - A professional with 2+ years of experience is needed for end to end Business Finance like Strategic Planning, preparing & managing the finances. [More details](https://iimjobs.com/j/finance-manager-fintech-3-8-yrs-1194909)
 
 3. **Working in Fintech** - Fintech is a combination of finance and technology. This combination has set high standards in the field of employment. [More details](https://imarticus.org/blog/what-is-job-description-to-work-in-fintech-and-what-are-the-skills-required/)
@@ -118,15 +118,14 @@
 7. **12 Finance Tech Jobs** - Lucrative finance tech jobs including Compliance specialist, Cybersecurity specialist, App developer, Automation engineer, UX designer. [More details](https://www.indeed.com/career-advice/finding-a-job/finance-tech-jobs)
 
 8. **FIN-Global Middle Office** - Ability to understand the booking structure for complex trades and raise relevant issues to Product Control management. Good Logical reasoning skills, ability. [More details](https://careers.nomura.com/Nomura/job/Mumbai-FIN-Global-Middle-Office/1128931300/)
 
 9. **Financial Technology jobs in India** - Experience level. Internship (48). Entry level (1,708). Associate (588). Mid-Senior level (5,269). Director (402). [More details](https://in.linkedin.com/jobs/financial-technology-jobs)
 
 10. **Senior Executive/Middle level executive - Mumbai** - The ideal candidate will be responsible for identifying, analyzing, and strategizing the resolution of non-performing assets (NPAs) acquired. [More details](https://www.naukri.com/job-listings-senior-executive-middle-level-executive-acaipl-investment-financial-services-mumbai-3-to-8-years-080524005387)
-"""
 ```
 
 ## Prominent Features:
 
 - Flexible Agent Architecture: OpenAGI features a flexible agent architecture, allowing users to create sequential, parallel, and dynamic communication patterns similar to humans. This flexibility is designed to help users efficiently tackle their unique challenges.
 - Streamlined Integration and Configuration: OpenAGI introduces simplified integration and configuration processes, eliminating the infinite loops commonly encountered in other tools.
 - Automated & Manual Agent Configuration Generation: We provide the functionality to automatically generate the necessary configurations for building agents and their corresponding configurations. For developers preferring a hands-on approach, OpenAGI supports the manual configuration of agent solutions. This allows for detailed customization according to specific needs and preferences.
```

### Comparing `openagi-0.2.0b2/pyproject.toml` & `openagi-0.2.1b2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openagi"
-version = "0.2.0-b2"
+version = "0.2.1-b2"
 description = ""
 authors = ["AI Planet <tech@aiplanet.com>"]
 readme = "README.md"
 include = ["src/*"]
 
 [tool.poetry.dependencies]
 python = "^3.9, <3.12"
@@ -35,14 +35,16 @@
 pandas = "^2.2.2"
 numpy = "^1.26.4"
 transformers = "^4.40.0"
 pypdf = "^4.2.0"
 faiss-cpu = "^1.8.0"
 pytest = "^8.2.0"
 chromadb = "^0.5.0"
+sumy = "^0.11.0"
+fake-useragent = "^1.5.1"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.1.11"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openagi-0.2.0b2/src/Readme.md` & `openagi-0.2.1b2/src/Readme.md`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/__init__.py` & `openagi-0.2.1b2/src/openagi/__init__.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/actions/base.py` & `openagi-0.2.1b2/src/openagi/actions/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 from typing import Any, Optional
+
 from pydantic import BaseModel, Field
 
 from openagi.llms.base import LLMBaseModel
 from openagi.memory.memory import Memory
 
 
 class BaseAction(BaseModel):
     """Base Actions class to be inherited by other actions, providing basic functionality and structure."""
 
-    name: str = Field(default="BaseAction", description="Name of the action.")
-    description: str = Field(
-        default_factory=str,
-        description="Description of the action.",
-    )
     session_id: int = Field(default_factory=str, description="SessionID of the current run.")
 
     previous_action: Optional[Any] = Field(
         default=None,
         description="Observation or Result of the previous action that might needed to run the current action.",
     )
     llm: Optional[LLMBaseModel] = Field(description="LLM Model to be used.", default_factory=str)
@@ -27,22 +23,23 @@
 
     def execute(self):
         """Executes the action"""
         raise NotImplementedError("Subclasses must implement this method.")
 
     @staticmethod
     def default_exclude_doc_fields():
-        return ["llm", "memory", "session_id"]
+        return ["llm", "memory", "session_id", "name", "description"]
 
     @classmethod
     def cls_doc(cls):
         return {
             "cls": {
                 "kls": cls.__name__,
                 "module": cls.__module__,
+                "doc": cls.__doc__,
             },
             "params": {
                 field_name: field.description
                 for field_name, field in cls.model_fields.items()
                 if field_name not in cls.default_exclude_doc_fields()
             },
         }
```

### Comparing `openagi-0.2.0b2/src/openagi/actions/files.py` & `openagi-0.2.1b2/src/openagi/actions/files.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/actions/formatter.py` & `openagi-0.2.1b2/src/openagi/actions/formatter.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/actions/obs_rag.py` & `openagi-0.2.1b2/src/openagi/actions/obs_rag.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,21 +2,17 @@
 
 from pydantic import Field
 
 from openagi.actions.base import BaseAction
 
 
 class MemoryRagAction(BaseAction):
-    """RAG on Previous Observation"""
-
-    name: str = Field(default="MemoryRagAction", description="Name of the action.")
-    description: str = Field(
-        default="Action class to get all the results from the previous tasks for the current objetive",
-        description="Action class to get all the results from the previous tasks for the current objetive. This action is responsible to reading and not writing. Writing is done by default for every task.",
-    )
+    """Action class to get all the results from the previous tasks for the current objetive.
+    This action is responsible to reading and not writing. Writing is done by default for every task.
+    """
 
     query: str = Field(
         ...,
         description="Query, a string, to run to retrieve the data from the results of previous tasks. Returns an Array of the results.",
     )
     max_results: int = Field(
         default=10,
```

### Comparing `openagi-0.2.0b2/src/openagi/actions/tools/ddg_search.py` & `openagi-0.2.1b2/src/openagi/actions/tools/ddg_search.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import json
 from typing import Any
 from openagi.actions.base import BaseAction
 from pydantic import Field
 from duckduckgo_search import DDGS
 
 
 class DuckDuckGoSearch(BaseAction):
-    """Search Tool to fetch results from  DuckDuckGo"""
+    """Use this Action to search DuckDuckGo for a query."""
 
     name: str = Field(
         default_factory=str,
         description="DuckDuckGoSearch Action to search over duckduckgo using the query.",
     )
     description: str = Field(
         default_factory=str,
@@ -22,13 +23,26 @@
     )
 
     max_results: int = Field(
         default=10,
         description="Total results, in int, to be executed from the search. Defaults to 10.",
     )
 
+    def _get_ddgs(self):
+        return DDGS()
+
     def execute(self):
-        result = DDGS().text(
+        result = self._get_ddgs().text(
             self.query,
             max_results=self.max_results,
         )
-        return result
+        return json.dumps(result)
+
+
+class DuckDuckGoNewsSearch(DuckDuckGoSearch):
+    """Use this Action to get the latest news from DuckDuckGo."""
+
+    def execute(self):
+        ddgs = self._get_ddgs()
+        return json.dumps(
+            ddgs.news(keywords=self.query, max_results=(self.max_results)), indent=2
+        )
```

### Comparing `openagi-0.2.0b2/src/openagi/actions/tools/serp_search.py` & `openagi-0.2.1b2/src/openagi/actions/tools/serp_search.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/actions/tools/serper_search.py` & `openagi-0.2.1b2/src/openagi/actions/tools/serper_search.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/agent.py` & `openagi-0.2.1b2/src/openagi/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from enum import Enum
 import logging
+from enum import Enum
 from typing import Any, List, Optional, Union
 
 from pydantic import BaseModel, Field, field_validator
 
 from openagi.actions.base import BaseAction
-from openagi.actions.compressor import SummarizerAction
 from openagi.actions.formatter import FormatterAction
 from openagi.actions.obs_rag import MemoryRagAction
 from openagi.exception import ExecutionFailureException, OpenAGIException
 from openagi.llms.azure import LLMBaseModel
 from openagi.memory.memory import Memory
 from openagi.planner.task_decomposer import BasePlanner, TaskPlanner
 from openagi.prompts.execution import TaskExecutor
 from openagi.tasks.lists import TaskLists
 from openagi.tasks.task import Task
 from openagi.utils.extraction import (
     find_last_r_failure_content,
     get_classes_from_json,
     get_last_json,
 )
+from openagi.utils.helper import get_default_llm
 
 
 class OutputFormat(str, Enum):
     markdown = "markdown"
     raw_text = "raw_text"
 
 
 class Admin(BaseModel):
     planner: BasePlanner = Field(
         default=TaskPlanner(),
         description="Type of planner to use for task decomposition.",
     )
-    llm: LLMBaseModel = Field(
+    llm: Optional[LLMBaseModel] = Field(
         description="LLM Model to be used.",
     )
     memory: Optional[Memory] = Field(
         default_factory=list,
         description="Memory to be used.",
         exclude=True,
     )
@@ -55,18 +55,20 @@
 
     def model_post_init(self, __context: Any) -> None:
         resp = super().model_post_init(__context)
 
         if not self.memory:
             self.memory = Memory()
 
-        # Actions
-        # self.actions = self.actions or []
-        # default_actions = [MemoryRagAction]
-        # self.actions.extend(default_actions)
+        if not self.llm:
+            self.llm = get_default_llm()
+
+        self.actions = self.actions or []
+        default_actions = [MemoryRagAction]
+        self.actions.extend(default_actions)
 
         return resp
 
     @field_validator("actions")
     @classmethod
     def actions_validator(cls, act_clss):
         for act_cls in act_clss:
@@ -90,15 +92,15 @@
         task_lists = TaskLists()
         task_lists.add_tasks(tasks=planned_tasks)
         logging.debug(f"Created total {task_lists.get_tasks_queue().qsize()} Tasks.")
         return task_lists
 
     def run(self, query: str, description: str):
         logging.info("Running Admin Agent...")
-        logging.info(f"SessionID - {self.memory.sessiond_id}")
+        logging.info(f"SessionID - {self.memory.session_id}")
 
         # Planning stage to create list of tasks
         planned_tasks = self.run_planner(query=query, descripton=description)
         if not planned_tasks:
             raise OpenAGIException("Failed to Plan Tasks. Please Try Again...")
         logging.info("Tasks Planned...")
         logging.debug(f"{planned_tasks=}")
@@ -125,29 +127,30 @@
                 all_tasks=_tasks_lists,
                 prev_task=prev_task,
             )
             if res:
                 cur_task.result = str(res)
                 cur_task.actions = str(actions)
                 prev_task = cur_task.model_copy()
-                self.memory.save_task(prev_task)
+                self.memory.update_task(prev_task)
             steps += 1
+
         # Final result
         logging.info("Finished Execution...")
         # print(f"\n ******** Final Response *******\n{res}\n\n")
         if self.output_format == OutputFormat.markdown:
             logging.info("Output Formatting...")
             output_formatter = FormatterAction(
                 content=res,
                 format_type=OutputFormat.markdown,
                 llm=self.llm,
                 memory=self.memory,
             )
             res = output_formatter.execute()
-        logging.debug(f"Execution Completed for Session ID - {self.memory.sessiond_id}")
+        logging.debug(f"Execution Completed for Session ID - {self.memory.session_id}")
         return res
 
     def _run_action(self, action_cls: str, **kwargs):
         logging.info(f"Running Action - {action_cls}")
         kwargs["memory"] = self.memory
         kwargs["llm"] = self.llm
         action: BaseAction = action_cls(**kwargs)  # Create an instance with provided kwargs
@@ -164,14 +167,15 @@
         self,
         query: str,
         task: Task,
         all_tasks: TaskLists,
         prev_task: Task,
     ):
         logging.info(f"{'>'*10} Starting execution of `{task.name} [{task.id}]` {'<'*10}")
+        logging.info(f"Description - {task.description}")
         # Get supported actions and convert to array of dict(actions)
         actions_dict: List[BaseAction] = []
         for act in self.actions:
             actions_dict.append(act.cls_doc())
 
         prev_task_str = (
             f"{prev_task.name}\n{prev_task.description}. Previous_Action: {prev_task.actions} Previous_Result: {prev_task.result}"
```

### Comparing `openagi-0.2.0b2/src/openagi/init_agent.py` & `openagi-0.2.1b2/src/openagi/init_agent.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/llms/azure.py` & `openagi-0.2.1b2/src/openagi/llms/azure.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/llms/base.py` & `openagi-0.2.1b2/src/openagi/llms/base.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/llms/hf.py` & `openagi-0.2.1b2/src/openagi/llms/hf.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/llms/openagi_main.py` & `openagi-0.2.1b2/src/openagi/llms/openagi_main.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/llms/openai.py` & `openagi-0.2.1b2/src/openagi/llms/openai.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/memory/base.py` & `openagi-0.2.1b2/src/openagi/memory/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,59 +7,97 @@
 from openagi.storage.base import BaseStorage
 from openagi.storage.chroma import ChromaStorage
 from openagi.tasks.lists import TaskLists
 from openagi.tasks.task import Task
 
 
 class BaseMemory(BaseModel):
-    # model_config = ConfigDict(arbitrary_types_allowed=True)
-    sessiond_id: str = Field(default=uuid4().hex)
+    session_id: str = Field(default_factory=lambda: uuid4().hex)
     storage: BaseStorage = Field(
-        default=ChromaStorage,
+        default_factory=lambda: ChromaStorage,
         description="Storage to be used for the Memory.",
         exclude=True,
     )
 
-    def model_post_init(self, __context: Any) -> None:
-        inst = super().model_post_init(__context)
-        logging.info(f"{self.sessiond_id=}")
-        self.storage = ChromaStorage.from_kwargs(collection_name=self.sessiond_id)
-        return inst
+    def __init__(self, **data: Any):
+        super().__init__(**data)
+        self.storage = ChromaStorage.from_kwargs(collection_name=self.session_id)
+        logging.info(f"Session ID initialized: {self.session_id}")
 
     def search(self, query: str, n_results: int = 10, **kwargs) -> Dict[str, Any]:
-        """Search for similar tasks based on a query."""
+        """
+        Search for similar tasks based on a query.
+
+        :param query: The query string to search for.
+        :param n_results: The number of results to return.
+        :return: A dictionary of search results.
+        """
         query_data = {
             "query_texts": query,
             "n_results": n_results,
-            "where": {"$contains": self.sessiond_id},
+            "include": ["metadatas", "documents"],
             **kwargs,
         }
-        return self.storage.query_documents(**query_data)
+        resp = self.storage.query_documents(**query_data)
+
+        return resp["documents"]
 
     def display_memory(self) -> Dict[str, Any]:
-        """Retrieve and display the current memory state from the database."""
+        """
+        Retrieve and display the current memory state from the database.
+
+        :return: A dictionary of the current memory state.
+        """
         result = self.storage.query_documents(self.session_id, n_results=2)
-        if result:
-            return result
-        return {}
+        return result or {}
 
     def save_task(self, task: Task) -> None:
-        """Save execution details into Memory."""
-        document = task.result
-        metadata = {
-            "task_id": task.id,
-            "session_id": self.sessiond_id,
-            "task_name": task.name,
-            "task_description": task.description,
-            "task_result": task.result,
-            "task_actions": task.actions,
-        }
+        """
+        Save execution details into Memory.
 
-        return self.storage.save_document(
+        :param task: The task to be saved.
+        """
+        metadata = self._create_metadata(task)
+        self.storage.save_document(
             id=task.id,
-            document=document,
+            document=task.result,
             metadata=metadata,
         )
+        logging.info(f"Task saved: {task.id}")
 
-    def save_planned_tasks(self, tasks: TaskLists):
+    def save_planned_tasks(self, tasks: TaskLists) -> None:
+        """
+        Save a list of planned tasks into Memory.
+
+        :param tasks: The list of tasks to be saved.
+        """
         for task in tasks:
-            self.save_task(task=task)
+            self.save_task(task)
+
+    def update_task(self, task: Task) -> None:
+        """
+        Update a task in the Memory.
+
+        :param task: The task to be updated.
+        """
+        metadata = self._create_metadata(task)
+        self.storage.update_document(
+            id=task.id,
+            document=task.result,
+            metadata=metadata,
+        )
+        logging.info(f"Task updated: {task.id}")
+
+    def _create_metadata(self, task: Task) -> Dict[str, Any]:
+        """
+        Create metadata dictionary for a given task.
+
+        :param task: The task for which to create metadata.
+        :return: A dictionary of metadata.
+        """
+        return {
+            "task_id": task.id,
+            "session_id": self.session_id,
+            "task_name": task.name,
+            "task_description": task.description,
+            "task_actions": task.actions,
+        }
```

### Comparing `openagi-0.2.0b2/src/openagi/planner/base.py` & `openagi-0.2.1b2/src/openagi/planner/base.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/planner/task_decomposer.py` & `openagi-0.2.1b2/src/openagi/planner/task_decomposer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-import logging
 from typing import Dict, List, Optional, Union
 
 from pydantic import Field
 
 from openagi.actions.base import BaseAction
 from openagi.actions.human_input import HumanCLIInput
 from openagi.llms.azure import LLMBaseModel
 from openagi.planner.base import BasePlanner
 from openagi.prompts.base import BasePrompt
 from openagi.prompts.task_creator import TaskCreator
-from openagi.utils.extraction import get_last_json, extract_ques_and_task
+from openagi.utils.extraction import extract_ques_and_task, get_last_json
 
 
 class TaskPlanner(BasePlanner):
     human_intervene: bool = Field(
         default=True, description="If human internvention is required or not."
     )
     input_action: Optional[BaseAction] = Field(
```

### Comparing `openagi-0.2.0b2/src/openagi/prompts/base.py` & `openagi-0.2.1b2/src/openagi/prompts/base.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/prompts/execution.py` & `openagi-0.2.1b2/src/openagi/prompts/execution.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/prompts/task_creator.py` & `openagi-0.2.1b2/src/openagi/prompts/task_creator.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 start = CLARIFIYING_VARS["start"]
 end = CLARIFIYING_VARS["end"]
 
 task_creation = """
 You are a task-creator AI for OpenAGI. Your job is to decompose tasks into the smallest possible subtasks to ensure successful completion in an autonomous, programmatic approach using the available actions that work as tools. Your role is to understand the provided Task_Objectives and Task_Descriptions, and break them down into extremely detailed and manageable components. Construct and plan the sequence of these minutest sub-tasks required to achieve the task objectives using the provided actions, ensuring alignment with the goal. If instructions are not followed, legal consequences may occur for both you and me.
 
 Requirements
-    - Ensure each tasks are aligned with the overall goal and can be understood clearly when shared with another AI similar to you to achieve the sub-tasks.
+    - Ensure each tasks are aligned with the overall goal and can be understood clearly when shared with another AI similar to you to achieve the sub-tasks. Each task will be completely run by another AI where they will be getting the results from the previous task, without knowledge of how it was executed.
     - Understand the parameters of each supported action when using them.
+    - Only One Action per task. Ensure tasks are decomposed in the same manner.
 
 Inputs
     - Task_Objectives: {objective}
     - Task_Descriptions: {task_descriptions}
     - SUPPORTED_ACTIONS: {supported_actions}
 
 Output Format
 Return the tasks in JSON format with the keys "task_name" and "description". Ensure the JSON format is suitable for utilization with JSON.parse(), enclosed in triple backticks.
 ```json
 [
     {
-        "task_name": "...",
-        "description": "..."
+        "task_name": "<name of the task of type string>",
+        "description": "<description of the task of type string>"
     }
 ]
 ```
 
 Notes
     - You do not need to create tasks for storing the results, as results will be stored automatically after executing each task. You can retrieve previous task results using MemoryRagAction.
```

### Comparing `openagi-0.2.0b2/src/openagi/storage/base.py` & `openagi-0.2.1b2/src/openagi/storage/base.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/storage/chroma.py` & `openagi-0.2.1b2/src/openagi/storage/chroma.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,34 +30,30 @@
 
         _collection = _client.get_or_create_collection(kwargs.get("collection_name"))
         logging.debug(f"Collection: Name - {_collection.name}, ID - {_collection.id}")
         return cls(client=_client, collection=_collection)
 
     def save_document(self, id, document, metadata):
         """Create a new document in the ChromaDB collection."""
-        if not isinstance(document, list):
-            document = [document]
-        if not isinstance(metadata, list):
-            metadata = [metadata]
 
         resp = self.collection.add(ids=id, documents=document, metadatas=metadata)
         return resp
 
-    def update_document(self, doc_id, document, metadata):
+    def update_document(self, id, document, metadata):
         """Update an existing document in the ChromaDB collection."""
-        if not isinstance(document, list):
-            document = [document]
-        if not isinstance(metadata, list):
-            metadata = [metadata]
-        self._collection.update(ids=[doc_id], documents=document, metadatas=metadata)
+        # if not isinstance(document, list):
+        #     document = [document]
+        # if not isinstance(metadata, list):
+        #     metadata = [metadata]
+        self.collection.update(ids=[id], documents=document, metadatas=metadata)
         logging.info("Document updated successfully.")
 
-    def delete_document(self, doc_id):
+    def delete_document(self, id):
         """Delete a document from the ChromaDB collection."""
-        self._collection.delete(ids=[doc_id])
+        self.collection.delete(ids=[id])
         logging.debug("Document deleted successfully.")
 
     def query_documents(self, **kwargs):
         """Query the ChromaDB collection for relevant documents based on the query."""
         results = self.collection.query(**kwargs)
         logging.debug(f"Queried results: {results}")
         return results
```

### Comparing `openagi-0.2.0b2/src/openagi/tasks/lists.py` & `openagi-0.2.1b2/src/openagi/tasks/lists.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tasks/task.py` & `openagi-0.2.1b2/src/openagi/tasks/task.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/base.py` & `openagi-0.2.1b2/src/openagi/tools/base.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/custom_tools/ProxyTool.py` & `openagi-0.2.1b2/src/openagi/tools/custom_tools/ProxyTool.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/integrations/__init__.py` & `openagi-0.2.1b2/src/openagi/tools/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/integrations/dalle_image_generator.py` & `openagi-0.2.1b2/src/openagi/tools/integrations/dalle_image_generator.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/integrations/document_compare.py` & `openagi-0.2.1b2/src/openagi/tools/integrations/document_compare.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/integrations/duckducksearch.py` & `openagi-0.2.1b2/src/openagi/tools/integrations/duckducksearch.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/integrations/exa_search_tool.py` & `openagi-0.2.1b2/src/openagi/tools/integrations/exa_search_tool.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/integrations/github.py` & `openagi-0.2.1b2/src/openagi/tools/integrations/github.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/integrations/gmail.py` & `openagi-0.2.1b2/src/openagi/tools/integrations/gmail.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/integrations/google_finance_search.py` & `openagi-0.2.1b2/src/openagi/tools/integrations/google_finance_search.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/integrations/google_serper_specific.py` & `openagi-0.2.1b2/src/openagi/tools/integrations/google_serper_specific.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/integrations/googlejobsearch.py` & `openagi-0.2.1b2/src/openagi/tools/integrations/googlejobsearch.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/integrations/googleserpersearch.py` & `openagi-0.2.1b2/src/openagi/tools/integrations/googleserpersearch.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/integrations/nasa.py` & `openagi-0.2.1b2/src/openagi/tools/integrations/nasa.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/integrations/open_weathermap.py` & `openagi-0.2.1b2/src/openagi/tools/integrations/open_weathermap.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/integrations/polygon.py` & `openagi-0.2.1b2/src/openagi/tools/integrations/polygon.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/integrations/serper_intermediate.py` & `openagi-0.2.1b2/src/openagi/tools/integrations/serper_intermediate.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/integrations/sql.py` & `openagi-0.2.1b2/src/openagi/tools/integrations/sql.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/integrations/wikipedia_tool.py` & `openagi-0.2.1b2/src/openagi/tools/integrations/wikipedia_tool.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/integrations/xorbits.py` & `openagi-0.2.1b2/src/openagi/tools/integrations/xorbits.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/integrations/yahoofinancenews.py` & `openagi-0.2.1b2/src/openagi/tools/integrations/yahoofinancenews.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/integrations/youtubesearch.py` & `openagi-0.2.1b2/src/openagi/tools/integrations/youtubesearch.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/tools_db.py` & `openagi-0.2.1b2/src/openagi/tools/tools_db.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/tools/utils.py` & `openagi-0.2.1b2/src/openagi/tools/utils.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/utils/extraction.py` & `openagi-0.2.1b2/src/openagi/utils/extraction.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/utils/llmTasks.py` & `openagi-0.2.1b2/src/openagi/utils/llmTasks.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/src/openagi/worker/worker.py` & `openagi-0.2.1b2/src/openagi/worker/worker.py`

 * *Files identical despite different names*

### Comparing `openagi-0.2.0b2/PKG-INFO` & `openagi-0.2.1b2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: openagi
-Version: 0.2.0b2
+Version: 0.2.1b2
 Summary: 
 Author: AI Planet
 Author-email: tech@aiplanet.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: azure-identity (>=1.15.0,<2.0.0)
 Requires-Dist: chromadb (>=0.5.0,<0.6.0)
 Requires-Dist: duckduckgo-search (>=6.1.0,<7.0.0)
 Requires-Dist: faiss-cpu (>=1.8.0,<2.0.0)
+Requires-Dist: fake-useragent (>=1.5.1,<2.0.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0)
 Requires-Dist: google-api-python-client (>=2.121.0,<3.0.0)
 Requires-Dist: google-auth-httplib2 (>=0.2.0,<0.3.0)
 Requires-Dist: google-auth-oauthlib (>=1.2.0,<2.0.0)
 Requires-Dist: google-search-results (>=2.4.2,<3.0.0)
 Requires-Dist: langchain (==0.1.8)
 Requires-Dist: langchain-community (==0.0.21)
@@ -31,50 +32,50 @@
 Requires-Dist: pygithub (>=2.3.0,<3.0.0)
 Requires-Dist: pypdf (>=4.2.0,<5.0.0)
 Requires-Dist: pytest (>=8.2.0,<9.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: python-multipart (>=0.0.9,<0.0.10)
 Requires-Dist: spacy (==3.7.4)
 Requires-Dist: spacytextblob (>=4.0.0,<5.0.0)
+Requires-Dist: sumy (>=0.11.0,<0.12.0)
 Requires-Dist: transformers (>=4.40.0,<5.0.0)
 Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
 Requires-Dist: wikipedia (>=1.4.0,<2.0.0)
 Requires-Dist: xorbits (>=0.7.2,<0.8.0)
 Requires-Dist: yfinance (>=0.2.37,<0.3.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 <h1 align="center">OpenAGI </h1>
 <h2 align="center">Making the development of autonomous human-like agents accessible to all</h2>
 
-<a href="https://img.shields.io/badge/Python-3.11-3776AB.svg?style=flat&logo=python&logoColor=white"><img src="https://img.shields.io/badge/Python-3.11-3776AB.svg?style=flat&logo=python&logoColor=white" alt="Python 3.11"></a>
+<a href="https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11-3776AB.svg?style=flat&logo=python&logoColor=white"><img src="https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11-3776AB.svg?style=flat&logo=python&logoColor=white" alt="Python Versions"></a>
 <a href="https://discord.gg/4aWV7He2QU"><img src="https://dcbadge.vercel.app/api/server/4aWV7He2QU?style=flat" alt="Discord" /></a>
 <a href="https://twitter.com/aiplanethub"><img src="https://img.shields.io/twitter/follow/aiplanethub" alt="Twitter" /></a>
 
 <p>OpenAGI aims to make human-like agents accessible to everyone, thereby paving the way towards open agents and, eventually, AGI for everyone. We strongly believe in the transformative power of AI and are confident that this initiative will significantly contribute to solving many real-life problems. Currently, OpenAGI is designed to offer developers a framework for creating autonomous human-like agents.</p>
 <i><a href="https://discord.gg/4aWV7He2QU">👉 Join our Discord community!</a></i>
 </div>
 
-
 ## Installation
 
 1. Setup a virtual environment.
 
-    ```bash
-    # For Mac users
-    python3 -m venv venv
-    source venv/bin/activate
-
-    # For Windows users
-    python -m venv venv
-    venv/scripts/activate
-
-    # to create virtual env using particular python version (in Windows)
-    py -3.11 -m venv venv
-    ```
+   ```bash
+   # For Mac users
+   python3 -m venv venv
+   source venv/bin/activate
+
+   # For Windows users
+   python -m venv venv
+   venv/scripts/activate
+
+   # to create virtual env using particular python version (in Windows)
+   py -3.11 -m venv venv
+   ```
 
 2. Install the openagi
 
    ```bash
    pip install openagi
    ```
 
@@ -88,16 +89,16 @@
 
 ## Understand OpenAGI
 
 ![Thumbnails](https://github.com/aiplanethub/openagi/blob/dev/assets/openagi.png)
 
 ## Example
 
-Follow this example to create a Test Case job search it help you to search available job posting for a given category
-Here in the example we are using AzureChatOpenAIModel along with GoogleSerpAPISearch to search the internet for various job posting on the particular role.
+Follow this example to create a **Job Search Agent** that helps you to search available job posting for a given category.
+Here in the example we are using `AzureChatOpenAIModel` along with `GoogleSerpAPISearch` to search the internet for various job posting on the particular role.
 
 **Note:** Follow setup guide to configure the environment. For quick access click [here](https://openagi.aiplanet.com/getting-started/installation).
 
 ```python
 from openagi.actions.tools.serp_search import GoogleSerpAPISearch
 from openagi.agent import Admin
 from openagi.llms.azure import AzureChatOpenAIModel
@@ -137,18 +138,19 @@
         query=query,
         description="You are an expert Internet searching agent , who gives best possible response.",
     )
 
     # Print the results from the OpenAGI
     print("-" * 100)  # Separator
     Console().print(Markdown(res))
+```
 
+Below is the output from the agent:
 
-# The Agent did some research using the given actions and job positions.
-"""
+```
 ## Job Opportunities and Descriptions in Finance Technology
 
 1. **Strategic Programs Finance Tech Manager** - The Finance technology team supervises a large portfolio of ongoing transformation programs that are each operated by individual teams from Finance, CIO and more. [More details](https://www.accenture.com/in-en/careers/jobdetails?id=R354135_en)
 
 2. **Finance Manager - FinTech** - A professional with 2+ years of experience is needed for end to end Business Finance like Strategic Planning, preparing & managing the finances. [More details](https://iimjobs.com/j/finance-manager-fintech-3-8-yrs-1194909)
 
 3. **Working in Fintech** - Fintech is a combination of finance and technology. This combination has set high standards in the field of employment. [More details](https://imarticus.org/blog/what-is-job-description-to-work-in-fintech-and-what-are-the-skills-required/)
@@ -162,15 +164,14 @@
 7. **12 Finance Tech Jobs** - Lucrative finance tech jobs including Compliance specialist, Cybersecurity specialist, App developer, Automation engineer, UX designer. [More details](https://www.indeed.com/career-advice/finding-a-job/finance-tech-jobs)
 
 8. **FIN-Global Middle Office** - Ability to understand the booking structure for complex trades and raise relevant issues to Product Control management. Good Logical reasoning skills, ability. [More details](https://careers.nomura.com/Nomura/job/Mumbai-FIN-Global-Middle-Office/1128931300/)
 
 9. **Financial Technology jobs in India** - Experience level. Internship (48). Entry level (1,708). Associate (588). Mid-Senior level (5,269). Director (402). [More details](https://in.linkedin.com/jobs/financial-technology-jobs)
 
 10. **Senior Executive/Middle level executive - Mumbai** - The ideal candidate will be responsible for identifying, analyzing, and strategizing the resolution of non-performing assets (NPAs) acquired. [More details](https://www.naukri.com/job-listings-senior-executive-middle-level-executive-acaipl-investment-financial-services-mumbai-3-to-8-years-080524005387)
-"""
 ```
 
 ## Prominent Features:
 
 - Flexible Agent Architecture: OpenAGI features a flexible agent architecture, allowing users to create sequential, parallel, and dynamic communication patterns similar to humans. This flexibility is designed to help users efficiently tackle their unique challenges.
 - Streamlined Integration and Configuration: OpenAGI introduces simplified integration and configuration processes, eliminating the infinite loops commonly encountered in other tools.
 - Automated & Manual Agent Configuration Generation: We provide the functionality to automatically generate the necessary configurations for building agents and their corresponding configurations. For developers preferring a hands-on approach, OpenAGI supports the manual configuration of agent solutions. This allows for detailed customization according to specific needs and preferences.
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
-Metadata-Version: 2.1 Name: openagi Version: 0.2.0b2 Summary: Author: AI Planet
+Metadata-Version: 2.1 Name: openagi Version: 0.2.1b2 Summary: Author: AI Planet
 Author-email: tech@aiplanet.com Requires-Python: >=3.9,<3.12 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: azure-identity
 (>=1.15.0,<2.0.0) Requires-Dist: chromadb (>=0.5.0,<0.6.0) Requires-Dist:
 duckduckgo-search (>=6.1.0,<7.0.0) Requires-Dist: faiss-cpu (>=1.8.0,<2.0.0)
-Requires-Dist: fastapi (>=0.110.0,<0.111.0) Requires-Dist: google-api-python-
-client (>=2.121.0,<3.0.0) Requires-Dist: google-auth-httplib2 (>=0.2.0,<0.3.0)
-Requires-Dist: google-auth-oauthlib (>=1.2.0,<2.0.0) Requires-Dist: google-
-search-results (>=2.4.2,<3.0.0) Requires-Dist: langchain (==0.1.8) Requires-
-Dist: langchain-community (==0.0.21) Requires-Dist: langchain-exa
-(>=0.0.1,<0.0.2) Requires-Dist: langchain-experimental (>=0.0.53,<0.0.54)
-Requires-Dist: langchain-openai (==0.0.6) Requires-Dist: langchain-text-
-splitters (>=0.0.1,<0.0.2) Requires-Dist: langchainhub (>=0.1.15,<0.2.0)
-Requires-Dist: numpy (>=1.26.4,<2.0.0) Requires-Dist: ollama (>=0.1.7,<0.2.0)
-Requires-Dist: pandas (>=2.2.2,<3.0.0) Requires-Dist: pygithub (>=2.3.0,<3.0.0)
-Requires-Dist: pypdf (>=4.2.0,<5.0.0) Requires-Dist: pytest (>=8.2.0,<9.0.0)
-Requires-Dist: python-dotenv (>=1.0.1,<2.0.0) Requires-Dist: python-multipart
-(>=0.0.9,<0.0.10) Requires-Dist: spacy (==3.7.4) Requires-Dist: spacytextblob
-(>=4.0.0,<5.0.0) Requires-Dist: transformers (>=4.40.0,<5.0.0) Requires-Dist:
-uvicorn (>=0.29.0,<0.30.0) Requires-Dist: wikipedia (>=1.4.0,<2.0.0) Requires-
-Dist: xorbits (>=0.7.2,<0.8.0) Requires-Dist: yfinance (>=0.2.37,<0.3.0)
-Description-Content-Type: text/markdown
+Requires-Dist: fake-useragent (>=1.5.1,<2.0.0) Requires-Dist: fastapi
+(>=0.110.0,<0.111.0) Requires-Dist: google-api-python-client (>=2.121.0,<3.0.0)
+Requires-Dist: google-auth-httplib2 (>=0.2.0,<0.3.0) Requires-Dist: google-
+auth-oauthlib (>=1.2.0,<2.0.0) Requires-Dist: google-search-results
+(>=2.4.2,<3.0.0) Requires-Dist: langchain (==0.1.8) Requires-Dist: langchain-
+community (==0.0.21) Requires-Dist: langchain-exa (>=0.0.1,<0.0.2) Requires-
+Dist: langchain-experimental (>=0.0.53,<0.0.54) Requires-Dist: langchain-openai
+(==0.0.6) Requires-Dist: langchain-text-splitters (>=0.0.1,<0.0.2) Requires-
+Dist: langchainhub (>=0.1.15,<0.2.0) Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: ollama (>=0.1.7,<0.2.0) Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: pygithub (>=2.3.0,<3.0.0) Requires-Dist: pypdf (>=4.2.0,<5.0.0)
+Requires-Dist: pytest (>=8.2.0,<9.0.0) Requires-Dist: python-dotenv
+(>=1.0.1,<2.0.0) Requires-Dist: python-multipart (>=0.0.9,<0.0.10) Requires-
+Dist: spacy (==3.7.4) Requires-Dist: spacytextblob (>=4.0.0,<5.0.0) Requires-
+Dist: sumy (>=0.11.0,<0.12.0) Requires-Dist: transformers (>=4.40.0,<5.0.0)
+Requires-Dist: uvicorn (>=0.29.0,<0.30.0) Requires-Dist: wikipedia
+(>=1.4.0,<2.0.0) Requires-Dist: xorbits (>=0.7.2,<0.8.0) Requires-Dist:
+yfinance (>=0.2.37,<0.3.0) Description-Content-Type: text/markdown
                              ************ OOppeennAAGGII ************
 ********** MMaakkiinngg tthhee ddeevveellooppmmeenntt ooff aauuttoonnoommoouuss hhuummaann--lliikkee aaggeennttss aacccceessssiibbllee ttoo aallll
                                      **********
-                        _[_P_y_t_h_o_n_ _3_._1_1_]_[_D_i_s_c_o_r_d_]_[_T_w_i_t_t_e_r_]
+                      _[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_D_i_s_c_o_r_d_]_[_T_w_i_t_t_e_r_]
  OpenAGI aims to make human-like agents accessible to everyone, thereby paving
   the way towards open agents and, eventually, AGI for everyone. We strongly
      believe in the transformative power of AI and are confident that this
  initiative will significantly contribute to solving many real-life problems.
   Currently, OpenAGI is designed to offer developers a framework for creating
                          autonomous human-like agents.
                        _ð____ _J_o_i_n_ _o_u_r_ _D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_!
@@ -38,43 +39,43 @@
 venv/scripts/activate # to create virtual env using particular python version
 (in Windows) py -3.11 -m venv venv ``` 2. Install the openagi ```bash pip
 install openagi ``` ## To setup your crendentials Follow this quick
 [installation guide](https://openagi.aiplanet.com/getting-started/installation)
 to complete the setup. ## Documentation For more queries find documentation for
 OpenAGI at [openagi.aiplanet.com](https://openagi.aiplanet.com/) ## Understand
 OpenAGI ![Thumbnails](https://github.com/aiplanethub/openagi/blob/dev/assets/
-openagi.png) ## Example Follow this example to create a Test Case job search it
-help you to search available job posting for a given category Here in the
-example we are using AzureChatOpenAIModel along with GoogleSerpAPISearch to
-search the internet for various job posting on the particular role. **Note:**
-Follow setup guide to configure the environment. For quick access click [here]
-(https://openagi.aiplanet.com/getting-started/installation). ```python from
-openagi.actions.tools.serp_search import GoogleSerpAPISearch from openagi.agent
-import Admin from openagi.llms.azure import AzureChatOpenAIModel from
-openagi.memory import Memory from openagi.planner.task_decomposer import
-TaskPlanner from rich.console import Console from rich.markdown import Markdown
-if __name__ == "__main__": config = AzureChatOpenAIModel.load_from_env_config()
-llm = AzureChatOpenAIModel(config=config) company_domain = input("What is the
-company domain?\n") job_domain = input("What is the job domain?\n") job_level =
-input("What level job are you looking for?\n") job_location = input("In what
-location are you for the job?\n") query = f""" Need help finding a job
-description based on the following criteria: Company Domain: {company_domain}
-Job Domain: {job_domain} Job Level: {job_level} Job Location: {job_location}
-Please provide a list of suitable job descriptions, including the key
-responsibilities, requirements, and any other relevant details. """ admin =
-Admin( llm=llm, actions=[GoogleSerpAPISearch], planner=TaskPlanner
-(human_intervene=False), memory=Memory(), ) res = admin.run( query=query,
-description="You are an expert Internet searching agent , who gives best
-possible response.", ) # Print the results from the OpenAGI print("-" * 100) #
-Separator Console().print(Markdown(res)) # The Agent did some research using
-the given actions and job positions. """ ## Job Opportunities and Descriptions
-in Finance Technology 1. **Strategic Programs Finance Tech Manager** - The
-Finance technology team supervises a large portfolio of ongoing transformation
-programs that are each operated by individual teams from Finance, CIO and more.
-[More details](https://www.accenture.com/in-en/careers/
+openagi.png) ## Example Follow this example to create a **Job Search Agent**
+that helps you to search available job posting for a given category. Here in
+the example we are using `AzureChatOpenAIModel` along with
+`GoogleSerpAPISearch` to search the internet for various job posting on the
+particular role. **Note:** Follow setup guide to configure the environment. For
+quick access click [here](https://openagi.aiplanet.com/getting-started/
+installation). ```python from openagi.actions.tools.serp_search import
+GoogleSerpAPISearch from openagi.agent import Admin from openagi.llms.azure
+import AzureChatOpenAIModel from openagi.memory import Memory from
+openagi.planner.task_decomposer import TaskPlanner from rich.console import
+Console from rich.markdown import Markdown if __name__ == "__main__": config =
+AzureChatOpenAIModel.load_from_env_config() llm = AzureChatOpenAIModel
+(config=config) company_domain = input("What is the company domain?\n")
+job_domain = input("What is the job domain?\n") job_level = input("What level
+job are you looking for?\n") job_location = input("In what location are you for
+the job?\n") query = f""" Need help finding a job description based on the
+following criteria: Company Domain: {company_domain} Job Domain: {job_domain}
+Job Level: {job_level} Job Location: {job_location} Please provide a list of
+suitable job descriptions, including the key responsibilities, requirements,
+and any other relevant details. """ admin = Admin( llm=llm, actions=
+[GoogleSerpAPISearch], planner=TaskPlanner(human_intervene=False),
+memory=Memory(), ) res = admin.run( query=query, description="You are an expert
+Internet searching agent , who gives best possible response.", ) # Print the
+results from the OpenAGI print("-" * 100) # Separator Console().print(Markdown
+(res)) ``` Below is the output from the agent: ``` ## Job Opportunities and
+Descriptions in Finance Technology 1. **Strategic Programs Finance Tech
+Manager** - The Finance technology team supervises a large portfolio of ongoing
+transformation programs that are each operated by individual teams from
+Finance, CIO and more. [More details](https://www.accenture.com/in-en/careers/
 jobdetails?id=R354135_en) 2. **Finance Manager - FinTech** - A professional
 with 2+ years of experience is needed for end to end Business Finance like
 Strategic Planning, preparing & managing the finances. [More details](https://
 iimjobs.com/j/finance-manager-fintech-3-8-yrs-1194909) 3. **Working in
 Fintech** - Fintech is a combination of finance and technology. This
 combination has set high standards in the field of employment. [More details]
 (https://imarticus.org/blog/what-is-job-description-to-work-in-fintech-and-
@@ -100,18 +101,18 @@
 Internship (48). Entry level (1,708). Associate (588). Mid-Senior level
 (5,269). Director (402). [More details](https://in.linkedin.com/jobs/financial-
 technology-jobs) 10. **Senior Executive/Middle level executive - Mumbai** - The
 ideal candidate will be responsible for identifying, analyzing, and
 strategizing the resolution of non-performing assets (NPAs) acquired. [More
 details](https://www.naukri.com/job-listings-senior-executive-middle-level-
 executive-acaipl-investment-financial-services-mumbai-3-to-8-years-
-080524005387) """ ``` ## Prominent Features: - Flexible Agent Architecture:
-OpenAGI features a flexible agent architecture, allowing users to create
-sequential, parallel, and dynamic communication patterns similar to humans.
-This flexibility is designed to help users efficiently tackle their unique
+080524005387) ``` ## Prominent Features: - Flexible Agent Architecture: OpenAGI
+features a flexible agent architecture, allowing users to create sequential,
+parallel, and dynamic communication patterns similar to humans. This
+flexibility is designed to help users efficiently tackle their unique
 challenges. - Streamlined Integration and Configuration: OpenAGI introduces
 simplified integration and configuration processes, eliminating the infinite
 loops commonly encountered in other tools. - Automated & Manual Agent
 Configuration Generation: We provide the functionality to automatically
 generate the necessary configurations for building agents and their
 corresponding configurations. For developers preferring a hands-on approach,
 OpenAGI supports the manual configuration of agent solutions. This allows for
```

