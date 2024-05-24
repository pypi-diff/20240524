# Comparing `tmp/csa_ai_foundation_model_api_clients-0.1.8.tar.gz` & `tmp/csa_ai_foundation_model_api_clients-0.1.9.tar.gz`

## Comparing `csa_ai_foundation_model_api_clients-0.1.8.tar` & `csa_ai_foundation_model_api_clients-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     1437 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/TODO.md
--rwxr-xr-x   0        0        0      357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/manual-package-update.md
--rwxr-xr-x   0        0        0     1132 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/output-example.json
--rwxr-xr-x   0        0        0      486 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/setup-venv.sh
--rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/.github/workflows/release.yml
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/src/csa_ai_foundation_model_api_clients/__init__.py
--rwxr-xr-x   0        0        0     7683 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/src/csa_ai_foundation_model_api_clients/csa_ai_foundation_model_api_clients.py
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/src/csa_ai_foundation_model_api_clients/ai_client/__init__.py
--rwxr-xr-x   0        0        0     1792 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py
--rwxr-xr-x   0        0        0     1740 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/src/csa_ai_foundation_model_api_clients/ai_client/claude.py
--rwxr-xr-x   0        0        0     1721 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py
--rwxr-xr-x   0        0        0      724 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/tests/dev/ask-chatgpt-the-capital-of-france.py
--rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/tests/dev/ask-claude-the-capital-of-france.py
--rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/tests/dev/ask-gemini-the-capital-of-france.py
--rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/.gitignore
--rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/LICENSE
--rwxr-xr-x   0        0        0     2221 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/README.md
--rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1437 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.9/TODO.md
+-rwxr-xr-x   0        0        0      357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.9/manual-package-update.md
+-rwxr-xr-x   0        0        0     1132 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.9/output-example.json
+-rwxr-xr-x   0        0        0      486 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.9/setup-venv.sh
+-rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.9/.github/workflows/release.yml
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.9/src/csa_ai_foundation_model_api_clients/__init__.py
+-rwxr-xr-x   0        0        0     7683 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.9/src/csa_ai_foundation_model_api_clients/csa_ai_foundation_model_api_clients.py
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.9/src/csa_ai_foundation_model_api_clients/ai_client/__init__.py
+-rwxr-xr-x   0        0        0     1711 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.9/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py
+-rwxr-xr-x   0        0        0     1740 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.9/src/csa_ai_foundation_model_api_clients/ai_client/claude.py
+-rwxr-xr-x   0        0        0     1721 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.9/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py
+-rwxr-xr-x   0        0        0      724 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.9/tests/dev/ask-chatgpt-the-capital-of-france.py
+-rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.9/tests/dev/ask-claude-the-capital-of-france.py
+-rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.9/tests/dev/ask-gemini-the-capital-of-france.py
+-rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.9/.gitignore
+-rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.9/LICENSE
+-rwxr-xr-x   0        0        0     2221 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.9/README.md
+-rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.9/PKG-INFO
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.8/TODO.md` & `csa_ai_foundation_model_api_clients-0.1.9/TODO.md`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.8/output-example.json` & `csa_ai_foundation_model_api_clients-0.1.9/output-example.json`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.8/src/csa_ai_foundation_model_api_clients/csa_ai_foundation_model_api_clients.py` & `csa_ai_foundation_model_api_clients-0.1.9/src/csa_ai_foundation_model_api_clients/csa_ai_foundation_model_api_clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from csa_ai_foundation_model_api_clients.ai_client import claude, chatgpt, gemini
 
 class FoundationModelAPIClient:
     def __init__(self, *, model, api_key=None, system_prompt, system_prompt_type, user_prompt, user_prompt_type, user_data=None, user_data_type, output_file=None, temperature=None, max_tokens=None):
         #
         # Increment this when updating the model
         #
-        self.csa_ai_foundation_model_api_clients_version = "0.1.8"
+        self.csa_ai_foundation_model_api_clients_version = "0.1.9"
         self.model = model
         self.api_key = api_key or self.get_model_api_key()
         self.model_name = self.get_model_mapping()
         self.system_prompt = system_prompt
         self.system_prompt_type = system_prompt_type
         self.user_prompt = user_prompt
         self.user_prompt_type = user_prompt_type
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.8/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py` & `csa_ai_foundation_model_api_clients-0.1.9/src/csa_ai_foundation_model_api_clients/ai_client/claude.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,57 @@
 #!/usr/bin/env python3
 
-import openai
+import anthropic
 import datetime
 
 def generate_response(model_name, api_key, system_prompt, user_prompt, **kwargs):
     TIME_START = datetime.datetime.now()
 
-    openai.api_key = api_key
+    client = anthropic.Anthropic(api_key=api_key)
 
     temperature = kwargs.get('temperature', 1)
     max_tokens = kwargs.get('max_tokens', 4096)
 
-    completion = openai.chat.completions.create(
-        model=model_name,
+    completion = client.messages.create(
+        model=model_name,        
         temperature=temperature,
         max_tokens=max_tokens,
-        #
-        # Set interactive=false
-        #
-        interactive="false",
+        system=system_prompt,
         messages=[
-            {"role": "system", "content": system_prompt},
             {"role": "user", "content": user_prompt}
-        ]
+        ],
     )
 
     TIME_FINISHED = datetime.datetime.now()
     duration = TIME_START - TIME_FINISHED
     TIME_TO_RUN = duration.total_seconds()
 
     try:
