# Comparing `tmp/okahu_observability-0.0.4.tar.gz` & `tmp/okahu_observability-0.0.5.tar.gz`

## Comparing `okahu_observability-0.0.4.tar` & `okahu_observability-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 okahu_observability-0.0.4/logprobs_sample.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 okahu_observability-0.0.4/src/okahu_apptrace/__init__.py
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 okahu_observability-0.0.4/src/okahu_apptrace/exporter.py
--rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 okahu_observability-0.0.4/src/okahu_apptrace/instrumentor.py
--rw-r--r--   0        0        0     7206 2020-02-02 00:00:00.000000 okahu_observability-0.0.4/src/okahu_apptrace/utils.py
--rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 okahu_observability-0.0.4/src/okahu_apptrace/wrapper.py
--rw-r--r--   0        0        0     9128 2020-02-02 00:00:00.000000 okahu_observability-0.0.4/storage/default__vector_store.json
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 okahu_observability-0.0.4/storage/docstore.json
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 okahu_observability-0.0.4/storage/graph_store.json
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 okahu_observability-0.0.4/storage/image__vector_store.json
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 okahu_observability-0.0.4/storage/index_store.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 okahu_observability-0.0.4/.gitignore
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 okahu_observability-0.0.4/LICENSE
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 okahu_observability-0.0.4/README.md
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 okahu_observability-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 okahu_observability-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 okahu_observability-0.0.5/src/okahu_apptrace/__init__.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 okahu_observability-0.0.5/src/okahu_apptrace/exporter.py
+-rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 okahu_observability-0.0.5/src/okahu_apptrace/instrumentor.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 okahu_observability-0.0.5/src/okahu_apptrace/utils.py
+-rw-r--r--   0        0        0     8066 2020-02-02 00:00:00.000000 okahu_observability-0.0.5/src/okahu_apptrace/wrap_common.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 okahu_observability-0.0.5/src/okahu_apptrace/wrapper.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 okahu_observability-0.0.5/src/okahu_apptrace/haystack/README.md
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 okahu_observability-0.0.5/src/okahu_apptrace/haystack/__init__.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 okahu_observability-0.0.5/src/okahu_apptrace/haystack/wrap_node.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 okahu_observability-0.0.5/src/okahu_apptrace/haystack/wrap_openai.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 okahu_observability-0.0.5/src/okahu_apptrace/haystack/wrap_pipeline.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 okahu_observability-0.0.5/src/okahu_apptrace/langchain/__init__.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 okahu_observability-0.0.5/src/okahu_apptrace/llamaindex/__init__.py
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 okahu_observability-0.0.5/.gitignore
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 okahu_observability-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 okahu_observability-0.0.5/README.md
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 okahu_observability-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 okahu_observability-0.0.5/PKG-INFO
```

### Comparing `okahu_observability-0.0.4/src/okahu_apptrace/exporter.py` & `okahu_observability-0.0.5/src/okahu_apptrace/exporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright (C) Okahu Inc 2023-2024. All rights reserved
+
 
 import json
 import logging
 import os
 from typing import Optional, Sequence
 import requests
 from opentelemetry.sdk.trace.export import SpanExporter, SpanExportResult
```

### Comparing `okahu_observability-0.0.4/src/okahu_apptrace/instrumentor.py` & `okahu_observability-0.0.5/src/okahu_apptrace/instrumentor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright (C) Okahu Inc 2023-2024. All rights reserved
+
 import logging
 from typing import Collection,List
 from wrapt import wrap_function_wrapper
 from opentelemetry.trace import get_tracer
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.instrumentation.utils import unwrap
 from opentelemetry.sdk.trace import TracerProvider
```

### Comparing `okahu_observability-0.0.4/src/okahu_apptrace/utils.py` & `okahu_observability-0.0.5/src/okahu_apptrace/wrap_common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,29 @@
+# Copyright (C) Okahu Inc 2023-2024. All rights reserved
+
 import logging
 import os
 from opentelemetry.trace import Tracer, Span
 
+from okahu_apptrace.utils import with_tracer_wrapper
+
 logger = logging.getLogger(__name__)
 WORKFLOW_TYPE_KEY = "workflow_type"
+CONTEXT_INPUT_KEY = "workflow_context_input"
+CONTEXT_OUTPUT_KEY = "workflow_context_output"
 PROMPT_INPUT_KEY = "workflow_input"
 PROMPT_OUTPUT_KEY = "workflow_output"
 
 WORKFLOW_TYPE_MAP = {
     "llama_index": "workflow.llamaindex",
-    "langchain": "workflow.langchain"
+    "langchain": "workflow.langchain",
+    "haystack": "workflow.haystack"
 }
 
