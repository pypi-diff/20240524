# Comparing `tmp/proxyllm-0.2.1.tar.gz` & `tmp/proxyllm-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxyllm-0.2.1.tar", max compression
+gzip compressed data, was "proxyllm-0.2.2.tar", max compression
```

## Comparing `proxyllm-0.2.1.tar` & `proxyllm-0.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1066 2024-05-03 16:18:32.748021 proxyllm-0.2.1/LICENSE
--rw-r--r--   0        0        0     9607 2024-05-03 16:26:19.835639 proxyllm-0.2.1/README.md
--rw-r--r--   0        0        0       39 2024-05-03 16:18:32.751240 proxyllm-0.2.1/proxyllm/__init__.py
--rw-r--r--   0        0        0      795 2024-05-03 16:18:32.751576 proxyllm-0.2.1/proxyllm/cli.py
--rw-r--r--   0        0        0        0 2024-05-03 16:18:32.751636 proxyllm-0.2.1/proxyllm/config/__init__.py
--rw-r--r--   0        0        0    10342 2024-05-03 16:18:32.751767 proxyllm-0.2.1/proxyllm/config/internal_config.py
--rw-r--r--   0        0        0        0 2024-05-03 16:18:32.751830 proxyllm-0.2.1/proxyllm/data/__init__.py
--rw-r--r--   0        0        0  1083514 2024-05-03 16:18:32.755836 proxyllm-0.2.1/proxyllm/data/tokenizer-wiki.json
--rw-r--r--   0        0        0        0 2024-05-03 16:18:32.756489 proxyllm-0.2.1/proxyllm/provider/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 16:18:32.756551 proxyllm-0.2.1/proxyllm/provider/anthropic/__init__.py
--rw-r--r--   0        0        0     8526 2024-05-03 16:18:32.757264 proxyllm-0.2.1/proxyllm/provider/anthropic/claude.py
--rw-r--r--   0        0        0     1475 2024-05-03 16:18:32.757552 proxyllm-0.2.1/proxyllm/provider/base.py
--rw-r--r--   0        0        0        0 2024-05-03 16:18:32.757617 proxyllm-0.2.1/proxyllm/provider/cohere/__init__.py
--rw-r--r--   0        0        0     7911 2024-05-03 16:18:32.758035 proxyllm-0.2.1/proxyllm/provider/cohere/cohere.py
--rw-r--r--   0        0        0        0 2024-05-03 16:18:32.758076 proxyllm-0.2.1/proxyllm/provider/google/__init__.py
--rw-r--r--   0        0        0    15887 2024-05-03 16:18:32.758503 proxyllm-0.2.1/proxyllm/provider/google/vertexai.py
--rw-r--r--   0        0        0        0 2024-05-03 16:18:32.758541 proxyllm-0.2.1/proxyllm/provider/huggingface/__init__.py
--rw-r--r--   0        0        0    11554 2024-05-03 16:18:32.758917 proxyllm-0.2.1/proxyllm/provider/huggingface/llama2.py
--rw-r--r--   0        0        0        0 2024-05-03 16:18:32.758962 proxyllm-0.2.1/proxyllm/provider/mistral/__init__.py
--rw-r--r--   0        0        0     7904 2024-05-03 16:18:32.759126 proxyllm-0.2.1/proxyllm/provider/mistral/mistral.py
--rw-r--r--   0        0        0        0 2024-05-03 16:18:32.759164 proxyllm-0.2.1/proxyllm/provider/openai/__init__.py
--rw-r--r--   0        0        0     8744 2024-05-03 16:18:32.759483 proxyllm-0.2.1/proxyllm/provider/openai/chatgpt.py
--rw-r--r--   0        0        0    26068 2024-05-03 16:18:32.759795 proxyllm-0.2.1/proxyllm/proxyllm.py
--rw-r--r--   0        0        0        0 2024-05-03 16:18:32.759852 proxyllm-0.2.1/proxyllm/utils/__init__.py
--rw-r--r--   0        0        0     1424 2024-05-03 16:18:32.760373 proxyllm-0.2.1/proxyllm/utils/categorization.py
--rw-r--r--   0        0        0     1299 2024-05-03 16:18:32.760440 proxyllm-0.2.1/proxyllm/utils/cost.py
--rw-r--r--   0        0        0     1701 2024-05-03 16:18:32.761037 proxyllm-0.2.1/proxyllm/utils/enums.py
--rw-r--r--   0        0        0      234 2024-05-03 16:18:32.761117 proxyllm-0.2.1/proxyllm/utils/exceptions/llmproxy_client.py
--rw-r--r--   0        0        0     1462 2024-05-03 16:18:32.761676 proxyllm-0.2.1/proxyllm/utils/exceptions/provider.py
--rw-r--r--   0        0        0     6045 2024-05-03 16:18:32.762181 proxyllm-0.2.1/proxyllm/utils/proxy_logger.py
--rw-r--r--   0        0        0     1382 2024-05-03 16:18:32.762480 proxyllm-0.2.1/proxyllm/utils/sorting.py
--rw-r--r--   0        0        0     3235 2024-05-03 16:18:32.762552 proxyllm-0.2.1/proxyllm/utils/timeout_function.py
--rw-r--r--   0        0        0     1556 2024-05-03 16:18:32.762654 proxyllm-0.2.1/proxyllm/utils/tokenizer.py
--rw-r--r--   0        0        0      952 2024-05-03 16:26:19.835916 proxyllm-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    10380 1970-01-01 00:00:00.000000 proxyllm-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-03 16:18:32.748021 proxyllm-0.2.2/LICENSE
+-rw-r--r--   0        0        0     9607 2024-05-24 01:07:16.558811 proxyllm-0.2.2/README.md
+-rw-r--r--   0        0        0       39 2024-05-03 16:18:32.751240 proxyllm-0.2.2/proxyllm/__init__.py
+-rw-r--r--   0        0        0      795 2024-05-03 16:18:32.751576 proxyllm-0.2.2/proxyllm/cli.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:18:32.751636 proxyllm-0.2.2/proxyllm/config/__init__.py
+-rw-r--r--   0        0        0    10926 2024-05-24 02:03:50.114536 proxyllm-0.2.2/proxyllm/config/internal_config.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:18:32.751830 proxyllm-0.2.2/proxyllm/data/__init__.py
+-rw-r--r--   0        0        0  1083514 2024-05-03 16:18:32.755836 proxyllm-0.2.2/proxyllm/data/tokenizer-wiki.json
+-rw-r--r--   0        0        0        0 2024-05-03 16:18:32.756489 proxyllm-0.2.2/proxyllm/provider/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:18:32.756551 proxyllm-0.2.2/proxyllm/provider/anthropic/__init__.py
+-rw-r--r--   0        0        0     8526 2024-05-03 16:18:32.757264 proxyllm-0.2.2/proxyllm/provider/anthropic/claude.py
+-rw-r--r--   0        0        0     1475 2024-05-03 16:18:32.757552 proxyllm-0.2.2/proxyllm/provider/base.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:18:32.757617 proxyllm-0.2.2/proxyllm/provider/cohere/__init__.py
+-rw-r--r--   0        0        0     8256 2024-05-24 02:03:50.114809 proxyllm-0.2.2/proxyllm/provider/cohere/cohere.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:18:32.758076 proxyllm-0.2.2/proxyllm/provider/google/__init__.py
+-rw-r--r--   0        0        0    15887 2024-05-03 16:18:32.758503 proxyllm-0.2.2/proxyllm/provider/google/vertexai.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:18:32.758541 proxyllm-0.2.2/proxyllm/provider/huggingface/__init__.py
+-rw-r--r--   0        0        0    11554 2024-05-03 16:18:32.758917 proxyllm-0.2.2/proxyllm/provider/huggingface/llama2.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:18:32.758962 proxyllm-0.2.2/proxyllm/provider/mistral/__init__.py
+-rw-r--r--   0        0        0     7904 2024-05-24 01:45:34.813280 proxyllm-0.2.2/proxyllm/provider/mistral/mistral.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:18:32.759164 proxyllm-0.2.2/proxyllm/provider/openai/__init__.py
+-rw-r--r--   0        0        0     9685 2024-05-24 02:03:50.115053 proxyllm-0.2.2/proxyllm/provider/openai/chatgpt.py
+-rw-r--r--   0        0        0    26068 2024-05-24 01:45:34.926018 proxyllm-0.2.2/proxyllm/proxyllm.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:18:32.759852 proxyllm-0.2.2/proxyllm/utils/__init__.py
+-rw-r--r--   0        0        0     1424 2024-05-03 16:18:32.760373 proxyllm-0.2.2/proxyllm/utils/categorization.py
+-rw-r--r--   0        0        0     1299 2024-05-03 16:18:32.760440 proxyllm-0.2.2/proxyllm/utils/cost.py
+-rw-r--r--   0        0        0     1701 2024-05-03 16:18:32.761037 proxyllm-0.2.2/proxyllm/utils/enums.py
+-rw-r--r--   0        0        0      234 2024-05-03 16:18:32.761117 proxyllm-0.2.2/proxyllm/utils/exceptions/llmproxy_client.py
+-rw-r--r--   0        0        0     1462 2024-05-03 16:18:32.761676 proxyllm-0.2.2/proxyllm/utils/exceptions/provider.py
+-rw-r--r--   0        0        0     6045 2024-05-03 16:18:32.762181 proxyllm-0.2.2/proxyllm/utils/proxy_logger.py
+-rw-r--r--   0        0        0     1382 2024-05-03 16:18:32.762480 proxyllm-0.2.2/proxyllm/utils/sorting.py
+-rw-r--r--   0        0        0     3235 2024-05-03 16:18:32.762552 proxyllm-0.2.2/proxyllm/utils/timeout_function.py
+-rw-r--r--   0        0        0     1556 2024-05-03 16:18:32.762654 proxyllm-0.2.2/proxyllm/utils/tokenizer.py
+-rw-r--r--   0        0        0      953 2024-05-24 02:03:50.115288 proxyllm-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    10383 1970-01-01 00:00:00.000000 proxyllm-0.2.2/PKG-INFO
```

### Comparing `proxyllm-0.2.1/LICENSE` & `proxyllm-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `proxyllm-0.2.1/README.md` & `proxyllm-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `proxyllm-0.2.1/proxyllm/cli.py` & `proxyllm-0.2.2/proxyllm/cli.py`

 * *Files identical despite different names*

### Comparing `proxyllm-0.2.1/proxyllm/config/internal_config.py` & `proxyllm-0.2.2/proxyllm/config/internal_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,26 @@
 from typing import Any, Dict, List
 
 internal_config: List[Dict[str, Any]] = [
     {
         "provider": "OpenAI",
         "adapter_path": "proxyllm.provider.openai.chatgpt.OpenAIAdapter",
         "models": [
+            {
+                "name": "gpt-4-turbo",
+                "cost_per_token_input": 10e-06,
+                "cost_per_token_output": 30e-06,
+                "elo": 1287,
+            },
+            {
+                "name": "gpt-4o",
+                "cost_per_token_input": 5e-06,
+                "cost_per_token_output": 15e-06,
+                "elo": 1287,
+            },
             # GPT-4 Turbo
             {
                 "name": "gpt-4-0125-preview",
                 "cost_per_token_input": 10e-06,
                 "cost_per_token_output": 30e-06,
                 "elo": 1248,
             },
@@ -83,15 +95,15 @@
                 "cost_per_token_output": 4e-06,
                 "elo": 1114,  # assumed elo is the same for gpt-3.5-turbo-0613
             },
             {
                 "name": "gpt-3.5-turbo-0301",
                 "cost_per_token_input": 1.5e-06,
                 "cost_per_token_output": 2e-06,
-                "elo": 0,  # no data for this model
+                "elo": 499,  # no data for this model
             },
         ],
     },
     {
         "provider": "Llama2",
         "adapter_path": "proxyllm.provider.huggingface.llama2.Llama2Adapter",
         "models": [
@@ -170,14 +182,20 @@
         ],
     },
     {
         "provider": "Cohere",
         "adapter_path": "proxyllm.provider.cohere.cohere.CohereAdapter",
         "models": [
             {
+                "name": "command-r-plus",
+                "cost_per_token_input": 3.0e-06,
+                "cost_per_token_output": 15.0e-06,
+                "elo": 1188,
+            },
+            {
                 "name": "command-r",
                 "cost_per_token_input": 0.5e-06,
                 "cost_per_token_output": 1.5e-06,
                 "elo": 1120,  # approximated, should have a similar elo rating to mixtral-8x7b-instruct-v0.1
             },
             {
                 "name": "command",
```

### Comparing `proxyllm-0.2.1/proxyllm/data/tokenizer-wiki.json` & `proxyllm-0.2.2/proxyllm/data/tokenizer-wiki.json`

 * *Files identical despite different names*

### Comparing `proxyllm-0.2.1/proxyllm/provider/anthropic/claude.py` & `proxyllm-0.2.2/proxyllm/provider/anthropic/claude.py`

 * *Files identical despite different names*

### Comparing `proxyllm-0.2.1/proxyllm/provider/base.py` & `proxyllm-0.2.2/proxyllm/provider/base.py`

 * *Files identical despite different names*

### Comparing `proxyllm-0.2.1/proxyllm/provider/cohere/cohere.py` & `proxyllm-0.2.2/proxyllm/provider/cohere/cohere.py`

 * *Files 9% similar despite different names*

```diff
@@ -65,14 +65,26 @@
             "Conversational AI Task": 1,
             "Educational Applications Task": 2,
             "Healthcare and Medical Task": 3,
             "Legal Task": 3,
             "Financial Task": 3,
             "Content Recommendation Task": 2,
         },
+        "command-r-plus": {
+            "Code Generation Task": 3,
+            "Text Generation Task": 3,
+            "Translation and Multilingual Applications Task": 3,
+            "Natural Language Processing Task": 4,
+            "Conversational AI Task": 3,
+            "Educational Applications Task": 3,
+            "Healthcare and Medical Task": 3,
+            "Legal Task": 3,
+            "Financial Task": 3,
+            "Content Recommendation Task": 3,
+        },
     }
 }
 
 # Mapping from role names to Cohere's format
 ROLE_NAME_TO_REP = {
     "user": "USER",
     "assistant": "CHATBOT",
@@ -124,15 +136,15 @@
 
         Returns:
             Dict[str, Any] | None: The model's text response and chat history, or None if an error occurs.
 
         Raises:
             CohereException: If an error occurs during the API request.
         """
-        from cohere import Client, CohereError
+        from cohere import Client
 
         try:
             if chat_history is None:
                 chat_history = []
 
             # Convert the proxy chat history into a format that Cohere can process
             cohere_chat_history = self.format_chat_history(chat_history)
@@ -151,16 +163,14 @@
             chat_history.append({"role": "assistant", "content": response.text})
 
             provider_response = {
                 "response": response.text,
                 "chat_history": chat_history,
             }
 
-        except CohereError as e:
-            raise CohereException(exception=str(e), error_type="CohereError") from e
         except Exception as e:
             raise CohereException(
                 exception=str(e), error_type="Unknown Cohere Error"
             ) from e
 
         return provider_response or None
```

### Comparing `proxyllm-0.2.1/proxyllm/provider/google/vertexai.py` & `proxyllm-0.2.2/proxyllm/provider/google/vertexai.py`

 * *Files identical despite different names*

### Comparing `proxyllm-0.2.1/proxyllm/provider/huggingface/llama2.py` & `proxyllm-0.2.2/proxyllm/provider/huggingface/llama2.py`

 * *Files identical despite different names*

### Comparing `proxyllm-0.2.1/proxyllm/provider/mistral/mistral.py` & `proxyllm-0.2.2/proxyllm/provider/mistral/mistral.py`

 * *Files identical despite different names*

### Comparing `proxyllm-0.2.1/proxyllm/provider/openai/chatgpt.py` & `proxyllm-0.2.2/proxyllm/provider/openai/chatgpt.py`

 * *Files 12% similar despite different names*

```diff
@@ -89,14 +89,38 @@
             "Conversational AI Task": 1,
             "Educational Applications Task": 1,
             "Healthcare and Medical Task": 2,
             "Legal Task": 2,
             "Financial Task": 2,
             "Content Recommendation Task": 1,
         },
+        "gpt-4-turbo": {
+            "Code Generation Task": 3,
+            "Text Generation Task": 4,
+            "Translation and Multilingual Applications Task": 4,
+            "Natural Language Processing Task": 5,
+            "Conversational AI Task": 3,
+            "Educational Applications Task": 3,
+            "Healthcare and Medical Task": 3,
+            "Legal Task": 3,
+            "Financial Task": 4,
+            "Content Recommendation Task": 5,
+        },
+        "gpt-4o": {
+            "Code Generation Task": 4,
+            "Text Generation Task": 4,
+            "Translation and Multilingual Applications Task": 4,
+            "Natural Language Processing Task": 5,
+            "Conversational AI Task": 4,
+            "Educational Applications Task": 3,
+            "Healthcare and Medical Task": 3,
+            "Legal Task": 3,
+            "Financial Task": 4,
+            "Content Recommendation Task": 5,
+        },
     }
 }
 
 
 class OpenAIAdapter(BaseAdapter):
     """
     Adapter class for interacting with OpenAI's language models.
```

### Comparing `proxyllm-0.2.1/proxyllm/proxyllm.py` & `proxyllm-0.2.2/proxyllm/proxyllm.py`

 * *Files identical despite different names*

### Comparing `proxyllm-0.2.1/proxyllm/utils/categorization.py` & `proxyllm-0.2.2/proxyllm/utils/categorization.py`

 * *Files identical despite different names*

### Comparing `proxyllm-0.2.1/proxyllm/utils/cost.py` & `proxyllm-0.2.2/proxyllm/utils/cost.py`

 * *Files identical despite different names*

### Comparing `proxyllm-0.2.1/proxyllm/utils/enums.py` & `proxyllm-0.2.2/proxyllm/utils/enums.py`

 * *Files identical despite different names*

### Comparing `proxyllm-0.2.1/proxyllm/utils/exceptions/provider.py` & `proxyllm-0.2.2/proxyllm/utils/exceptions/provider.py`

 * *Files identical despite different names*

### Comparing `proxyllm-0.2.1/proxyllm/utils/proxy_logger.py` & `proxyllm-0.2.2/proxyllm/utils/proxy_logger.py`

 * *Files identical despite different names*

### Comparing `proxyllm-0.2.1/proxyllm/utils/sorting.py` & `proxyllm-0.2.2/proxyllm/utils/sorting.py`

 * *Files identical despite different names*

### Comparing `proxyllm-0.2.1/proxyllm/utils/timeout_function.py` & `proxyllm-0.2.2/proxyllm/utils/timeout_function.py`

 * *Files identical despite different names*

### Comparing `proxyllm-0.2.1/proxyllm/utils/tokenizer.py` & `proxyllm-0.2.2/proxyllm/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `proxyllm-0.2.1/PKG-INFO` & `proxyllm-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: proxyllm
-Version: 0.2.1
+Version: 0.2.2
 Summary: LLM Proxy to reduce cost and complexity of using multiple LLMs
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: anthropic (>=0.20.0,<0.21.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: cohere (>=4.27,<5.0)
+Requires-Dist: cohere (>=5.5.3,<6.0.0)
 Requires-Dist: google-cloud-aiplatform (>=1.35.0,<2.0.0)
 Requires-Dist: mistralai (>=0.1.8,<0.2.0)
 Requires-Dist: openai (>=1.11.1,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: torch (>=2.2.1,<3.0.0)
 Requires-Dist: transformers (>=4.38.2,<5.0.0)
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: proxyllm Version: 0.2.1 Summary: LLM Proxy to
+Metadata-Version: 2.1 Name: proxyllm Version: 0.2.2 Summary: LLM Proxy to
 reduce cost and complexity of using multiple LLMs Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: anthropic (>=0.20.0,<0.21.0) Requires-Dist: click
-(>=8.1.7,<9.0.0) Requires-Dist: cohere (>=4.27,<5.0) Requires-Dist: google-
+(>=8.1.7,<9.0.0) Requires-Dist: cohere (>=5.5.3,<6.0.0) Requires-Dist: google-
 cloud-aiplatform (>=1.35.0,<2.0.0) Requires-Dist: mistralai (>=0.1.8,<0.2.0)
 Requires-Dist: openai (>=1.11.1,<2.0.0) Requires-Dist: python-dotenv
 (>=1.0.0,<2.0.0) Requires-Dist: tiktoken (>=0.6.0,<0.7.0) Requires-Dist: torch
 (>=2.2.1,<3.0.0) Requires-Dist: transformers (>=4.38.2,<5.0.0) Description-
 Content-Type: text/markdown
                               ******** LLLLMM PPrrooxxyy ********
    A low-code solution to efficiently manage multiple large language models
```