-        tokens_input = completion.usage.prompt_tokens
-        tokens_output = completion.usage.completion_tokens
-        total_tokens = completion.usage.total_tokens
+        tokens_input = completion.usage.input_tokens
+        tokens_output = completion.usage.output_tokens
+        total_tokens = completion.usage.input_tokens + completion.usage.output_tokens
     except AttributeError:
         tokens_input = tokens_output = total_tokens = None
     
     try:
-        response_message = completion.choices[0].message.content
+        response_message = completion.content[0].text
         status = "success"
     except AttributeError:
         response_message = None
         status = "error"
 
     api_response = {
-        "status": "success",
+        "status": status,
         "model_name": model_name,
         "temperature": temperature,
         "ai_query_time": TIME_START.isoformat(),
         "ai_response_time": TIME_FINISHED.isoformat(),
         "ai_runtime": TIME_TO_RUN,
         "tokens_input": tokens_input,
         "tokens_output": tokens_output,
         "tokens_total": total_tokens,
         "ai_response_http_status_code": None,
-        "ai_response_stop_reason": None,
+        "ai_response_stop_reason": completion.stop_reason,
         "ai_response_data": response_message
     }
 
     return api_response
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.8/src/csa_ai_foundation_model_api_clients/ai_client/claude.py` & `csa_ai_foundation_model_api_clients-0.1.9/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 #!/usr/bin/env python3
 
-import anthropic
+import openai
 import datetime
 
 def generate_response(model_name, api_key, system_prompt, user_prompt, **kwargs):
     TIME_START = datetime.datetime.now()
 
-    client = anthropic.Anthropic(api_key=api_key)
+    openai.api_key = api_key
 
     temperature = kwargs.get('temperature', 1)
     max_tokens = kwargs.get('max_tokens', 4096)
 
-    completion = client.messages.create(
-        model=model_name,        
+    completion = openai.chat.completions.create(
+        model=model_name,
         temperature=temperature,
         max_tokens=max_tokens,
-        system=system_prompt,
         messages=[
+            {"role": "system", "content": system_prompt},
             {"role": "user", "content": user_prompt}
-        ],
+        ]
     )
 
     TIME_FINISHED = datetime.datetime.now()
     duration = TIME_START - TIME_FINISHED
     TIME_TO_RUN = duration.total_seconds()
 
     try:
-        tokens_input = completion.usage.input_tokens
-        tokens_output = completion.usage.output_tokens
-        total_tokens = completion.usage.input_tokens + completion.usage.output_tokens
+        tokens_input = completion.usage.prompt_tokens
+        tokens_output = completion.usage.completion_tokens
+        total_tokens = completion.usage.total_tokens
     except AttributeError:
         tokens_input = tokens_output = total_tokens = None
     
     try:
-        response_message = completion.content[0].text
+        response_message = completion.choices[0].message.content
         status = "success"
     except AttributeError:
         response_message = None
         status = "error"
 
     api_response = {
-        "status": status,
+        "status": "success",
         "model_name": model_name,
         "temperature": temperature,
         "ai_query_time": TIME_START.isoformat(),
         "ai_response_time": TIME_FINISHED.isoformat(),
         "ai_runtime": TIME_TO_RUN,
         "tokens_input": tokens_input,
         "tokens_output": tokens_output,
         "tokens_total": total_tokens,
         "ai_response_http_status_code": None,
-        "ai_response_stop_reason": completion.stop_reason,
+        "ai_response_stop_reason": None,
         "ai_response_data": response_message
     }
 
     return api_response
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.8/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py` & `csa_ai_foundation_model_api_clients-0.1.9/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.8/tests/dev/ask-chatgpt-the-capital-of-france.py` & `csa_ai_foundation_model_api_clients-0.1.9/tests/dev/ask-chatgpt-the-capital-of-france.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.8/tests/dev/ask-claude-the-capital-of-france.py` & `csa_ai_foundation_model_api_clients-0.1.9/tests/dev/ask-claude-the-capital-of-france.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.8/tests/dev/ask-gemini-the-capital-of-france.py` & `csa_ai_foundation_model_api_clients-0.1.9/tests/dev/ask-gemini-the-capital-of-france.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.8/.gitignore` & `csa_ai_foundation_model_api_clients-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.8/LICENSE` & `csa_ai_foundation_model_api_clients-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.8/README.md` & `csa_ai_foundation_model_api_clients-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.8/pyproject.toml` & `csa_ai_foundation_model_api_clients-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "csa_ai_foundation_model_api_clients"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Kurt Seifried", email="kseifried@cloudsecurityalliance.org" },
 ]
 description = "Cloud Security Alliance AI Foundation Model API Clients"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.8/PKG-INFO` & `csa_ai_foundation_model_api_clients-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: csa_ai_foundation_model_api_clients
-Version: 0.1.8
+Version: 0.1.9
 Summary: Cloud Security Alliance AI Foundation Model API Clients
 Project-URL: Homepage, https://github.com/CloudSecurityAlliance/csa-ai-foundation-model-api-clients
 Project-URL: Issues, https://github.com/CloudSecurityAlliance/csa-ai-foundation-model-api-clients/issues
 Author-email: Kurt Seifried <kseifried@cloudsecurityalliance.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