-def _with_tracer_wrapper(func):
-    """Helper for providing tracer for wrapper functions."""
-
-    def _with_tracer(tracer, to_wrap):
-        def wrapper(wrapped, instance, args, kwargs):
-            return func(tracer, to_wrap, wrapped, instance, args, kwargs)
-
-        return wrapper
-
-    return _with_tracer
-
-@_with_tracer_wrapper
+@with_tracer_wrapper
 def task_wrapper(tracer: Tracer, to_wrap, wrapped, instance, args, kwargs):
     """Instruments and calls every function defined in TO_WRAP."""
 
     # Some Langchain objects are wrapped elsewhere, so we ignore them here
     if instance.__class__.__name__ in ("AgentExecutor"):
         return wrapped(*args, **kwargs)
     
@@ -39,25 +35,27 @@
         name = f"langchain.task.{instance.__class__.__name__}"
     kind = to_wrap.get("kind")
     
     with tracer.start_as_current_span(name) as span:
         if is_root_span(span):
             update_span_with_prompt_input(to_wrap=to_wrap, wrapped_args=args, span=span)
 
+        update_span_with_context_input(to_wrap=to_wrap, wrapped_args=args, span=span)
         return_value = wrapped(*args, **kwargs)
+        update_span_with_context_output(to_wrap=to_wrap, return_value=return_value, span=span)
 
         if is_root_span(span):
             workflow_name = span.resource.attributes.get("service.name")
             span.set_attribute("workflow_name",workflow_name)
             update_span_with_prompt_output(to_wrap=to_wrap, wrapped_args=return_value, span=span)
             update_workflow_type(to_wrap, span)
 
     return return_value
 
-@_with_tracer_wrapper
+@with_tracer_wrapper
 async def atask_wrapper(tracer, to_wrap, wrapped, instance, args, kwargs):
     """Instruments and calls every function defined in TO_WRAP."""
 
     # Some Langchain objects are wrapped elsewhere, so we ignore them here
     if instance.__class__.__name__ in ("AgentExecutor"):
         return wrapped(*args, **kwargs)
 
@@ -69,15 +67,15 @@
         name = f"langchain.task.{instance.__class__.__name__}"
     kind = to_wrap.get("kind")
     with tracer.start_as_current_span(name) as span:
         return_value = await wrapped(*args, **kwargs)
 
     return return_value
 
-@_with_tracer_wrapper
+@with_tracer_wrapper
 async def allm_wrapper(tracer, to_wrap, wrapped, instance, args, kwargs):
     # Some Langchain objects are wrapped elsewhere, so we ignore them here
     if instance.__class__.__name__ in ("AgentExecutor"):
         return wrapped(*args, **kwargs)
 
     if hasattr(instance, "name") and instance.name:
         name = f"{to_wrap.get('span_name')}.{instance.name.lower()}"
@@ -89,15 +87,15 @@
     with tracer.start_as_current_span(name) as span:
         update_llm_endpoint(curr_span= span, instance=instance)
         
         return_value = await wrapped(*args, **kwargs)
 
     return return_value
 
-@_with_tracer_wrapper
+@with_tracer_wrapper
 def llm_wrapper(tracer: Tracer, to_wrap, wrapped, instance, args, kwargs):
     
     # Some Langchain objects are wrapped elsewhere, so we ignore them here
     if instance.__class__.__name__ in ("AgentExecutor"):
         return wrapped(*args, **kwargs)
 
     if hasattr(instance, "name") and instance.name:
@@ -162,14 +160,29 @@
 def update_workflow_type(to_wrap, span: Span):
     package_name = to_wrap.get('package')
 
     for (package, workflow_type) in WORKFLOW_TYPE_MAP.items():
         if(package_name is not None and package in package_name):
             span.set_attribute(WORKFLOW_TYPE_KEY, workflow_type)
 
