# Comparing `tmp/cohere_haystack-1.0.0.tar.gz` & `tmp/cohere_haystack-1.1.0.tar.gz`

## Comparing `cohere_haystack-1.0.0.tar` & `cohere_haystack-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/examples/cohere_ranker_in_a_pipeline.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/pydoc/config.yml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/src/haystack_integrations/components/embedders/cohere/__init__.py
--rw-r--r--   0        0        0     8081 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/src/haystack_integrations/components/embedders/cohere/document_embedder.py
--rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/src/haystack_integrations/components/embedders/cohere/text_embedder.py
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/src/haystack_integrations/components/embedders/cohere/utils.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/src/haystack_integrations/components/generators/cohere/__init__.py
--rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/src/haystack_integrations/components/generators/cohere/generator.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/src/haystack_integrations/components/generators/cohere/chat/__init__.py
--rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/src/haystack_integrations/components/generators/cohere/chat/chat_generator.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/src/haystack_integrations/components/rankers/cohere/__init__.py
--rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/src/haystack_integrations/components/rankers/cohere/ranker.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0    11735 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/tests/test_cohere_chat_generator.py
--rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/tests/test_cohere_generators.py
--rw-r--r--   0        0        0    15463 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/tests/test_cohere_ranker.py
--rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/tests/test_document_embedder.py
--rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/tests/test_text_embedder.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/README.md
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 cohere_haystack-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/examples/cohere_ranker_in_a_pipeline.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/pydoc/config.yml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/src/haystack_integrations/components/embedders/cohere/__init__.py
+-rw-r--r--   0        0        0     8081 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/src/haystack_integrations/components/embedders/cohere/document_embedder.py
+-rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/src/haystack_integrations/components/embedders/cohere/text_embedder.py
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/src/haystack_integrations/components/embedders/cohere/utils.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/src/haystack_integrations/components/generators/cohere/__init__.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/src/haystack_integrations/components/generators/cohere/generator.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/src/haystack_integrations/components/generators/cohere/chat/__init__.py
+-rw-r--r--   0        0        0    10780 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/src/haystack_integrations/components/generators/cohere/chat/chat_generator.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/src/haystack_integrations/components/rankers/cohere/__init__.py
+-rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/src/haystack_integrations/components/rankers/cohere/ranker.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0    11735 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/tests/test_cohere_chat_generator.py
+-rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/tests/test_cohere_generators.py
+-rw-r--r--   0        0        0    15463 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/tests/test_cohere_ranker.py
+-rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/tests/test_document_embedder.py
+-rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/tests/test_text_embedder.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/README.md
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 cohere_haystack-1.1.0/PKG-INFO
```

### Comparing `cohere_haystack-1.0.0/examples/cohere_ranker_in_a_pipeline.py` & `cohere_haystack-1.1.0/examples/cohere_ranker_in_a_pipeline.py`

 * *Files identical despite different names*

### Comparing `cohere_haystack-1.0.0/pydoc/config.yml` & `cohere_haystack-1.1.0/pydoc/config.yml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     expression:
     documented_only: true
     do_not_filter_modules: false
     skip_empty_modules: true
   - type: smart
   - type: crossref
 renderer:
-  type: haystack_pydoc_tools.renderers.ReadmePreviewRenderer
+  type: haystack_pydoc_tools.renderers.ReadmeIntegrationRenderer
   excerpt: Cohere integration for Haystack
   category_slug: integrations-api
   title: Cohere
   slug: integrations-cohere
   order: 50
   markdown:
     descriptive_class_title: false
```

### Comparing `cohere_haystack-1.0.0/src/haystack_integrations/components/embedders/cohere/document_embedder.py` & `cohere_haystack-1.1.0/src/haystack_integrations/components/embedders/cohere/document_embedder.py`

 * *Files identical despite different names*

### Comparing `cohere_haystack-1.0.0/src/haystack_integrations/components/embedders/cohere/text_embedder.py` & `cohere_haystack-1.1.0/src/haystack_integrations/components/embedders/cohere/text_embedder.py`

 * *Files identical despite different names*

### Comparing `cohere_haystack-1.0.0/src/haystack_integrations/components/embedders/cohere/utils.py` & `cohere_haystack-1.1.0/src/haystack_integrations/components/embedders/cohere/utils.py`

 * *Files identical despite different names*

### Comparing `cohere_haystack-1.0.0/src/haystack_integrations/components/generators/cohere/chat/chat_generator.py` & `cohere_haystack-1.1.0/src/haystack_integrations/components/generators/cohere/chat/chat_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,13 +220,13 @@
 
         total_tokens = cohere_response.meta.billed_units.input_tokens + cohere_response.meta.billed_units.output_tokens
         message.meta.update(
             {
                 "model": self.model,
                 "usage": total_tokens,
                 "index": 0,
-                "finish_reason": None,
+                "finish_reason": cohere_response.finish_reason,
                 "documents": cohere_response.documents,
                 "citations": cohere_response.citations,
             }
         )
         return message
