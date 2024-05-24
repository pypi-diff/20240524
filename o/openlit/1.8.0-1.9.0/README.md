# Comparing `tmp/openlit-1.8.0.tar.gz` & `tmp/openlit-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlit-1.8.0.tar", max compression
+gzip compressed data, was "openlit-1.9.0.tar", max compression
```

## Comparing `openlit-1.8.0.tar` & `openlit-1.9.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0    11357 2024-05-23 11:34:43.013329 openlit-1.8.0/LICENSE
--rw-r--r--   0        0        0    11181 2024-05-23 11:34:43.013329 openlit-1.8.0/README.md
--rw-r--r--   0        0        0      966 2024-05-23 11:34:43.013329 openlit-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     5545 2024-05-23 11:34:43.013329 openlit-1.8.0/src/openlit/__helpers.py
--rw-r--r--   0        0        0    10141 2024-05-23 11:34:43.013329 openlit-1.8.0/src/openlit/__init__.py
--rw-r--r--   0        0        0     1955 2024-05-23 11:34:43.013329 openlit-1.8.0/src/openlit/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0    16026 2024-05-23 11:34:43.013329 openlit-1.8.0/src/openlit/instrumentation/anthropic/anthropic.py
--rw-r--r--   0        0        0    16068 2024-05-23 11:34:43.013329 openlit-1.8.0/src/openlit/instrumentation/anthropic/async_anthropic.py
--rw-r--r--   0        0        0     1540 2024-05-23 11:34:43.013329 openlit-1.8.0/src/openlit/instrumentation/bedrock/__init__.py
--rw-r--r--   0        0        0    22278 2024-05-23 11:34:43.013329 openlit-1.8.0/src/openlit/instrumentation/bedrock/bedrock.py
--rw-r--r--   0        0        0     3253 2024-05-23 11:34:43.013329 openlit-1.8.0/src/openlit/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0    10407 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/chroma/chroma.py
--rw-r--r--   0        0        0     1920 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0    20381 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/cohere/cohere.py
--rw-r--r--   0        0        0     1911 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/groq/__init__.py
--rw-r--r--   0        0        0    19084 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/groq/async_groq.py
--rw-r--r--   0        0        0    19048 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/groq/groq.py
--rw-r--r--   0        0        0     1758 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/haystack/__init__.py
--rw-r--r--   0        0        0     3891 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/haystack/haystack.py
--rw-r--r--   0        0        0     2531 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     7639 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/langchain/langchain.py
--rw-r--r--   0        0        0     1973 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/llamaindex/__init__.py
--rw-r--r--   0        0        0     4048 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/llamaindex/llamaindex.py
--rw-r--r--   0        0        0     2961 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/milvus/__init__.py
--rw-r--r--   0        0        0     9121 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/milvus/milvus.py
--rw-r--r--   0        0        0     3156 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/mistral/__init__.py
--rw-r--r--   0        0        0    21361 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/mistral/async_mistral.py
--rw-r--r--   0        0        0    21212 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/mistral/mistral.py
--rw-r--r--   0        0        0     3812 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/ollama/__init__.py
--rw-r--r--   0        0        0    28991 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/ollama/async_ollama.py
--rw-r--r--   0        0        0    28901 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/ollama/ollama.py
--rw-r--r--   0        0        0    16265 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0    46297 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/openai/async_azure_openai.py
--rw-r--r--   0        0        0    45841 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/openai/async_openai.py
--rw-r--r--   0        0        0    46091 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/openai/azure_openai.py
--rw-r--r--   0        0        0    46522 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/openai/openai.py
--rw-r--r--   0        0        0     2526 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     8765 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/pinecone/pinecone.py
--rw-r--r--   0        0        0     4799 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/qdrant/__init__.py
--rw-r--r--   0        0        0    14436 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/qdrant/qdrant.py
--rw-r--r--   0        0        0     1478 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/transformers/__init__.py
--rw-r--r--   0        0        0     7592 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/transformers/transformers.py
--rw-r--r--   0        0        0     6079 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/vertexai/__init__.py
--rw-r--r--   0        0        0    52372 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/vertexai/async_vertexai.py
--rw-r--r--   0        0        0    52125 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/instrumentation/vertexai/vertexai.py
--rw-r--r--   0        0        0     4291 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/otel/metrics.py
--rw-r--r--   0        0        0     3712 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/otel/tracing.py
--rw-r--r--   0        0        0     6328 2024-05-23 11:34:43.017329 openlit-1.8.0/src/openlit/semcov/__init__.py
--rw-r--r--   0        0        0    12481 1970-01-01 00:00:00.000000 openlit-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-24 14:24:02.910928 openlit-1.9.0/LICENSE
+-rw-r--r--   0        0        0    11540 2024-05-24 14:24:02.910928 openlit-1.9.0/README.md
+-rw-r--r--   0        0        0      966 2024-05-24 14:24:02.910928 openlit-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5545 2024-05-24 14:24:02.910928 openlit-1.9.0/src/openlit/__helpers.py
+-rw-r--r--   0        0        0    10141 2024-05-24 14:24:02.910928 openlit-1.9.0/src/openlit/__init__.py
+-rw-r--r--   0        0        0     1955 2024-05-24 14:24:02.910928 openlit-1.9.0/src/openlit/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0    16026 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/anthropic/anthropic.py
+-rw-r--r--   0        0        0    16068 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/anthropic/async_anthropic.py
+-rw-r--r--   0        0        0     1540 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/bedrock/__init__.py
+-rw-r--r--   0        0        0    22278 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/bedrock/bedrock.py
+-rw-r--r--   0        0        0     3253 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0    10407 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/chroma/chroma.py
+-rw-r--r--   0        0        0     1920 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0    20437 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/cohere/cohere.py
+-rw-r--r--   0        0        0     1911 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/groq/__init__.py
+-rw-r--r--   0        0        0    19084 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/groq/async_groq.py
+-rw-r--r--   0        0        0    19048 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/groq/groq.py
+-rw-r--r--   0        0        0     1758 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/haystack/__init__.py
+-rw-r--r--   0        0        0     3891 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/haystack/haystack.py
+-rw-r--r--   0        0        0     2531 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     7639 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/langchain/langchain.py
+-rw-r--r--   0        0        0     1973 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0        0        0     4048 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/llamaindex/llamaindex.py
+-rw-r--r--   0        0        0     2961 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/milvus/__init__.py
+-rw-r--r--   0        0        0     9121 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/milvus/milvus.py
+-rw-r--r--   0        0        0     3156 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/mistral/__init__.py
+-rw-r--r--   0        0        0    21361 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/mistral/async_mistral.py
+-rw-r--r--   0        0        0    21212 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/mistral/mistral.py
+-rw-r--r--   0        0        0     3812 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/ollama/__init__.py
+-rw-r--r--   0        0        0    28991 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/ollama/async_ollama.py
+-rw-r--r--   0        0        0    28901 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/ollama/ollama.py
+-rw-r--r--   0        0        0    16265 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0    46297 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/openai/async_azure_openai.py
+-rw-r--r--   0        0        0    45841 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/openai/async_openai.py
+-rw-r--r--   0        0        0    46091 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/openai/azure_openai.py
+-rw-r--r--   0        0        0    46522 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/openai/openai.py
+-rw-r--r--   0        0        0     2526 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     8765 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/pinecone/pinecone.py
+-rw-r--r--   0        0        0     4799 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/qdrant/__init__.py
+-rw-r--r--   0        0        0    14436 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/qdrant/qdrant.py
+-rw-r--r--   0        0        0     1478 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/transformers/__init__.py
+-rw-r--r--   0        0        0     7592 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/transformers/transformers.py
+-rw-r--r--   0        0        0     6079 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/vertexai/__init__.py
+-rw-r--r--   0        0        0    52372 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/vertexai/async_vertexai.py
+-rw-r--r--   0        0        0    52125 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/instrumentation/vertexai/vertexai.py
+-rw-r--r--   0        0        0     4291 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/otel/metrics.py
+-rw-r--r--   0        0        0     3712 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/otel/tracing.py
+-rw-r--r--   0        0        0     6328 2024-05-24 14:24:02.914928 openlit-1.9.0/src/openlit/semcov/__init__.py
+-rw-r--r--   0        0        0    12840 1970-01-01 00:00:00.000000 openlit-1.9.0/PKG-INFO
```

### Comparing `openlit-1.8.0/LICENSE` & `openlit-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/README.md` & `openlit-1.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: openlit
+Version: 1.9.0
+Summary: OpenTelemetry-native Auto instrumentation library for monitoring LLM Applications, facilitating the integration of observability into your GenAI-driven projects
+Home-page: https://github.com/openlit/openlit/tree/main/openlit/python
+Keywords: OpenTelemetry,otel,otlp,llm,tracing,openai,anthropic,claude,cohere,llm monitoring,observability,monitoring,gpt,Generative AI,chatGPT
+Author: OpenLIT
+Requires-Python: >=3.7.1,<4.0.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: boto3 (>=1.34.0,<2.0.0)
+Requires-Dist: botocore (>=1.34.0,<2.0.0)
+Requires-Dist: opentelemetry-api (>=1.24.0,<2.0.0)
+Requires-Dist: opentelemetry-exporter-otlp (>=1.24.0,<2.0.0)
+Requires-Dist: opentelemetry-instrumentation (>=0.45b0,<0.46)
+Requires-Dist: opentelemetry-sdk (>=1.24.0,<2.0.0)
+Requires-Dist: requests (>=2.26.0,<3.0.0)
+Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
+Project-URL: Repository, https://github.com/openlit/openlit/tree/main/openlit/python
+Description-Content-Type: text/markdown
+
 <div align="center">
 <img src="https://github.com/openlit/.github/blob/main/profile/assets/wide-logo-no-bg.png?raw=true" alt="OpenLIT Logo" width="30%"><h1>
 OpenTelemetry Auto-Instrumentation for GenAI & LLM Applications</h1>
 
 **[Documentation](https://docs.openlit.io/) | [Quickstart](#-getting-started) | [Python SDK](https://github.com/openlit/openlit/tree/main/sdk/python)**
 
 [![OpenLIT](https://img.shields.io/badge/OpenLIT-orange)](https://github.com/openlit/openlit)
@@ -9,47 +34,39 @@
 [![Downloads](https://static.pepy.tech/badge/openlit/month)](https://pepy.tech/project/openlit)
 [![GitHub Last Commit](https://img.shields.io/github/last-commit/openlit/openlit)](https://github.com/openlit/openlit/pulse)
 [![GitHub Contributors](https://img.shields.io/github/contributors/openlit/openlit)](https://github.com/openlit/openlit/graphs/contributors)
 
 [![Slack](https://img.shields.io/badge/Slack-4A154B?logo=slack&logoColor=white)](https://join.slack.com/t/openlit/shared_invite/zt-2etnfttwg-TjP_7BZXfYg84oAukY8QRQ)
 [![X](https://img.shields.io/badge/follow-%40OpenLIT-1DA1F2?logo=x&style=social)](https://twitter.com/openlit_io)
 
+![OpenLIT Connections Banner](https://github.com/openlit/.github/blob/main/profile/assets/github-readme-connections-banner.png?raw=true)
+
+
 </div>
 
 OpenLIT Python SDK is an **OpenTelemetry-native** Auto instrumentation library for monitoring LLM Applications, facilitating the integration of observability into your GenAI-driven projects. Designed with simplicity and efficiency, OpenLIT offers the ability to embed observability into your GenAI-driven projects effortlessly using just **a single line of code**.
 
 Whether you're directly using LLM Libraries like OpenAI, Anthropic or building complex RAG Agents using Langchain, OpenLIT seamlessly integrates observability into your applications, ensuring enhanced performance and reliability across diverse scenarios.
 
 This project adheres to the [Semantic Conventions](https://github.com/open-telemetry/semantic-conventions/tree/main/docs/gen-ai) proposed by the OpenTelemetry community. You can check out the current definitions [here](src/openlit/semcov/__init__.py).
 
-## What can be Auto Instrumented?
+## Auto Instrumentation Capabilities
 
-### LLMs
-- [✅ OpenAI](https://docs.openlit.io/latest/integrations/openai)
-- [✅ Ollama](https://docs.openlit.io/latest/integrations/ollama)
-- [✅ Anthropic](https://docs.openlit.io/latest/integrations/anthropic)
-- [✅ Cohere](https://docs.openlit.io/latest/integrations/cohere)
-- [✅ Mistral](https://docs.openlit.io/latest/integrations/mistral)
-- [✅ Azure OpenAI](https://docs.openlit.io/latest/integrations/azure-openai)
-- [✅ HuggingFace Transformers](https://docs.openlit.io/latest/integrations/huggingface)
-- [✅ Amazon Bedrock](https://docs.openlit.io/latest/integrations/bedrock)
-- [✅ Vertex AI](https://docs.openlit.io/latest/integrations/vertexai)
-- [✅ Groq](https://docs.openlit.io/latest/integrations/groq)
-
-### Vector DBs
-- [✅ ChromaDB](https://docs.openlit.io/latest/integrations/chromadb)
-- [✅ Pinecone](https://docs.openlit.io/latest/integrations/pinecone)
-- [✅ Qdrant](https://docs.openlit.io/latest/integrations/qdrant)
-- [✅ Milvus](https://docs.openlit.io/latest/integrations/milvus)
-
-### Frameworks
-- [✅ Langchain](https://docs.openlit.io/latest/integrations/langchain)
-- [✅ LiteLLM](https://docs.openlit.io/latest/integrations/litellm)
-- [✅ LlamaIndex](https://docs.openlit.io/latest/integrations/llama-index)
-- [✅ Haystack](https://docs.openlit.io/latest/integrations/haystack)
+| LLMs                                                     | Vector DBs                                   | Frameworks                                   |
+|----------------------------------------------------------|----------------------------------------------|----------------------------------------------|
+| [✅ OpenAI](https://docs.openlit.io/latest/integrations/openai)               | [✅ ChromaDB](https://docs.openlit.io/latest/integrations/chromadb)       | [✅ Langchain](https://docs.openlit.io/latest/integrations/langchain)     |
+| [✅ Ollama](https://docs.openlit.io/latest/integrations/ollama)               | [✅ Pinecone](https://docs.openlit.io/latest/integrations/pinecone)       | [✅ LiteLLM](https://docs.openlit.io/latest/integrations/litellm)         |
+| [✅ Anthropic](https://docs.openlit.io/latest/integrations/anthropic)         | [✅ Qdrant](https://docs.openlit.io/latest/integrations/qdrant)           | [✅ LlamaIndex](https://docs.openlit.io/latest/integrations/llama-index)  |
+| [✅ Cohere](https://docs.openlit.io/latest/integrations/cohere)               | [✅ Milvus](https://docs.openlit.io/latest/integrations/milvus)           | [✅ Haystack](https://docs.openlit.io/latest/integrations/haystack)       |
+| [✅ Mistral](https://docs.openlit.io/latest/integrations/mistral)             |                                                                          |                                   
+| [✅ Azure OpenAI](https://docs.openlit.io/latest/integrations/azure-openai)   |                                                                          |                                        
+| [✅ HuggingFace Transformers](https://docs.openlit.io/latest/integrations/huggingface) |                                                                          |                                           
+| [✅ Amazon Bedrock](https://docs.openlit.io/latest/integrations/bedrock)         |                                                                          |                                       
+| [✅ Vertex AI](https://docs.openlit.io/latest/integrations/vertexai)         |                                                                          |                                      
+| [✅ Groq](https://docs.openlit.io/latest/integrations/groq)                   |                                                                          |                                
 
 ## Supported Destinations
 - [✅ OpenTelemetry Collector](https://docs.openlit.io/latest/connections/otelcol)
 - [✅ Prometheus + Tempo](https://docs.openlit.io/latest/connections/prometheus-tempo)
 - [✅ Prometheus + Jaeger](https://docs.openlit.io/latest/connections/prometheus-jaeger)
 - [✅ Grafana Cloud](https://docs.openlit.io/latest/connections/grafanacloud)
 - [✅ DataDog](https://docs.openlit.io/latest/connections/datadog)
@@ -63,69 +80,93 @@
 
 ```bash
 pip install openlit
 ```
 
 ## 🚀 Getting Started
 
-## Step 1: Install OpenLIT SDK
+### Step 1: Install OpenLIT
+
+Open your command line or terminal and run:
 
 ```bash
 pip install openlit
 ```
 
-### Step 2: Instrument your Application
-Integrating the OpenLIT into LLM applications is straightforward. Start monitoring for your LLM Application with just **one line of code**: 
+### Step 2: Initialize OpenLIT in your Application
+Integrating the OpenLIT into LLM applications is straightforward. Start monitoring for your LLM Application with just **two lines of code**: 
 
 ```python
 import openlit
 
 openlit.init()
 ```
 
-By default, OpenLIT directs traces and metrics straight to your console. To forward telemetry data to an HTTP OTLP endpoint, such as the OpenTelemetry Collector, set the `otlp_endpoint` parameter with the desired endpoint. Alternatively, you can configure the endpoint by setting the `OTEL_EXPORTER_OTLP_ENDPOINT` environment variable as recommended in the OpenTelemetry documentation.
+To forward telemetry data to an HTTP OTLP endpoint, such as the OpenTelemetry Collector, set the `otlp_endpoint` parameter with the desired endpoint. Alternatively, you can configure the endpoint by setting the `OTEL_EXPORTER_OTLP_ENDPOINT` environment variable as recommended in the OpenTelemetry documentation.
+
+> 💡 Info: If you dont provide `otlp_endpoint` function argument or set the `OTEL_EXPORTER_OTLP_ENDPOINT` environment variable, OpenLIT directs the trace directly to your console, which can be useful during development.
 
 To send telemetry to OpenTelemetry backends requiring authentication, set the `otlp_headers` parameter with its desired value. Alternatively, you can configure the endpoint by setting the `OTEL_EXPORTER_OTLP_HEADERS` environment variable as recommended in the OpenTelemetry documentation.
 
 #### Example
 
-Here is how you can send telemetry from OpenLIT to Grafana Cloud
+---
 
-```python
-openlit.init(
-  otlp_endpoint="https://otlp-gateway-prod-us-east-0.grafana.net/otlp", 
-  otlp_headers="Authorization=Basic%20<base64 encoded Instance ID and API Token>"
-)
-```
+<details>
+  <summary>Initialize using Function Arguments</summary>
+  
+  ---
 
-Alternatively, You can also choose to set these values using `OTEL_EXPORTER_OTLP_ENDPOINT` and `OTEL_EXPORTER_OTLP_HEADERS` environment variables
+  Add the following two lines to your application code:
+  
+  ```python
+  import openlit
+  
+  openlit.init(
+    otlp_endpoint="YOUR_OTEL_ENDPOINT", 
+    otlp_headers ="YOUR_OTEL_ENDPOINT_AUTH"
+  )
+  ```
 
-```python
-openlit.init()
-```
+</details>
 
-```env
-export OTEL_EXPORTER_OTLP_ENDPOINT = "https://otlp-gateway-prod-us-east-0.grafana.net/otlp"
-export OTEL_EXPORTER_OTLP_HEADERS = "Authorization=Basic%20<base64 encoded Instance ID and API Token>"
-```
+---
+
+<details>
+
+  <summary>Initialize using Environment Variables</summary>
+
+  ---
+
+  Add the following two lines to your application code:
+
+  ```python
+  import openlit
+
+  openlit.init()
+  ```
+  
+  Then, configure the your OTLP endpoint using environment variable:
+
+  ```env
+  export OTEL_EXPORTER_OTLP_ENDPOINT = "YOUR_OTEL_ENDPOINT"
+  export OTEL_EXPORTER_OTLP_HEADERS = "YOUR_OTEL_ENDPOINT_AUTH"
+  ```
+</details>
+
+---
 
 ### Step 3: Visualize and Optimize!
-With the LLM Observability data now being collected and sent to your chosen OpenTelemetry backend, the next step is to visualize and analyze this data to glean insights into your application's performance, behavior, and identify areas of improvement. Here is how you would use the data in Grafana, follow these detailed instructions to explore your LLM application's Telemetry data.
+With the LLM Observability data now being collected and sent to OpenLIT, the next step is to visualize and analyze this data to get insights into your LLM application’s performance, behavior, and identify areas of improvement.
+
+To begin exploring your LLM Application's performance data within the OpenLIT UI, please see the [Quickstart Guide](https://docs.openlit.io/latest/quickstart).
 
-   - Select the **Explore** option from Grafana's sidebar.
-   - At the top, ensure the correct Tempo data source is selected from the dropdown menu.
-   - Use the **Query** field to specify any particular traces you are interested in, or leave it empty to browse through all the available traces.
-   - You can adjust the time range to focus on specific periods of interest.
-   - Hit **Run Query** to fetch your trace data. You'll see a visual representation of your traces along with detailed information on particular spans when clicked.
-
-#### Next Steps
-
-- **Create Dashboards:** Beyond just exploring traces, consider creating dashboards in Grafana to monitor key performance indicators (KPIs) and metrics over time. Dashboards can be customized with various panels to display graphs, logs, and single stats that are most relevant to your application's performance and usage patterns.
-- **Set Alerts:** Grafana also allows you to set up alerts based on specific thresholds. This feature can be invaluable in proactively managing your application's health by notifying you of potential issues before they impact users.
-- **Iterate and Optimize:** Use the insights gained from your observability data to make informed decisions on optimizing your LLM application. This might involve refining model parameters, adjusting scaling strategies, or identifying and resolving bottlenecks.
+If you want to integrate and send metrics and traces to your existing observability tools, refer to our [Connections Guide](https://docs.openlit.io/latest/connections/intro) for detailed instructions.
+
+![](https://github.com/openlit/.github/blob/main/profile/assets/openlit-client-1.png?raw=true)
 
 
 ### Configuration
 
 Below is a detailed overview of the configuration options available, allowing you to adjust OpenLIT's behavior and functionality to align with your specific observability needs:
 
 | Argument                | Description                                                                                   | Default Value  | Required |
@@ -134,15 +175,15 @@
 | `application_name`      | Identifies the name of your application.                                                      | `"default"`    |    Yes   |
 | `tracer`                | An instance of OpenTelemetry Tracer for tracing operations.                                   | `None`         |    No    |
 | `meter`                 | An OpenTelemetry Metrics instance for capturing metrics.                                      | `None`         |    No    |
 | `otlp_endpoint`         | Specifies the OTLP endpoint for transmitting telemetry data.                                  | `None`         |    No    |
 | `otlp_headers`          | Defines headers for the OTLP exporter, useful for backends requiring authentication.          | `None`         |    No    |
 | `disable_batch`         | A flag to disable batch span processing, favoring immediate dispatch.                         | `False`        |    No    |
 | `trace_content`         | Enables tracing of content for deeper insights.                                               | `True`         |    No    |
-| `disabled_instrumentors`| List of instrumentors to disable. Choices: `["openai", "anthropic", "langchain", "cohere", "mistral", "transformers", "chroma", "pinecone"]`. | `None` |    No    |
+| `disabled_instrumentors`| List of instrumentors to disable. | `None` |    No    |
 | `disable_metrics`       | If set, disables the collection of metrics.                                                   | `False`        |    No    |
 | `pricing_json`          | URL or file path of the pricing JSON file.                                             | `https://github.com/openlit/openlit/blob/main/assets/pricing.json`        |    No    |
 
 ## 🌱 Contributing
 
 Whether it's big or small, we love contributions 💚. Check out our [Contribution guide](../../CONTRIBUTING.md) to get started
 
@@ -156,7 +197,8 @@
 
 Connect with the OpenLIT community and maintainers for support, discussions, and updates:
 
 - 🌟 If you like it, Leave a star on our [GitHub](https://github.com/openlit/openlit/)
 - 🌍 Join our [Slack](https://join.slack.com/t/openlit/shared_invite/zt-2etnfttwg-TjP_7BZXfYg84oAukY8QRQ) Community for live interactions and questions.
 - 🐞 Report bugs on our [GitHub Issues](https://github.com/openlit/openlit/issues) to help us improve OpenLIT.
 - 𝕏 Follow us on [X](https://x.com/openlit_io) for the latest updates and news.
+
```

### Comparing `openlit-1.8.0/pyproject.toml` & `openlit-1.9.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openlit"
-version = "1.8.0"
+version = "1.9.0"
 description = "OpenTelemetry-native Auto instrumentation library for monitoring LLM Applications, facilitating the integration of observability into your GenAI-driven projects"
 authors = ["OpenLIT"]
 repository = "https://github.com/openlit/openlit/tree/main/openlit/python"
 readme = "README.md"
 homepage = "https://github.com/openlit/openlit/tree/main/openlit/python"
 keywords = ["OpenTelemetry", "otel", "otlp","llm", "tracing", "openai", "anthropic", "claude", "cohere", "llm monitoring", "observability", "monitoring", "gpt", "Generative AI", "chatGPT"]
```

### Comparing `openlit-1.8.0/src/openlit/__helpers.py` & `openlit-1.9.0/src/openlit/__helpers.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/__init__.py` & `openlit-1.9.0/src/openlit/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/anthropic/__init__.py` & `openlit-1.9.0/src/openlit/instrumentation/anthropic/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/anthropic/anthropic.py` & `openlit-1.9.0/src/openlit/instrumentation/anthropic/anthropic.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/anthropic/async_anthropic.py` & `openlit-1.9.0/src/openlit/instrumentation/anthropic/async_anthropic.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/bedrock/__init__.py` & `openlit-1.9.0/src/openlit/instrumentation/bedrock/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/bedrock/bedrock.py` & `openlit-1.9.0/src/openlit/instrumentation/bedrock/bedrock.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/chroma/__init__.py` & `openlit-1.9.0/src/openlit/instrumentation/chroma/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/chroma/chroma.py` & `openlit-1.9.0/src/openlit/instrumentation/chroma/chroma.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/cohere/__init__.py` & `openlit-1.9.0/src/openlit/instrumentation/cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/cohere/cohere.py` & `openlit-1.9.0/src/openlit/instrumentation/cohere/cohere.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,17 +199,17 @@
                 span.set_attribute(SemanticConvetion.GEN_AI_REQUEST_FREQUENCY_PENALTY,
                                     kwargs.get("frequency_penalty", 0.0))
                 span.set_attribute(SemanticConvetion.GEN_AI_REQUEST_PRESENCE_PENALTY,
                                     kwargs.get("presence_penalty", 0.0))
                 span.set_attribute(SemanticConvetion.GEN_AI_REQUEST_IS_STREAM,
                                     False)
                 span.set_attribute(SemanticConvetion.GEN_AI_RESPONSE_ID,
-                                    response.response_id)
+                                    response.generation_id)
                 span.set_attribute(SemanticConvetion.GEN_AI_RESPONSE_FINISH_REASON,
-                                    response.response_id)
+                                    response.finish_reason)
                 span.set_attribute(SemanticConvetion.GEN_AI_USAGE_PROMPT_TOKENS,
                                     response.meta.billed_units.input_tokens)
                 span.set_attribute(SemanticConvetion.GEN_AI_USAGE_COMPLETION_TOKENS,
                                     response.meta.billed_units.output_tokens)
                 span.set_attribute(SemanticConvetion.GEN_AI_USAGE_TOTAL_TOKENS,
                                     response.meta.billed_units.input_tokens +
                                     response.meta.billed_units.output_tokens)
@@ -302,18 +302,19 @@
                 llmresponse = ""
 
                 # Loop through streaming events capturing relevant details
                 for event in wrapped(*args, **kwargs):
                     # Collect message IDs and aggregated response from events
                     if event.event_type == "stream-end":
                         llmresponse = event.response.text
-                        response_id = event.response.response_id
                         prompt_tokens = event.response.meta.billed_units.input_tokens
                         completion_tokens = event.response.meta.billed_units.output_tokens
                         finish_reason = event.finish_reason
+                    if event.event_type == "stream-start":
+                        response_id = event.generation_id
                     yield event
 
                 # Handling exception ensure observability without disrupting operation
                 try:
                     # Calculate cost of the operation
                     cost = get_chat_model_cost(kwargs.get("model", "command"),
                                                 pricing_info, prompt_tokens, completion_tokens)
```

### Comparing `openlit-1.8.0/src/openlit/instrumentation/groq/__init__.py` & `openlit-1.9.0/src/openlit/instrumentation/groq/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/groq/async_groq.py` & `openlit-1.9.0/src/openlit/instrumentation/groq/async_groq.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/groq/groq.py` & `openlit-1.9.0/src/openlit/instrumentation/groq/groq.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/haystack/__init__.py` & `openlit-1.9.0/src/openlit/instrumentation/haystack/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/haystack/haystack.py` & `openlit-1.9.0/src/openlit/instrumentation/haystack/haystack.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/langchain/__init__.py` & `openlit-1.9.0/src/openlit/instrumentation/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/langchain/langchain.py` & `openlit-1.9.0/src/openlit/instrumentation/langchain/langchain.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/llamaindex/__init__.py` & `openlit-1.9.0/src/openlit/instrumentation/llamaindex/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/llamaindex/llamaindex.py` & `openlit-1.9.0/src/openlit/instrumentation/llamaindex/llamaindex.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/milvus/__init__.py` & `openlit-1.9.0/src/openlit/instrumentation/milvus/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/milvus/milvus.py` & `openlit-1.9.0/src/openlit/instrumentation/milvus/milvus.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/mistral/__init__.py` & `openlit-1.9.0/src/openlit/instrumentation/mistral/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/mistral/async_mistral.py` & `openlit-1.9.0/src/openlit/instrumentation/mistral/async_mistral.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/mistral/mistral.py` & `openlit-1.9.0/src/openlit/instrumentation/mistral/mistral.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/ollama/__init__.py` & `openlit-1.9.0/src/openlit/instrumentation/ollama/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/ollama/async_ollama.py` & `openlit-1.9.0/src/openlit/instrumentation/ollama/async_ollama.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/ollama/ollama.py` & `openlit-1.9.0/src/openlit/instrumentation/ollama/ollama.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/openai/__init__.py` & `openlit-1.9.0/src/openlit/instrumentation/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/openai/async_azure_openai.py` & `openlit-1.9.0/src/openlit/instrumentation/openai/async_azure_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/openai/async_openai.py` & `openlit-1.9.0/src/openlit/instrumentation/openai/async_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/openai/azure_openai.py` & `openlit-1.9.0/src/openlit/instrumentation/openai/azure_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/openai/openai.py` & `openlit-1.9.0/src/openlit/instrumentation/openai/openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/pinecone/__init__.py` & `openlit-1.9.0/src/openlit/instrumentation/pinecone/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/pinecone/pinecone.py` & `openlit-1.9.0/src/openlit/instrumentation/pinecone/pinecone.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/qdrant/__init__.py` & `openlit-1.9.0/src/openlit/instrumentation/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/qdrant/qdrant.py` & `openlit-1.9.0/src/openlit/instrumentation/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/transformers/__init__.py` & `openlit-1.9.0/src/openlit/instrumentation/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/transformers/transformers.py` & `openlit-1.9.0/src/openlit/instrumentation/transformers/transformers.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/vertexai/__init__.py` & `openlit-1.9.0/src/openlit/instrumentation/vertexai/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/vertexai/async_vertexai.py` & `openlit-1.9.0/src/openlit/instrumentation/vertexai/async_vertexai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/instrumentation/vertexai/vertexai.py` & `openlit-1.9.0/src/openlit/instrumentation/vertexai/vertexai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/otel/metrics.py` & `openlit-1.9.0/src/openlit/otel/metrics.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/otel/tracing.py` & `openlit-1.9.0/src/openlit/otel/tracing.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/src/openlit/semcov/__init__.py` & `openlit-1.9.0/src/openlit/semcov/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.8.0/PKG-INFO` & `openlit-1.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: openlit
-Version: 1.8.0
-Summary: OpenTelemetry-native Auto instrumentation library for monitoring LLM Applications, facilitating the integration of observability into your GenAI-driven projects
-Home-page: https://github.com/openlit/openlit/tree/main/openlit/python
-Keywords: OpenTelemetry,otel,otlp,llm,tracing,openai,anthropic,claude,cohere,llm monitoring,observability,monitoring,gpt,Generative AI,chatGPT
-Author: OpenLIT
-Requires-Python: >=3.7.1,<4.0.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: boto3 (>=1.34.0,<2.0.0)
-Requires-Dist: botocore (>=1.34.0,<2.0.0)
-Requires-Dist: opentelemetry-api (>=1.24.0,<2.0.0)
-Requires-Dist: opentelemetry-exporter-otlp (>=1.24.0,<2.0.0)
-Requires-Dist: opentelemetry-instrumentation (>=0.45b0,<0.46)
-Requires-Dist: opentelemetry-sdk (>=1.24.0,<2.0.0)
-Requires-Dist: requests (>=2.26.0,<3.0.0)
-Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
-Project-URL: Repository, https://github.com/openlit/openlit/tree/main/openlit/python
-Description-Content-Type: text/markdown
-
 <div align="center">
 <img src="https://github.com/openlit/.github/blob/main/profile/assets/wide-logo-no-bg.png?raw=true" alt="OpenLIT Logo" width="30%"><h1>
 OpenTelemetry Auto-Instrumentation for GenAI & LLM Applications</h1>
 
 **[Documentation](https://docs.openlit.io/) | [Quickstart](#-getting-started) | [Python SDK](https://github.com/openlit/openlit/tree/main/sdk/python)**
 
 [![OpenLIT](https://img.shields.io/badge/OpenLIT-orange)](https://github.com/openlit/openlit)
@@ -34,47 +9,39 @@
 [![Downloads](https://static.pepy.tech/badge/openlit/month)](https://pepy.tech/project/openlit)
 [![GitHub Last Commit](https://img.shields.io/github/last-commit/openlit/openlit)](https://github.com/openlit/openlit/pulse)
 [![GitHub Contributors](https://img.shields.io/github/contributors/openlit/openlit)](https://github.com/openlit/openlit/graphs/contributors)
 
 [![Slack](https://img.shields.io/badge/Slack-4A154B?logo=slack&logoColor=white)](https://join.slack.com/t/openlit/shared_invite/zt-2etnfttwg-TjP_7BZXfYg84oAukY8QRQ)
 [![X](https://img.shields.io/badge/follow-%40OpenLIT-1DA1F2?logo=x&style=social)](https://twitter.com/openlit_io)
 
+![OpenLIT Connections Banner](https://github.com/openlit/.github/blob/main/profile/assets/github-readme-connections-banner.png?raw=true)
+
+
 </div>
 
 OpenLIT Python SDK is an **OpenTelemetry-native** Auto instrumentation library for monitoring LLM Applications, facilitating the integration of observability into your GenAI-driven projects. Designed with simplicity and efficiency, OpenLIT offers the ability to embed observability into your GenAI-driven projects effortlessly using just **a single line of code**.
 
 Whether you're directly using LLM Libraries like OpenAI, Anthropic or building complex RAG Agents using Langchain, OpenLIT seamlessly integrates observability into your applications, ensuring enhanced performance and reliability across diverse scenarios.
 
 This project adheres to the [Semantic Conventions](https://github.com/open-telemetry/semantic-conventions/tree/main/docs/gen-ai) proposed by the OpenTelemetry community. You can check out the current definitions [here](src/openlit/semcov/__init__.py).
 
-## What can be Auto Instrumented?
+## Auto Instrumentation Capabilities
 
-### LLMs
-- [✅ OpenAI](https://docs.openlit.io/latest/integrations/openai)
-- [✅ Ollama](https://docs.openlit.io/latest/integrations/ollama)
-- [✅ Anthropic](https://docs.openlit.io/latest/integrations/anthropic)
-- [✅ Cohere](https://docs.openlit.io/latest/integrations/cohere)
-- [✅ Mistral](https://docs.openlit.io/latest/integrations/mistral)
-- [✅ Azure OpenAI](https://docs.openlit.io/latest/integrations/azure-openai)
-- [✅ HuggingFace Transformers](https://docs.openlit.io/latest/integrations/huggingface)
-- [✅ Amazon Bedrock](https://docs.openlit.io/latest/integrations/bedrock)
-- [✅ Vertex AI](https://docs.openlit.io/latest/integrations/vertexai)
-- [✅ Groq](https://docs.openlit.io/latest/integrations/groq)
-
-### Vector DBs
-- [✅ ChromaDB](https://docs.openlit.io/latest/integrations/chromadb)
-- [✅ Pinecone](https://docs.openlit.io/latest/integrations/pinecone)
-- [✅ Qdrant](https://docs.openlit.io/latest/integrations/qdrant)
-- [✅ Milvus](https://docs.openlit.io/latest/integrations/milvus)
-
-### Frameworks
-- [✅ Langchain](https://docs.openlit.io/latest/integrations/langchain)
-- [✅ LiteLLM](https://docs.openlit.io/latest/integrations/litellm)
-- [✅ LlamaIndex](https://docs.openlit.io/latest/integrations/llama-index)
-- [✅ Haystack](https://docs.openlit.io/latest/integrations/haystack)
+| LLMs                                                     | Vector DBs                                   | Frameworks                                   |
+|----------------------------------------------------------|----------------------------------------------|----------------------------------------------|
+| [✅ OpenAI](https://docs.openlit.io/latest/integrations/openai)               | [✅ ChromaDB](https://docs.openlit.io/latest/integrations/chromadb)       | [✅ Langchain](https://docs.openlit.io/latest/integrations/langchain)     |
+| [✅ Ollama](https://docs.openlit.io/latest/integrations/ollama)               | [✅ Pinecone](https://docs.openlit.io/latest/integrations/pinecone)       | [✅ LiteLLM](https://docs.openlit.io/latest/integrations/litellm)         |
+| [✅ Anthropic](https://docs.openlit.io/latest/integrations/anthropic)         | [✅ Qdrant](https://docs.openlit.io/latest/integrations/qdrant)           | [✅ LlamaIndex](https://docs.openlit.io/latest/integrations/llama-index)  |
+| [✅ Cohere](https://docs.openlit.io/latest/integrations/cohere)               | [✅ Milvus](https://docs.openlit.io/latest/integrations/milvus)           | [✅ Haystack](https://docs.openlit.io/latest/integrations/haystack)       |
+| [✅ Mistral](https://docs.openlit.io/latest/integrations/mistral)             |                                                                          |                                   
+| [✅ Azure OpenAI](https://docs.openlit.io/latest/integrations/azure-openai)   |                                                                          |                                        
+| [✅ HuggingFace Transformers](https://docs.openlit.io/latest/integrations/huggingface) |                                                                          |                                           
+| [✅ Amazon Bedrock](https://docs.openlit.io/latest/integrations/bedrock)         |                                                                          |                                       
+| [✅ Vertex AI](https://docs.openlit.io/latest/integrations/vertexai)         |                                                                          |                                      
+| [✅ Groq](https://docs.openlit.io/latest/integrations/groq)                   |                                                                          |                                
 
 ## Supported Destinations
 - [✅ OpenTelemetry Collector](https://docs.openlit.io/latest/connections/otelcol)
 - [✅ Prometheus + Tempo](https://docs.openlit.io/latest/connections/prometheus-tempo)
 - [✅ Prometheus + Jaeger](https://docs.openlit.io/latest/connections/prometheus-jaeger)
 - [✅ Grafana Cloud](https://docs.openlit.io/latest/connections/grafanacloud)
 - [✅ DataDog](https://docs.openlit.io/latest/connections/datadog)
@@ -88,69 +55,93 @@
 
 ```bash
 pip install openlit
 ```
 
 ## 🚀 Getting Started
 
-## Step 1: Install OpenLIT SDK
+### Step 1: Install OpenLIT
+
+Open your command line or terminal and run:
 
 ```bash
 pip install openlit
 ```
 
-### Step 2: Instrument your Application
-Integrating the OpenLIT into LLM applications is straightforward. Start monitoring for your LLM Application with just **one line of code**: 
+### Step 2: Initialize OpenLIT in your Application
+Integrating the OpenLIT into LLM applications is straightforward. Start monitoring for your LLM Application with just **two lines of code**: 
 
 ```python
 import openlit
 
 openlit.init()
 ```
 
-By default, OpenLIT directs traces and metrics straight to your console. To forward telemetry data to an HTTP OTLP endpoint, such as the OpenTelemetry Collector, set the `otlp_endpoint` parameter with the desired endpoint. Alternatively, you can configure the endpoint by setting the `OTEL_EXPORTER_OTLP_ENDPOINT` environment variable as recommended in the OpenTelemetry documentation.
+To forward telemetry data to an HTTP OTLP endpoint, such as the OpenTelemetry Collector, set the `otlp_endpoint` parameter with the desired endpoint. Alternatively, you can configure the endpoint by setting the `OTEL_EXPORTER_OTLP_ENDPOINT` environment variable as recommended in the OpenTelemetry documentation.
+
+> 💡 Info: If you dont provide `otlp_endpoint` function argument or set the `OTEL_EXPORTER_OTLP_ENDPOINT` environment variable, OpenLIT directs the trace directly to your console, which can be useful during development.
 
 To send telemetry to OpenTelemetry backends requiring authentication, set the `otlp_headers` parameter with its desired value. Alternatively, you can configure the endpoint by setting the `OTEL_EXPORTER_OTLP_HEADERS` environment variable as recommended in the OpenTelemetry documentation.
 
 #### Example
 
-Here is how you can send telemetry from OpenLIT to Grafana Cloud
+---
 
-```python
-openlit.init(
-  otlp_endpoint="https://otlp-gateway-prod-us-east-0.grafana.net/otlp", 
-  otlp_headers="Authorization=Basic%20<base64 encoded Instance ID and API Token>"
-)
-```
+<details>
+  <summary>Initialize using Function Arguments</summary>
+  
+  ---
 
-Alternatively, You can also choose to set these values using `OTEL_EXPORTER_OTLP_ENDPOINT` and `OTEL_EXPORTER_OTLP_HEADERS` environment variables
+  Add the following two lines to your application code:
+  
+  ```python
+  import openlit
+  
+  openlit.init(
+    otlp_endpoint="YOUR_OTEL_ENDPOINT", 
+    otlp_headers ="YOUR_OTEL_ENDPOINT_AUTH"
+  )
+  ```
 
-```python
-openlit.init()
-```
+</details>
 
-```env
-export OTEL_EXPORTER_OTLP_ENDPOINT = "https://otlp-gateway-prod-us-east-0.grafana.net/otlp"
-export OTEL_EXPORTER_OTLP_HEADERS = "Authorization=Basic%20<base64 encoded Instance ID and API Token>"
-```
+---
+
+<details>
+
+  <summary>Initialize using Environment Variables</summary>
+
+  ---
+
+  Add the following two lines to your application code:
+
+  ```python
+  import openlit
+
+  openlit.init()
+  ```
+  
+  Then, configure the your OTLP endpoint using environment variable:
+
+  ```env
+  export OTEL_EXPORTER_OTLP_ENDPOINT = "YOUR_OTEL_ENDPOINT"
+  export OTEL_EXPORTER_OTLP_HEADERS = "YOUR_OTEL_ENDPOINT_AUTH"
+  ```
+</details>
+
+---
 
 ### Step 3: Visualize and Optimize!
-With the LLM Observability data now being collected and sent to your chosen OpenTelemetry backend, the next step is to visualize and analyze this data to glean insights into your application's performance, behavior, and identify areas of improvement. Here is how you would use the data in Grafana, follow these detailed instructions to explore your LLM application's Telemetry data.
+With the LLM Observability data now being collected and sent to OpenLIT, the next step is to visualize and analyze this data to get insights into your LLM application’s performance, behavior, and identify areas of improvement.
+
+To begin exploring your LLM Application's performance data within the OpenLIT UI, please see the [Quickstart Guide](https://docs.openlit.io/latest/quickstart).
 
-   - Select the **Explore** option from Grafana's sidebar.
-   - At the top, ensure the correct Tempo data source is selected from the dropdown menu.
-   - Use the **Query** field to specify any particular traces you are interested in, or leave it empty to browse through all the available traces.
-   - You can adjust the time range to focus on specific periods of interest.
-   - Hit **Run Query** to fetch your trace data. You'll see a visual representation of your traces along with detailed information on particular spans when clicked.
-
-#### Next Steps
-
-- **Create Dashboards:** Beyond just exploring traces, consider creating dashboards in Grafana to monitor key performance indicators (KPIs) and metrics over time. Dashboards can be customized with various panels to display graphs, logs, and single stats that are most relevant to your application's performance and usage patterns.
-- **Set Alerts:** Grafana also allows you to set up alerts based on specific thresholds. This feature can be invaluable in proactively managing your application's health by notifying you of potential issues before they impact users.
-- **Iterate and Optimize:** Use the insights gained from your observability data to make informed decisions on optimizing your LLM application. This might involve refining model parameters, adjusting scaling strategies, or identifying and resolving bottlenecks.
+If you want to integrate and send metrics and traces to your existing observability tools, refer to our [Connections Guide](https://docs.openlit.io/latest/connections/intro) for detailed instructions.
+
+![](https://github.com/openlit/.github/blob/main/profile/assets/openlit-client-1.png?raw=true)
 
 
 ### Configuration
 
 Below is a detailed overview of the configuration options available, allowing you to adjust OpenLIT's behavior and functionality to align with your specific observability needs:
 
 | Argument                | Description                                                                                   | Default Value  | Required |
@@ -159,15 +150,15 @@
 | `application_name`      | Identifies the name of your application.                                                      | `"default"`    |    Yes   |
 | `tracer`                | An instance of OpenTelemetry Tracer for tracing operations.                                   | `None`         |    No    |
 | `meter`                 | An OpenTelemetry Metrics instance for capturing metrics.                                      | `None`         |    No    |
 | `otlp_endpoint`         | Specifies the OTLP endpoint for transmitting telemetry data.                                  | `None`         |    No    |
 | `otlp_headers`          | Defines headers for the OTLP exporter, useful for backends requiring authentication.          | `None`         |    No    |
 | `disable_batch`         | A flag to disable batch span processing, favoring immediate dispatch.                         | `False`        |    No    |
 | `trace_content`         | Enables tracing of content for deeper insights.                                               | `True`         |    No    |
-| `disabled_instrumentors`| List of instrumentors to disable. Choices: `["openai", "anthropic", "langchain", "cohere", "mistral", "transformers", "chroma", "pinecone"]`. | `None` |    No    |
+| `disabled_instrumentors`| List of instrumentors to disable. | `None` |    No    |
 | `disable_metrics`       | If set, disables the collection of metrics.                                                   | `False`        |    No    |
 | `pricing_json`          | URL or file path of the pricing JSON file.                                             | `https://github.com/openlit/openlit/blob/main/assets/pricing.json`        |    No    |
 
 ## 🌱 Contributing
 
 Whether it's big or small, we love contributions 💚. Check out our [Contribution guide](../../CONTRIBUTING.md) to get started
 
@@ -181,8 +172,7 @@
 
 Connect with the OpenLIT community and maintainers for support, discussions, and updates:
 
 - 🌟 If you like it, Leave a star on our [GitHub](https://github.com/openlit/openlit/)
 - 🌍 Join our [Slack](https://join.slack.com/t/openlit/shared_invite/zt-2etnfttwg-TjP_7BZXfYg84oAukY8QRQ) Community for live interactions and questions.
 - 🐞 Report bugs on our [GitHub Issues](https://github.com/openlit/openlit/issues) to help us improve OpenLIT.
 - 𝕏 Follow us on [X](https://x.com/openlit_io) for the latest updates and news.
-
```

