# Comparing `tmp/rag4p-0.3.0.tar.gz` & `tmp/rag4p-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rag4p-0.3.0.tar", max compression
+gzip compressed data, was "rag4p-0.4.0.tar", max compression
```

## Comparing `rag4p-0.3.0.tar` & `rag4p-0.4.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     3266 2024-05-11 10:54:33.026591 rag4p-0.3.0/README.md
--rw-r--r--   0        0        0      781 2024-05-20 08:16:12.868937 rag4p-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-17 15:16:40.886501 rag4p-0.3.0/rag4p/__init__.py
--rw-r--r--   0        0        0     3546 2024-05-11 10:19:26.281070 rag4p-0.3.0/rag4p/app_complete_local.py
--rw-r--r--   0        0        0     3224 2024-02-15 14:42:08.665322 rag4p-0.3.0/rag4p/app_complete_weaviate.py
--rw-r--r--   0        0        0     1154 2024-02-15 14:50:41.830101 rag4p-0.3.0/rag4p/app_generation_answer_generator.py
--rw-r--r--   0        0        0     1318 2024-05-11 10:19:26.290206 rag4p-0.3.0/rag4p/app_generation_answer_quality.py
--rw-r--r--   0        0        0     1292 2024-05-11 10:24:23.583279 rag4p-0.3.0/rag4p/app_generation_answer_quality_ollama.py
--rw-r--r--   0        0        0     2708 2024-02-15 15:49:18.900194 rag4p-0.3.0/rag4p/app_generation_question_generator.py
--rw-r--r--   0        0        0     1432 2024-02-15 15:31:45.716697 rag4p-0.3.0/rag4p/app_generation_questions_generator_vasa.py
--rw-r--r--   0        0        0     1214 2024-02-15 15:59:09.706810 rag4p-0.3.0/rag4p/app_indexing_local.py
--rw-r--r--   0        0        0     2330 2024-03-11 09:33:23.161900 rag4p-0.3.0/rag4p/app_indexing_weaviate.py
--rw-r--r--   0        0        0     1254 2024-02-15 15:31:45.728308 rag4p-0.3.0/rag4p/app_retrieval_quality_vasa.py
--rw-r--r--   0        0        0     1514 2024-05-15 14:45:34.878603 rag4p-0.3.0/rag4p/app_retrieval_retriever_local.py
--rw-r--r--   0        0        0     1691 2024-02-15 16:00:53.497383 rag4p-0.3.0/rag4p/app_retrieval_retriever_weaviate.py
--rw-r--r--   0        0        0     1878 2024-02-15 15:31:45.712149 rag4p-0.3.0/rag4p/app_retrieval_strategy.py
--rw-r--r--   0        0        0      429 2024-01-31 07:51:24.674544 rag4p-0.3.0/rag4p/app_weaviate_info.py
--rw-r--r--   0        0        0        0 2024-01-17 15:16:40.886501 rag4p-0.3.0/rag4p/indexing/__init__.py
--rw-r--r--   0        0        0      117 2024-01-18 16:12:32.211578 rag4p-0.3.0/rag4p/indexing/content_reader.py
--rw-r--r--   0        0        0      675 2024-02-15 14:54:08.869449 rag4p-0.3.0/rag4p/indexing/indexing_service.py
--rw-r--r--   0        0        0      232 2024-01-17 15:25:27.590307 rag4p-0.3.0/rag4p/indexing/input_document.py
--rw-r--r--   0        0        0      285 2024-02-13 20:32:37.812960 rag4p-0.3.0/rag4p/indexing/splitter.py
--rw-r--r--   0        0        0        0 2024-02-13 19:57:32.062188 rag4p-0.3.0/rag4p/indexing/splitters/__init__.py
--rw-r--r--   0        0        0     1356 2024-02-13 20:28:11.172941 rag4p-0.3.0/rag4p/indexing/splitters/max_token_splitter.py
--rw-r--r--   0        0        0      671 2024-02-13 20:32:37.826115 rag4p-0.3.0/rag4p/indexing/splitters/sentence_splitter.py
--rw-r--r--   0        0        0      474 2024-02-13 20:32:37.822569 rag4p-0.3.0/rag4p/indexing/splitters/single_chunk_splitter.py
--rw-r--r--   0        0        0        0 2024-02-13 20:16:16.212988 rag4p-0.3.0/rag4p/integrations/__init__.py
--rw-r--r--   0        0        0      204 2024-05-10 14:28:00.181901 rag4p-0.3.0/rag4p/integrations/ollama/__init__.py
--rw-r--r--   0        0        0     2361 2024-05-10 15:59:57.265154 rag4p-0.3.0/rag4p/integrations/ollama/access_ollama.py
--rw-r--r--   0        0        0      808 2024-05-13 07:17:37.558316 rag4p-0.3.0/rag4p/integrations/ollama/ollama_answer_generator.py
--rw-r--r--   0        0        0      547 2024-05-10 14:37:39.142352 rag4p-0.3.0/rag4p/integrations/ollama/ollama_embedder.py
--rw-r--r--   0        0        0     1456 2024-05-13 07:17:37.553472 rag4p-0.3.0/rag4p/integrations/ollama/ollama_question_generator.py
--rw-r--r--   0        0        0        0 2024-05-11 10:09:25.775349 rag4p-0.3.0/rag4p/integrations/ollama/quality/__init__.py
--rw-r--r--   0        0        0     1429 2024-05-11 10:36:04.986424 rag4p-0.3.0/rag4p/integrations/ollama/quality/ollama_answer_quality_service.py
--rw-r--r--   0        0        0      429 2024-05-11 10:04:59.548674 rag4p-0.3.0/rag4p/integrations/openai/__init__.py
--rw-r--r--   0        0        0     1311 2024-05-11 09:33:48.693626 rag4p-0.3.0/rag4p/integrations/openai/openai_answer_generator.py
--rw-r--r--   0        0        0      943 2024-02-13 21:03:08.370679 rag4p-0.3.0/rag4p/integrations/openai/openai_embedder.py
--rw-r--r--   0        0        0     1709 2024-02-13 21:03:08.339951 rag4p-0.3.0/rag4p/integrations/openai/openai_question_generator.py
--rw-r--r--   0        0        0        0 2024-05-11 09:39:07.588936 rag4p-0.3.0/rag4p/integrations/openai/quality/__init__.py
--rw-r--r--   0        0        0     1828 2024-05-11 10:32:57.682591 rag4p-0.3.0/rag4p/integrations/openai/quality/openai_answer_quality_service.py
--rw-r--r--   0        0        0       26 2024-03-11 09:33:23.149502 rag4p-0.3.0/rag4p/integrations/weaviate/__init__.py
--rw-r--r--   0        0        0     2930 2024-03-11 09:33:23.144857 rag4p-0.3.0/rag4p/integrations/weaviate/access_weaviate.py
--rw-r--r--   0        0        0     1001 2024-02-06 22:07:59.527805 rag4p-0.3.0/rag4p/integrations/weaviate/chunk_collection.py
--rw-r--r--   0        0        0     1190 2024-03-11 09:33:23.157565 rag4p-0.3.0/rag4p/integrations/weaviate/weaviate_content_store.py
--rw-r--r--   0        0        0     4505 2024-03-11 09:36:16.461784 rag4p-0.3.0/rag4p/integrations/weaviate/weaviate_retriever.py
--rw-r--r--   0        0        0        0 2024-02-13 20:01:14.586737 rag4p-0.3.0/rag4p/rag/__init__.py
--rw-r--r--   0        0        0        0 2024-02-13 20:01:31.907902 rag4p-0.3.0/rag4p/rag/embedding/__init__.py
--rw-r--r--   0        0        0      190 2024-02-13 22:23:33.027284 rag4p-0.3.0/rag4p/rag/embedding/embedder.py
--rw-r--r--   0        0        0        0 2024-02-13 20:01:59.778652 rag4p-0.3.0/rag4p/rag/embedding/local/__init__.py
--rw-r--r--   0        0        0     1426 2024-02-13 22:23:33.033084 rag4p-0.3.0/rag4p/rag/embedding/local/onnx_embedder.py
--rw-r--r--   0        0        0        0 2024-02-13 20:03:17.496572 rag4p-0.3.0/rag4p/rag/generation/__init__.py
--rw-r--r--   0        0        0      262 2024-02-13 22:23:33.009410 rag4p-0.3.0/rag4p/rag/generation/answer_generator.py
--rw-r--r--   0        0        0        0 2024-02-13 22:24:49.086889 rag4p-0.3.0/rag4p/rag/generation/chat/__init__.py
--rw-r--r--   0        0        0      875 2024-02-13 22:46:03.836482 rag4p-0.3.0/rag4p/rag/generation/chat/chat_prompt.py
--rw-r--r--   0        0        0      592 2024-02-15 14:06:38.894059 rag4p-0.3.0/rag4p/rag/generation/observed_answer_generator.py
--rw-r--r--   0        0        0        0 2024-02-13 20:08:51.049910 rag4p-0.3.0/rag4p/rag/generation/quality/__init__.py
--rw-r--r--   0        0        0      178 2024-01-21 10:12:21.187448 rag4p-0.3.0/rag4p/rag/generation/quality/answer_from_context_quality.py
--rw-r--r--   0        0        0      532 2024-02-13 22:23:33.021369 rag4p-0.3.0/rag4p/rag/generation/quality/answer_quality.py
--rw-r--r--   0        0        0     4371 2024-05-18 10:20:51.530679 rag4p-0.3.0/rag4p/rag/generation/quality/answer_quality_service.py
--rw-r--r--   0        0        0      418 2024-01-21 09:11:19.307021 rag4p-0.3.0/rag4p/rag/generation/quality/answer_to_question_quality.py
--rw-r--r--   0        0        0      155 2024-01-28 16:24:26.211097 rag4p-0.3.0/rag4p/rag/generation/question_generator.py
--rw-r--r--   0        0        0     1710 2024-02-15 14:10:18.771548 rag4p-0.3.0/rag4p/rag/generation/question_generator_service.py
--rw-r--r--   0        0        0        0 2024-02-13 20:18:42.944968 rag4p-0.3.0/rag4p/rag/model/__init__.py
--rw-r--r--   0        0        0      494 2024-01-21 16:30:55.882221 rag4p-0.3.0/rag4p/rag/model/chunk.py
--rw-r--r--   0        0        0      282 2024-02-15 14:10:18.764160 rag4p-0.3.0/rag4p/rag/model/relevant_chunk.py
--rw-r--r--   0        0        0        0 2024-02-13 20:10:33.450731 rag4p-0.3.0/rag4p/rag/retrieval/__init__.py
--rw-r--r--   0        0        0      917 2024-02-15 14:20:29.071323 rag4p-0.3.0/rag4p/rag/retrieval/observed_retriever.py
--rw-r--r--   0        0        0        0 2024-02-13 20:11:00.416743 rag4p-0.3.0/rag4p/rag/retrieval/quality/__init__.py
--rw-r--r--   0        0        0      259 2024-01-21 12:16:35.290144 rag4p-0.3.0/rag4p/rag/retrieval/quality/question_answer_record.py
--rw-r--r--   0        0        0      337 2024-01-21 11:47:35.273879 rag4p-0.3.0/rag4p/rag/retrieval/quality/retrieval_quality.py
--rw-r--r--   0        0        0     1759 2024-05-17 15:11:07.973126 rag4p-0.3.0/rag4p/rag/retrieval/quality/retrieval_quality_service.py
--rw-r--r--   0        0        0      481 2024-01-17 15:45:56.775642 rag4p-0.3.0/rag4p/rag/retrieval/retrieval_output.py
--rw-r--r--   0        0        0      500 2024-02-15 14:20:29.076513 rag4p-0.3.0/rag4p/rag/retrieval/retrieval_strategy.py
--rw-r--r--   0        0        0      897 2024-02-15 14:33:56.290130 rag4p-0.3.0/rag4p/rag/retrieval/retriever.py
--rw-r--r--   0        0        0        0 2024-02-13 20:13:14.325777 rag4p-0.3.0/rag4p/rag/retrieval/strategies/__init__.py
--rw-r--r--   0        0        0     4133 2024-05-20 08:02:56.131116 rag4p-0.3.0/rag4p/rag/retrieval/strategies/document_retrieval_strategy.py
--rw-r--r--   0        0        0     1346 2024-02-15 14:18:36.054148 rag4p-0.3.0/rag4p/rag/retrieval/strategies/topn_retrieval_strategy.py
--rw-r--r--   0        0        0     2563 2024-02-15 14:18:36.048293 rag4p-0.3.0/rag4p/rag/retrieval/strategies/window_retrieval_strategy.py
--rw-r--r--   0        0        0        0 2024-02-13 20:14:17.876016 rag4p-0.3.0/rag4p/rag/store/__init__.py
--rw-r--r--   0        0        0      204 2024-02-15 14:22:14.366016 rag4p-0.3.0/rag4p/rag/store/content_store.py
--rw-r--r--   0        0        0        0 2024-02-13 20:14:47.220156 rag4p-0.3.0/rag4p/rag/store/local/__init__.py
--rw-r--r--   0        0        0     2814 2024-05-15 14:38:58.769218 rag4p-0.3.0/rag4p/rag/store/local/internal_content_store.py
--rw-r--r--   0        0        0        0 2024-01-18 17:24:10.044644 rag4p-0.3.0/rag4p/rag/tracker/__init__.py
--rw-r--r--   0        0        0     1304 2024-01-21 14:50:45.211063 rag4p-0.3.0/rag4p/rag/tracker/rag_observer.py
--rw-r--r--   0        0        0      108 2024-02-15 14:33:56.284091 rag4p-0.3.0/rag4p/rag/tracker/rag_tracker.py
--rw-r--r--   0        0        0        0 2024-01-17 16:06:54.281693 rag4p-0.3.0/rag4p/util/__init__.py
--rw-r--r--   0        0        0     3363 2024-01-21 09:28:32.748688 rag4p-0.3.0/rag4p/util/key_loader.py
--rw-r--r--   0        0        0      814 2024-02-15 15:32:43.848743 rag4p-0.3.0/rag4p/vasa_content_reader.py
--rw-r--r--   0        0        0     4337 1970-01-01 00:00:00.000000 rag4p-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3266 2024-05-20 08:34:12.059855 rag4p-0.4.0/README.md
+-rw-r--r--   0        0        0      781 2024-05-24 05:42:42.101645 rag4p-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-17 15:16:40.886501 rag4p-0.4.0/rag4p/__init__.py
+-rw-r--r--   0        0        0     3546 2024-05-11 10:19:26.281070 rag4p-0.4.0/rag4p/app_complete_local.py
+-rw-r--r--   0        0        0     3224 2024-02-15 14:42:08.665322 rag4p-0.4.0/rag4p/app_complete_weaviate.py
+-rw-r--r--   0        0        0     1154 2024-02-15 14:50:41.830101 rag4p-0.4.0/rag4p/app_generation_answer_generator.py
+-rw-r--r--   0        0        0     1318 2024-05-11 10:19:26.290206 rag4p-0.4.0/rag4p/app_generation_answer_quality.py
+-rw-r--r--   0        0        0     1292 2024-05-11 10:24:23.583279 rag4p-0.4.0/rag4p/app_generation_answer_quality_ollama.py
+-rw-r--r--   0        0        0     2708 2024-02-15 15:49:18.900194 rag4p-0.4.0/rag4p/app_generation_question_generator.py
+-rw-r--r--   0        0        0     1432 2024-02-15 15:31:45.716697 rag4p-0.4.0/rag4p/app_generation_questions_generator_vasa.py
+-rw-r--r--   0        0        0     1214 2024-02-15 15:59:09.706810 rag4p-0.4.0/rag4p/app_indexing_local.py
+-rw-r--r--   0        0        0     2330 2024-03-11 09:33:23.161900 rag4p-0.4.0/rag4p/app_indexing_weaviate.py
+-rw-r--r--   0        0        0     1254 2024-02-15 15:31:45.728308 rag4p-0.4.0/rag4p/app_retrieval_quality_vasa.py
+-rw-r--r--   0        0        0     1514 2024-05-15 14:45:34.878603 rag4p-0.4.0/rag4p/app_retrieval_retriever_local.py
+-rw-r--r--   0        0        0     1800 2024-05-21 18:57:47.887764 rag4p-0.4.0/rag4p/app_retrieval_retriever_weaviate.py
+-rw-r--r--   0        0        0     1878 2024-02-15 15:31:45.712149 rag4p-0.4.0/rag4p/app_retrieval_strategy.py
+-rw-r--r--   0        0        0      429 2024-01-31 07:51:24.674544 rag4p-0.4.0/rag4p/app_weaviate_info.py
+-rw-r--r--   0        0        0        0 2024-01-17 15:16:40.886501 rag4p-0.4.0/rag4p/indexing/__init__.py
+-rw-r--r--   0        0        0      117 2024-01-18 16:12:32.211578 rag4p-0.4.0/rag4p/indexing/content_reader.py
+-rw-r--r--   0        0        0      675 2024-02-15 14:54:08.869449 rag4p-0.4.0/rag4p/indexing/indexing_service.py
+-rw-r--r--   0        0        0      232 2024-01-17 15:25:27.590307 rag4p-0.4.0/rag4p/indexing/input_document.py
+-rw-r--r--   0        0        0      285 2024-02-13 20:32:37.812960 rag4p-0.4.0/rag4p/indexing/splitter.py
+-rw-r--r--   0        0        0        0 2024-02-13 19:57:32.062188 rag4p-0.4.0/rag4p/indexing/splitters/__init__.py
+-rw-r--r--   0        0        0     1356 2024-02-13 20:28:11.172941 rag4p-0.4.0/rag4p/indexing/splitters/max_token_splitter.py
+-rw-r--r--   0        0        0      671 2024-02-13 20:32:37.826115 rag4p-0.4.0/rag4p/indexing/splitters/sentence_splitter.py
+-rw-r--r--   0        0        0      474 2024-02-13 20:32:37.822569 rag4p-0.4.0/rag4p/indexing/splitters/single_chunk_splitter.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:16:16.212988 rag4p-0.4.0/rag4p/integrations/__init__.py
+-rw-r--r--   0        0        0      204 2024-05-10 14:28:00.181901 rag4p-0.4.0/rag4p/integrations/ollama/__init__.py
+-rw-r--r--   0        0        0     2361 2024-05-10 15:59:57.265154 rag4p-0.4.0/rag4p/integrations/ollama/access_ollama.py
+-rw-r--r--   0        0        0      808 2024-05-13 07:17:37.558316 rag4p-0.4.0/rag4p/integrations/ollama/ollama_answer_generator.py
+-rw-r--r--   0        0        0      547 2024-05-10 14:37:39.142352 rag4p-0.4.0/rag4p/integrations/ollama/ollama_embedder.py
+-rw-r--r--   0        0        0     1456 2024-05-13 07:17:37.553472 rag4p-0.4.0/rag4p/integrations/ollama/ollama_question_generator.py
+-rw-r--r--   0        0        0        0 2024-05-11 10:09:25.775349 rag4p-0.4.0/rag4p/integrations/ollama/quality/__init__.py
+-rw-r--r--   0        0        0     1429 2024-05-11 10:36:04.986424 rag4p-0.4.0/rag4p/integrations/ollama/quality/ollama_answer_quality_service.py
+-rw-r--r--   0        0        0      429 2024-05-11 10:04:59.548674 rag4p-0.4.0/rag4p/integrations/openai/__init__.py
+-rw-r--r--   0        0        0     1311 2024-05-11 09:33:48.693626 rag4p-0.4.0/rag4p/integrations/openai/openai_answer_generator.py
+-rw-r--r--   0        0        0      943 2024-02-13 21:03:08.370679 rag4p-0.4.0/rag4p/integrations/openai/openai_embedder.py
+-rw-r--r--   0        0        0     1709 2024-02-13 21:03:08.339951 rag4p-0.4.0/rag4p/integrations/openai/openai_question_generator.py
+-rw-r--r--   0        0        0        0 2024-05-11 09:39:07.588936 rag4p-0.4.0/rag4p/integrations/openai/quality/__init__.py
+-rw-r--r--   0        0        0     1828 2024-05-11 10:32:57.682591 rag4p-0.4.0/rag4p/integrations/openai/quality/openai_answer_quality_service.py
+-rw-r--r--   0        0        0       26 2024-03-11 09:33:23.149502 rag4p-0.4.0/rag4p/integrations/weaviate/__init__.py
+-rw-r--r--   0        0        0     2930 2024-03-11 09:33:23.144857 rag4p-0.4.0/rag4p/integrations/weaviate/access_weaviate.py
+-rw-r--r--   0        0        0     1001 2024-02-06 22:07:59.527805 rag4p-0.4.0/rag4p/integrations/weaviate/chunk_collection.py
+-rw-r--r--   0        0        0     1190 2024-03-11 09:33:23.157565 rag4p-0.4.0/rag4p/integrations/weaviate/weaviate_content_store.py
+-rw-r--r--   0        0        0     4610 2024-05-21 18:55:01.151138 rag4p-0.4.0/rag4p/integrations/weaviate/weaviate_retriever.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:01:14.586737 rag4p-0.4.0/rag4p/rag/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:01:31.907902 rag4p-0.4.0/rag4p/rag/embedding/__init__.py
+-rw-r--r--   0        0        0      190 2024-02-13 22:23:33.027284 rag4p-0.4.0/rag4p/rag/embedding/embedder.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:01:59.778652 rag4p-0.4.0/rag4p/rag/embedding/local/__init__.py
+-rw-r--r--   0        0        0     1426 2024-02-13 22:23:33.033084 rag4p-0.4.0/rag4p/rag/embedding/local/onnx_embedder.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:03:17.496572 rag4p-0.4.0/rag4p/rag/generation/__init__.py
+-rw-r--r--   0        0        0      262 2024-02-13 22:23:33.009410 rag4p-0.4.0/rag4p/rag/generation/answer_generator.py
+-rw-r--r--   0        0        0        0 2024-02-13 22:24:49.086889 rag4p-0.4.0/rag4p/rag/generation/chat/__init__.py
+-rw-r--r--   0        0        0      875 2024-02-13 22:46:03.836482 rag4p-0.4.0/rag4p/rag/generation/chat/chat_prompt.py
+-rw-r--r--   0        0        0      592 2024-02-15 14:06:38.894059 rag4p-0.4.0/rag4p/rag/generation/observed_answer_generator.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:08:51.049910 rag4p-0.4.0/rag4p/rag/generation/quality/__init__.py
+-rw-r--r--   0        0        0      178 2024-01-21 10:12:21.187448 rag4p-0.4.0/rag4p/rag/generation/quality/answer_from_context_quality.py
+-rw-r--r--   0        0        0      532 2024-02-13 22:23:33.021369 rag4p-0.4.0/rag4p/rag/generation/quality/answer_quality.py
+-rw-r--r--   0        0        0     4371 2024-05-18 10:20:51.530679 rag4p-0.4.0/rag4p/rag/generation/quality/answer_quality_service.py
+-rw-r--r--   0        0        0      418 2024-01-21 09:11:19.307021 rag4p-0.4.0/rag4p/rag/generation/quality/answer_to_question_quality.py
+-rw-r--r--   0        0        0      155 2024-01-28 16:24:26.211097 rag4p-0.4.0/rag4p/rag/generation/question_generator.py
+-rw-r--r--   0        0        0     1710 2024-02-15 14:10:18.771548 rag4p-0.4.0/rag4p/rag/generation/question_generator_service.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:18:42.944968 rag4p-0.4.0/rag4p/rag/model/__init__.py
+-rw-r--r--   0        0        0      494 2024-01-21 16:30:55.882221 rag4p-0.4.0/rag4p/rag/model/chunk.py
+-rw-r--r--   0        0        0      282 2024-02-15 14:10:18.764160 rag4p-0.4.0/rag4p/rag/model/relevant_chunk.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:10:33.450731 rag4p-0.4.0/rag4p/rag/retrieval/__init__.py
+-rw-r--r--   0        0        0      917 2024-02-15 14:20:29.071323 rag4p-0.4.0/rag4p/rag/retrieval/observed_retriever.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:11:00.416743 rag4p-0.4.0/rag4p/rag/retrieval/quality/__init__.py
+-rw-r--r--   0        0        0      259 2024-01-21 12:16:35.290144 rag4p-0.4.0/rag4p/rag/retrieval/quality/question_answer_record.py
+-rw-r--r--   0        0        0      337 2024-01-21 11:47:35.273879 rag4p-0.4.0/rag4p/rag/retrieval/quality/retrieval_quality.py
+-rw-r--r--   0        0        0     1759 2024-05-17 15:11:07.973126 rag4p-0.4.0/rag4p/rag/retrieval/quality/retrieval_quality_service.py
+-rw-r--r--   0        0        0      481 2024-01-17 15:45:56.775642 rag4p-0.4.0/rag4p/rag/retrieval/retrieval_output.py
+-rw-r--r--   0        0        0      500 2024-02-15 14:20:29.076513 rag4p-0.4.0/rag4p/rag/retrieval/retrieval_strategy.py
+-rw-r--r--   0        0        0      897 2024-02-15 14:33:56.290130 rag4p-0.4.0/rag4p/rag/retrieval/retriever.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:13:14.325777 rag4p-0.4.0/rag4p/rag/retrieval/strategies/__init__.py
+-rw-r--r--   0        0        0     4133 2024-05-20 08:02:56.131116 rag4p-0.4.0/rag4p/rag/retrieval/strategies/document_retrieval_strategy.py
+-rw-r--r--   0        0        0     1346 2024-02-15 14:18:36.054148 rag4p-0.4.0/rag4p/rag/retrieval/strategies/topn_retrieval_strategy.py
+-rw-r--r--   0        0        0     2563 2024-02-15 14:18:36.048293 rag4p-0.4.0/rag4p/rag/retrieval/strategies/window_retrieval_strategy.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:14:17.876016 rag4p-0.4.0/rag4p/rag/store/__init__.py
+-rw-r--r--   0        0        0      204 2024-02-15 14:22:14.366016 rag4p-0.4.0/rag4p/rag/store/content_store.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:14:47.220156 rag4p-0.4.0/rag4p/rag/store/local/__init__.py
+-rw-r--r--   0        0        0     2814 2024-05-15 14:38:58.769218 rag4p-0.4.0/rag4p/rag/store/local/internal_content_store.py
+-rw-r--r--   0        0        0        0 2024-01-18 17:24:10.044644 rag4p-0.4.0/rag4p/rag/tracker/__init__.py
+-rw-r--r--   0        0        0     1304 2024-01-21 14:50:45.211063 rag4p-0.4.0/rag4p/rag/tracker/rag_observer.py
+-rw-r--r--   0        0        0      108 2024-02-15 14:33:56.284091 rag4p-0.4.0/rag4p/rag/tracker/rag_tracker.py
+-rw-r--r--   0        0        0        0 2024-01-17 16:06:54.281693 rag4p-0.4.0/rag4p/util/__init__.py
+-rw-r--r--   0        0        0     3363 2024-01-21 09:28:32.748688 rag4p-0.4.0/rag4p/util/key_loader.py
+-rw-r--r--   0        0        0      814 2024-02-15 15:32:43.848743 rag4p-0.4.0/rag4p/vasa_content_reader.py
+-rw-r--r--   0        0        0     4337 1970-01-01 00:00:00.000000 rag4p-0.4.0/PKG-INFO
```

### Comparing `rag4p-0.3.0/README.md` & `rag4p-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -41,22 +41,22 @@
 Please use this key for the workshop only, and limit the amount of interaction, or we get blocked for exceeding our
 limits. The API key is obtained through a remote file, which is encrypted. Of course you can also use your own key if
 you have it.
 
 ### Environment variables
 The easiest way to load the API key is to set an environment variable for each required key. In Python we prefer the file .env.properties in the root of the project with the following properties:
 ```properties
-openai_api_key=sk-...
-weaviate_api_key=...
-weaviate_url=...
+OPENAI_API_KEY=sk-...
+WEAVIATE_API_KEY=...
+WEAVIATE_URL=...
 ```
 
 If you do not have your own key, you can load ours. The key is stored in a remote location. You need the .env.properties file in the root of the project with the following line:
 ```properties
-secret_key=...
+SECRET_KEY=...
 ```
 This secret key is used to decrypt the remote file containing the API keys. We will provide the value for this key
 during the workshop.
 
 ## Using Ollama
 There is a simple way to run a Language Model on your local machine. Depending on your machine and the chosen model, it runs fast. I am not going in to much details on how to install it, but you can find the installation instructions on the [Ollama Downloads page](https://ollama.com/download/).
```

### Comparing `rag4p-0.3.0/pyproject.toml` & `rag4p-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rag4p"
-version = "0.3.0"
+version = "0.4.0"
 description = "This project I use a lot for workshops, it contains some utils for splitters, tokenizers, and a weaviate client that I reuse a lot"
 authors = ["Jettro Coenradie <jettro.coenradie@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 nltk = "^3.8.1"
@@ -15,15 +15,15 @@
 python-dotenv = "^1.0.0"
 pandas = "^2.1.4"
 scipy = "^1.11.4"
 onnxruntime = "1.16.3"
 tokenizers = "^0.15.0"
 unidecode = "^1.3.8"
 weaviate-client = {version = "^4.0.0", allow-prereleases = false}
-tiktoken = "^0.6.0"
+tiktoken = "^0.7.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
 
 
 [build-system]
```

### Comparing `rag4p-0.3.0/rag4p/app_complete_local.py` & `rag4p-0.4.0/rag4p/app_complete_local.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/app_complete_weaviate.py` & `rag4p-0.4.0/rag4p/app_complete_weaviate.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/app_generation_answer_generator.py` & `rag4p-0.4.0/rag4p/app_generation_answer_generator.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/app_generation_answer_quality.py` & `rag4p-0.4.0/rag4p/app_generation_answer_quality.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/app_generation_answer_quality_ollama.py` & `rag4p-0.4.0/rag4p/app_generation_answer_quality_ollama.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/app_generation_question_generator.py` & `rag4p-0.4.0/rag4p/app_generation_question_generator.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/app_generation_questions_generator_vasa.py` & `rag4p-0.4.0/rag4p/app_generation_questions_generator_vasa.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/app_indexing_local.py` & `rag4p-0.4.0/rag4p/app_indexing_local.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/app_indexing_weaviate.py` & `rag4p-0.4.0/rag4p/app_indexing_weaviate.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/app_retrieval_quality_vasa.py` & `rag4p-0.4.0/rag4p/app_retrieval_quality_vasa.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/app_retrieval_retriever_local.py` & `rag4p-0.4.0/rag4p/app_retrieval_retriever_local.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/app_retrieval_retriever_weaviate.py` & `rag4p-0.4.0/rag4p/app_retrieval_retriever_weaviate.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,29 +13,30 @@
     client = AccessWeaviate(url=key_loader.get_weaviate_url(), access_key=key_loader.get_weaviate_api_key())
 
     client.print_meta()
 
     embedder = OpenAIEmbedder(api_key=key_loader.get_openai_api_key())
     retriever = WeaviateRetriever(weaviate_access=client,
                                   embedder=embedder,
-                                  additional_properties=["title", "timerange"],
-                                  hybrid=False)
+                                  additional_properties=["title", "speakers"],
+                                  hybrid=True)
 
     for chunk in retriever.loop_over_chunks():
         print(f"Document: {chunk.document_id} - {chunk.chunk_id}")
 
-    get_chunk = retriever.get_chunk(document_id="vasa", chunk_id=0)
+    get_chunk = retriever.get_chunk(document_id="using-ai-to-save-time-and-sanity", chunk_id=0)
     print("--------------------------------------------------")
     print(f"Document: {get_chunk.document_id} - {get_chunk.chunk_id}")
 
-    relevant_chunks = retriever.find_relevant_chunks("How many bolts were replaced?", max_results=2)
-    print(f"Found {len(relevant_chunks)} relevant chunks for query: How many bolts were replaced?")
+    relevant_chunks = retriever.find_relevant_chunks("What are jettro and daniel talking about?", max_results=2)
+    print(f"Found {len(relevant_chunks)} relevant chunks for query: What are jettro and daniel talking about?")
 
     for chunk in relevant_chunks:
         print(f"Document: {chunk.document_id}")
         print(f"Chunk id: {chunk.chunk_id}")
         print(f"Title: {chunk.properties['title']}")
+        print(f"Speakers: {chunk.properties['speakers']}")
         print(f"Text: {chunk.chunk_text}")
         print(f"Score: {chunk.score}")
         print("--------------------------------------------------")
 
     client.close()
```

### Comparing `rag4p-0.3.0/rag4p/app_retrieval_strategy.py` & `rag4p-0.4.0/rag4p/app_retrieval_strategy.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/indexing/indexing_service.py` & `rag4p-0.4.0/rag4p/indexing/indexing_service.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/indexing/splitters/max_token_splitter.py` & `rag4p-0.4.0/rag4p/indexing/splitters/max_token_splitter.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/indexing/splitters/sentence_splitter.py` & `rag4p-0.4.0/rag4p/indexing/splitters/sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/integrations/ollama/access_ollama.py` & `rag4p-0.4.0/rag4p/integrations/ollama/access_ollama.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/integrations/ollama/ollama_answer_generator.py` & `rag4p-0.4.0/rag4p/integrations/ollama/ollama_answer_generator.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/integrations/ollama/ollama_embedder.py` & `rag4p-0.4.0/rag4p/integrations/ollama/ollama_embedder.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/integrations/ollama/ollama_question_generator.py` & `rag4p-0.4.0/rag4p/integrations/ollama/ollama_question_generator.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/integrations/ollama/quality/ollama_answer_quality_service.py` & `rag4p-0.4.0/rag4p/integrations/ollama/quality/ollama_answer_quality_service.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/integrations/openai/openai_answer_generator.py` & `rag4p-0.4.0/rag4p/integrations/openai/openai_answer_generator.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/integrations/openai/openai_embedder.py` & `rag4p-0.4.0/rag4p/integrations/openai/openai_embedder.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/integrations/openai/openai_question_generator.py` & `rag4p-0.4.0/rag4p/integrations/openai/openai_question_generator.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/integrations/openai/quality/openai_answer_quality_service.py` & `rag4p-0.4.0/rag4p/integrations/openai/quality/openai_answer_quality_service.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/integrations/weaviate/access_weaviate.py` & `rag4p-0.4.0/rag4p/integrations/weaviate/access_weaviate.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/integrations/weaviate/chunk_collection.py` & `rag4p-0.4.0/rag4p/integrations/weaviate/chunk_collection.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/integrations/weaviate/weaviate_content_store.py` & `rag4p-0.4.0/rag4p/integrations/weaviate/weaviate_content_store.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/integrations/weaviate/weaviate_retriever.py` & `rag4p-0.4.0/rag4p/integrations/weaviate/weaviate_retriever.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         self.hybrid = hybrid
         self.collection_name = collection_name
 
     def find_relevant_chunks(self, question: str, max_results: int = 4) -> [RelevantChunk]:
         vector = self.embedder.embed(question)
         if self.hybrid:
             result = self.__chunk_collection().query.hybrid(query=question,
+                                                            query_properties=self.additional_properties,
                                                             limit=max_results,
                                                             alpha=0.5,
                                                             fusion_type=wvc.query.HybridFusion.RELATIVE_SCORE,
                                                             vector=vector,
                                                             return_metadata=wvc.query.MetadataQuery(
                                                                 distance=True, score=True)
                                                             )
```

### Comparing `rag4p-0.3.0/rag4p/rag/embedding/local/onnx_embedder.py` & `rag4p-0.4.0/rag4p/rag/embedding/local/onnx_embedder.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/rag/generation/chat/chat_prompt.py` & `rag4p-0.4.0/rag4p/rag/generation/chat/chat_prompt.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/rag/generation/observed_answer_generator.py` & `rag4p-0.4.0/rag4p/rag/generation/observed_answer_generator.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/rag/generation/quality/answer_quality.py` & `rag4p-0.4.0/rag4p/rag/generation/quality/answer_quality.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/rag/generation/quality/answer_quality_service.py` & `rag4p-0.4.0/rag4p/rag/generation/quality/answer_quality_service.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/rag/generation/question_generator_service.py` & `rag4p-0.4.0/rag4p/rag/generation/question_generator_service.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/rag/retrieval/observed_retriever.py` & `rag4p-0.4.0/rag4p/rag/retrieval/observed_retriever.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/rag/retrieval/quality/retrieval_quality_service.py` & `rag4p-0.4.0/rag4p/rag/retrieval/quality/retrieval_quality_service.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/rag/retrieval/retriever.py` & `rag4p-0.4.0/rag4p/rag/retrieval/retriever.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/rag/retrieval/strategies/document_retrieval_strategy.py` & `rag4p-0.4.0/rag4p/rag/retrieval/strategies/document_retrieval_strategy.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/rag/retrieval/strategies/topn_retrieval_strategy.py` & `rag4p-0.4.0/rag4p/rag/retrieval/strategies/topn_retrieval_strategy.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/rag/retrieval/strategies/window_retrieval_strategy.py` & `rag4p-0.4.0/rag4p/rag/retrieval/strategies/window_retrieval_strategy.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/rag/store/local/internal_content_store.py` & `rag4p-0.4.0/rag4p/rag/store/local/internal_content_store.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/rag/tracker/rag_observer.py` & `rag4p-0.4.0/rag4p/rag/tracker/rag_observer.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/util/key_loader.py` & `rag4p-0.4.0/rag4p/util/key_loader.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/rag4p/vasa_content_reader.py` & `rag4p-0.4.0/rag4p/vasa_content_reader.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.3.0/PKG-INFO` & `rag4p-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag4p
-Version: 0.3.0
+Version: 0.4.0
 Summary: This project I use a lot for workshops, it contains some utils for splitters, tokenizers, and a weaviate client that I reuse a lot
 Author: Jettro Coenradie
 Author-email: jettro.coenradie@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -14,15 +14,15 @@
 Requires-Dist: onnxruntime (==1.16.3)
 Requires-Dist: openai (>=1.13,<2.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
 Requires-Dist: pycryptodome (>=3.20.0,<4.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: scipy (>=1.11.4,<2.0.0)
-Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
+Requires-Dist: tiktoken (>=0.7.0,<0.8.0)
 Requires-Dist: tokenizers (>=0.15.0,<0.16.0)
 Requires-Dist: unidecode (>=1.3.8,<2.0.0)
 Requires-Dist: weaviate-client (>=4.0.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # RAG4P - Retrieval Augmented Generation for Python
 Welcome to the repository for our project [RAG4P.org](https://rag4p.org). This project is a Python implementation of the Retrieval Augmented Generation framework. It is a framework that is simple to use and understand. But powerful 
@@ -67,22 +67,22 @@
 Please use this key for the workshop only, and limit the amount of interaction, or we get blocked for exceeding our
 limits. The API key is obtained through a remote file, which is encrypted. Of course you can also use your own key if
 you have it.
 
 ### Environment variables
 The easiest way to load the API key is to set an environment variable for each required key. In Python we prefer the file .env.properties in the root of the project with the following properties:
 ```properties
-openai_api_key=sk-...
-weaviate_api_key=...
-weaviate_url=...
+OPENAI_API_KEY=sk-...
+WEAVIATE_API_KEY=...
+WEAVIATE_URL=...
 ```
 
 If you do not have your own key, you can load ours. The key is stored in a remote location. You need the .env.properties file in the root of the project with the following line:
 ```properties
-secret_key=...
+SECRET_KEY=...
 ```
 This secret key is used to decrypt the remote file containing the API keys. We will provide the value for this key
 during the workshop.
 
 ## Using Ollama
 There is a simple way to run a Language Model on your local machine. Depending on your machine and the chosen model, it runs fast. I am not going in to much details on how to install it, but you can find the installation instructions on the [Ollama Downloads page](https://ollama.com/download/).
```