+def update_span_with_context_input(to_wrap, wrapped_args ,span: Span):
+    package_name: str = to_wrap.get('package')
+    if("langchain_core.retrievers" in package_name):
+        input_arg_text = wrapped_args[0]
+        span.set_attribute(CONTEXT_INPUT_KEY, input_arg_text)
+    if("llama_index.core.indices.base_retriever" in package_name):
+        input_arg_text = wrapped_args[0].query_str
+        span.set_attribute(CONTEXT_INPUT_KEY, input_arg_text)
+
+def update_span_with_context_output(to_wrap, return_value ,span: Span):
+    package_name: str = to_wrap.get('package')
+    if("llama_index.core.indices.base_retriever" in package_name):
+        output_arg_text = return_value[0].text
+        span.set_attribute(CONTEXT_OUTPUT_KEY, output_arg_text)
+
 def update_span_with_prompt_input(to_wrap, wrapped_args ,span: Span):
     input_arg_text = wrapped_args[0]
     span.set_attribute(PROMPT_INPUT_KEY, input_arg_text)
 
 def update_span_with_prompt_output(to_wrap, wrapped_args ,span: Span):
     package_name: str = to_wrap.get('package')
     if type(wrapped_args) == str:
```

### Comparing `okahu_observability-0.0.4/src/okahu_apptrace/wrapper.py` & `okahu_observability-0.0.5/src/okahu_apptrace/langchain/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,10 @@
-from okahu_apptrace.utils import task_wrapper, atask_wrapper, llm_wrapper, allm_wrapper
+# Copyright (C) Okahu Inc 2023-2024. All rights reserved
 
-class WrapperMethod:
-    def __init__(
-            self,
-            package: str,
-            object: str,
-            method: str,
-            span_name: str = None,
-            wrapper = task_wrapper
-            ):
-        self.package = package
-        self.object = object
-        self.method = method
-        self.span_name = span_name
-        self.wrapper = wrapper
-        
+from okahu_apptrace.wrap_common import allm_wrapper, atask_wrapper, llm_wrapper, task_wrapper
 
 LANGCHAIN_METHODS = [
     {
         "package": "langchain.prompts.base",
         "object": "BasePromptTemplate",
         "method": "invoke",
         "wrapper": task_wrapper,
@@ -103,55 +89,7 @@
         "object": "RunnableParallel",
         "method": "ainvoke",
         "span_name": "langchain.workflow",
         "wrapper": atask_wrapper,
     },
     
 ]
-
-LLAMAINDEX_METHODS = [
-    {
-        "package": "llama_index.core.indices.base_retriever",
-        "object": "BaseRetriever",
-        "method": "retrieve",
-        "span_name": "llamaindex.retrieve",
-        "wrapper": task_wrapper
-    },
-    {
-        "package": "llama_index.core.indices.base_retriever",
-        "object": "BaseRetriever",
-        "method": "aretrieve",
-        "span_name": "llamaindex.retrieve",
-        "wrapper": atask_wrapper
-    },
-    {
-        "package": "llama_index.core.base.base_query_engine",
-        "object": "BaseQueryEngine",
-        "method": "query",
-        "span_name": "llamaindex.query",
-        "wrapper": task_wrapper,
-    },
-    {
-        "package": "llama_index.core.base.base_query_engine",
-        "object": "BaseQueryEngine",
-        "method": "aquery",
-        "span_name": "llamaindex.query",
-        "wrapper": atask_wrapper,
-    },
-    {
-        "package": "llama_index.core.llms.custom",
-        "object": "CustomLLM",
-        "method": "chat",
-        "span_name": "llamaindex.llmchat",
-        "wrapper": task_wrapper,
-    },
-    {
-        "package": "llama_index.core.llms.custom",
-        "object": "CustomLLM",
-        "method": "achat",
-        "span_name": "llamaindex.llmchat",
-        "wrapper": atask_wrapper,
-    }
-]
-
-METHODS_LIST = LANGCHAIN_METHODS + LLAMAINDEX_METHODS
-
```

### Comparing `okahu_observability-0.0.4/.gitignore` & `okahu_observability-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `okahu_observability-0.0.4/LICENSE` & `okahu_observability-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `okahu_observability-0.0.4/README.md` & `okahu_observability-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `okahu_observability-0.0.4/pyproject.toml` & `okahu_observability-0.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "okahu-observability"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Okahu Inc.", email="okahu-pypi@okahu.ai" },
 ]
 description = "package with okahu opentelemetry"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `okahu_observability-0.0.4/PKG-INFO` & `okahu_observability-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: okahu-observability
-Version: 0.0.4
+Version: 0.0.5
 Summary: package with okahu opentelemetry
 Project-URL: Homepage, https://github.com/okahu/demo-repository
 Project-URL: Issues, https://github.com/okahu/demo-repository/issues
 Author-email: "Okahu Inc." <okahu-pypi@okahu.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