```

### Comparing `cohere_haystack-1.0.0/src/haystack_integrations/components/rankers/cohere/ranker.py` & `cohere_haystack-1.1.0/src/haystack_integrations/components/rankers/cohere/ranker.py`

 * *Files identical despite different names*

### Comparing `cohere_haystack-1.0.0/tests/test_cohere_chat_generator.py` & `cohere_haystack-1.1.0/tests/test_cohere_chat_generator.py`

 * *Files identical despite different names*

### Comparing `cohere_haystack-1.0.0/tests/test_cohere_generators.py` & `cohere_haystack-1.1.0/tests/test_cohere_generators.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         assert data == {
             "type": "haystack_integrations.components.generators.cohere.generator.CohereGenerator",
             "init_parameters": {
                 "model": "command",
                 "api_key": {"env_vars": ["COHERE_API_KEY", "CO_API_KEY"], "strict": True, "type": "env_var"},
                 "streaming_callback": None,
                 "api_base_url": COHERE_API_URL,
+                "generation_kwargs": {},
             },
         }
 
     def test_to_dict_with_parameters(self, monkeypatch):
         monkeypatch.setenv("COHERE_API_KEY", "test-api-key")
         monkeypatch.setenv("CO_API_KEY", "fake-api-key")
         component = CohereGenerator(
@@ -65,19 +66,18 @@
             api_base_url="test-base-url",
         )
         data = component.to_dict()
         assert data == {
             "type": "haystack_integrations.components.generators.cohere.generator.CohereGenerator",
             "init_parameters": {
                 "model": "command-light",
-                "max_tokens": 10,
-                "some_test_param": "test-params",
                 "api_base_url": "test-base-url",
                 "api_key": {"env_vars": ["ENV_VAR"], "strict": False, "type": "env_var"},
                 "streaming_callback": "haystack.components.generators.utils.print_streaming_chunk",
+                "generation_kwargs": {},
             },
         }
 
     def test_to_dict_with_lambda_streaming_callback(self, monkeypatch):
         monkeypatch.setenv("COHERE_API_KEY", "test-api-key")
         component = CohereGenerator(
             model="command",
@@ -88,18 +88,17 @@
         )
         data = component.to_dict()
         assert data == {
             "type": "haystack_integrations.components.generators.cohere.generator.CohereGenerator",
             "init_parameters": {
                 "model": "command",
                 "streaming_callback": "tests.test_cohere_generators.<lambda>",
-                "api_key": {"env_vars": ["COHERE_API_KEY", "CO_API_KEY"], "strict": True, "type": "env_var"},
                 "api_base_url": "test-base-url",
-                "max_tokens": 10,
-                "some_test_param": "test-params",
+                "api_key": {"type": "env_var", "env_vars": ["COHERE_API_KEY", "CO_API_KEY"], "strict": True},
+                "generation_kwargs": {},
             },
         }
 
     def test_from_dict(self, monkeypatch):
         monkeypatch.setenv("COHERE_API_KEY", "fake-api-key")
         monkeypatch.setenv("CO_API_KEY", "fake-api-key")
         data = {
```

### Comparing `cohere_haystack-1.0.0/tests/test_cohere_ranker.py` & `cohere_haystack-1.1.0/tests/test_cohere_ranker.py`

 * *Files identical despite different names*

### Comparing `cohere_haystack-1.0.0/tests/test_document_embedder.py` & `cohere_haystack-1.1.0/tests/test_document_embedder.py`

 * *Files identical despite different names*

### Comparing `cohere_haystack-1.0.0/tests/test_text_embedder.py` & `cohere_haystack-1.1.0/tests/test_text_embedder.py`

 * *Files identical despite different names*

### Comparing `cohere_haystack-1.0.0/.gitignore` & `cohere_haystack-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cohere_haystack-1.0.0/LICENSE.txt` & `cohere_haystack-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cohere_haystack-1.0.0/README.md` & `cohere_haystack-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cohere_haystack-1.0.0/pyproject.toml` & `cohere_haystack-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cohere_haystack-1.0.0/PKG-INFO` & `cohere_haystack-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cohere-haystack
-Version: 1.0.0
+Version: 1.1.0
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/cohere#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/cohere
 Author-email: deepset GmbH <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

