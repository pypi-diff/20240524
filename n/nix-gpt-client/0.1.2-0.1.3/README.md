# Comparing `tmp/nix_gpt_client-0.1.2.tar.gz` & `tmp/nix_gpt_client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nix_gpt_client-0.1.2.tar", last modified: Fri May 17 12:43:11 2024, max compression
+gzip compressed data, was "nix_gpt_client-0.1.3.tar", last modified: Fri May 24 10:21:48 2024, max compression
```

## Comparing `nix_gpt_client-0.1.2.tar` & `nix_gpt_client-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-17 12:43:11.814694 nix_gpt_client-0.1.2/
--rw-r--r--   0 nix       (1000) nix       (1000)     1063 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.2/LICENCE
--rw-r--r--   0 nix       (1000) nix       (1000)     4163 2024-05-17 12:43:11.814694 nix_gpt_client-0.1.2/PKG-INFO
--rw-r--r--   0 nix       (1000) nix       (1000)     3470 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.2/README.md
--rw-r--r--   0 nix       (1000) nix       (1000)      832 2024-05-17 12:42:25.000000 nix_gpt_client-0.1.2/pyproject.toml
--rw-r--r--   0 nix       (1000) nix       (1000)       38 2024-05-17 12:43:11.814694 nix_gpt_client-0.1.2/setup.cfg
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-17 12:43:11.811360 nix_gpt_client-0.1.2/src/
--rw-r--r--   0 nix       (1000) nix       (1000)        0 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.2/src/__init__.py
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-17 12:43:11.811360 nix_gpt_client-0.1.2/src/nix/
--rw-r--r--   0 nix       (1000) nix       (1000)        0 2024-05-17 12:27:48.000000 nix_gpt_client-0.1.2/src/nix/__init__.py
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-17 12:43:11.814694 nix_gpt_client-0.1.2/src/nix/gptclient/
--rw-r--r--   0 nix       (1000) nix       (1000)       95 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.2/src/nix/gptclient/__init__.py
--rw-r--r--   0 nix       (1000) nix       (1000)     2159 2024-05-17 12:42:10.000000 nix_gpt_client-0.1.2/src/nix/gptclient/_gpt_client.py
--rw-r--r--   0 nix       (1000) nix       (1000)      680 2024-05-17 12:09:50.000000 nix_gpt_client-0.1.2/src/nix/gptclient/_types.py
--rw-r--r--   0 nix       (1000) nix       (1000)      654 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.2/src/nix/gptclient/_validate.py
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-17 12:43:11.814694 nix_gpt_client-0.1.2/src/nix_gpt_client.egg-info/
--rw-r--r--   0 nix       (1000) nix       (1000)     4163 2024-05-17 12:43:11.000000 nix_gpt_client-0.1.2/src/nix_gpt_client.egg-info/PKG-INFO
--rw-r--r--   0 nix       (1000) nix       (1000)      399 2024-05-17 12:43:11.000000 nix_gpt_client-0.1.2/src/nix_gpt_client.egg-info/SOURCES.txt
--rw-r--r--   0 nix       (1000) nix       (1000)        1 2024-05-17 12:43:11.000000 nix_gpt_client-0.1.2/src/nix_gpt_client.egg-info/dependency_links.txt
--rw-r--r--   0 nix       (1000) nix       (1000)        7 2024-05-17 12:43:11.000000 nix_gpt_client-0.1.2/src/nix_gpt_client.egg-info/requires.txt
--rw-r--r--   0 nix       (1000) nix       (1000)       13 2024-05-17 12:43:11.000000 nix_gpt_client-0.1.2/src/nix_gpt_client.egg-info/top_level.txt
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-24 10:21:48.678083 nix_gpt_client-0.1.3/
+-rw-r--r--   0 nix       (1000) nix       (1000)     1063 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.3/LICENCE
+-rw-r--r--   0 nix       (1000) nix       (1000)     4187 2024-05-24 10:21:48.678083 nix_gpt_client-0.1.3/PKG-INFO
+-rw-r--r--   0 nix       (1000) nix       (1000)     3470 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.3/README.md
+-rw-r--r--   0 nix       (1000) nix       (1000)      848 2024-05-24 10:19:59.000000 nix_gpt_client-0.1.3/pyproject.toml
+-rw-r--r--   0 nix       (1000) nix       (1000)       38 2024-05-24 10:21:48.678083 nix_gpt_client-0.1.3/setup.cfg
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-24 10:21:48.674749 nix_gpt_client-0.1.3/src/
+-rw-r--r--   0 nix       (1000) nix       (1000)        0 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.3/src/__init__.py
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-24 10:21:48.674749 nix_gpt_client-0.1.3/src/nix/
+-rw-r--r--   0 nix       (1000) nix       (1000)        0 2024-05-17 12:27:48.000000 nix_gpt_client-0.1.3/src/nix/__init__.py
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-24 10:21:48.678083 nix_gpt_client-0.1.3/src/nix/gptclient/
+-rw-r--r--   0 nix       (1000) nix       (1000)       95 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.3/src/nix/gptclient/__init__.py
+-rw-r--r--   0 nix       (1000) nix       (1000)     2382 2024-05-24 10:19:46.000000 nix_gpt_client-0.1.3/src/nix/gptclient/_gpt_client.py
+-rw-r--r--   0 nix       (1000) nix       (1000)      520 2024-05-24 10:19:17.000000 nix_gpt_client-0.1.3/src/nix/gptclient/_tokens_count.py
+-rw-r--r--   0 nix       (1000) nix       (1000)      680 2024-05-17 12:09:50.000000 nix_gpt_client-0.1.3/src/nix/gptclient/_types.py
+-rw-r--r--   0 nix       (1000) nix       (1000)      654 2024-05-06 15:30:22.000000 nix_gpt_client-0.1.3/src/nix/gptclient/_validate.py
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2024-05-24 10:21:48.678083 nix_gpt_client-0.1.3/src/nix_gpt_client.egg-info/
+-rw-r--r--   0 nix       (1000) nix       (1000)     4187 2024-05-24 10:21:48.000000 nix_gpt_client-0.1.3/src/nix_gpt_client.egg-info/PKG-INFO
+-rw-r--r--   0 nix       (1000) nix       (1000)      434 2024-05-24 10:21:48.000000 nix_gpt_client-0.1.3/src/nix_gpt_client.egg-info/SOURCES.txt
+-rw-r--r--   0 nix       (1000) nix       (1000)        1 2024-05-24 10:21:48.000000 nix_gpt_client-0.1.3/src/nix_gpt_client.egg-info/dependency_links.txt
+-rw-r--r--   0 nix       (1000) nix       (1000)       16 2024-05-24 10:21:48.000000 nix_gpt_client-0.1.3/src/nix_gpt_client.egg-info/requires.txt
+-rw-r--r--   0 nix       (1000) nix       (1000)       13 2024-05-24 10:21:48.000000 nix_gpt_client-0.1.3/src/nix_gpt_client.egg-info/top_level.txt
```

### Comparing `nix_gpt_client-0.1.2/LICENCE` & `nix_gpt_client-0.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `nix_gpt_client-0.1.2/PKG-INFO` & `nix_gpt_client-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: nix-gpt-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library for easy interaction with the GPT API, featuring typed requests and responses.
 Author-email: nks_nix <nikusunix@gmail.com>
 Maintainer-email: nks_nix <nikusunix@gmail.com>
 Project-URL: Homepage, https://github.com/nixnks/nix-gpt-client
 Project-URL: Documentation, https://readthedocs.org
 Project-URL: Repository, https://github.com/nixnks/nix-gpt-client.git
 Project-URL: Changelog, https://github.com/nixnks/nix-gpt-client/CHANGELOG.md
 Keywords: openai,gpt
 Classifier: Programming Language :: Python
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: openai
+Requires-Dist: tiktoken
 
 # nix-gpt-client
 
 nix-gpt-client is a simple Python library for working with the GPT API. It uses Pydantic to add input and output
 schemas, allowing you to manage data structures with ease.
 
 ## Table of Contents
```

### Comparing `nix_gpt_client-0.1.2/README.md` & `nix_gpt_client-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nix_gpt_client-0.1.2/pyproject.toml` & `nix_gpt_client-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nix-gpt-client"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
-    "openai"
+    "openai",
+    "tiktoken"
 ]
 requires-python = ">=3.11"
 authors = [
     { name = "nks_nix", email = "nikusunix@gmail.com" },
 ]
 maintainers = [
     { name = "nks_nix", email = "nikusunix@gmail.com" },
```

### Comparing `nix_gpt_client-0.1.2/src/nix/gptclient/_gpt_client.py` & `nix_gpt_client-0.1.3/src/nix/gptclient/_gpt_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,24 +39,28 @@
     def set_schema(self, schema: BaseModel, schema_type: GPTSchemaType):
         json_schema = json.dumps(schema.model_json_schema())
         self._messages.append({
             "role": "system",
             "content": f"{schema_type} JSON schema: {json_schema}"
         })
 
+    def get_messages_token_count(self, encoding_name: str) -> int:
+        from ._tokens_count import num_token_from_message
+        return sum([num_token_from_message(message, encoding_name) for message in self._messages])
+
     def run(self):
         try:
             response = self._ai_client.chat.completions.create(
                 messages=self._messages,
                 model=self._model,
                 temperature=self._temperature,
                 top_p=self._top_p,
                 presence_penalty=self._presence_penalty,
                 frequency_penalty=self._frequency_penalty,
-                response_format = self.response_format
+                response_format=self.response_format
             )
             if response.choices:
                 return response.choices[0].message.content
             else:
                 return None
         except openai.OpenAIError as error:
             raise error
```

### Comparing `nix_gpt_client-0.1.2/src/nix/gptclient/_types.py` & `nix_gpt_client-0.1.3/src/nix/gptclient/_types.py`

 * *Files identical despite different names*

### Comparing `nix_gpt_client-0.1.2/src/nix/gptclient/_validate.py` & `nix_gpt_client-0.1.3/src/nix/gptclient/_validate.py`

 * *Files identical despite different names*

### Comparing `nix_gpt_client-0.1.2/src/nix_gpt_client.egg-info/PKG-INFO` & `nix_gpt_client-0.1.3/src/nix_gpt_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: nix-gpt-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library for easy interaction with the GPT API, featuring typed requests and responses.
 Author-email: nks_nix <nikusunix@gmail.com>
 Maintainer-email: nks_nix <nikusunix@gmail.com>
 Project-URL: Homepage, https://github.com/nixnks/nix-gpt-client
 Project-URL: Documentation, https://readthedocs.org
 Project-URL: Repository, https://github.com/nixnks/nix-gpt-client.git
 Project-URL: Changelog, https://github.com/nixnks/nix-gpt-client/CHANGELOG.md
 Keywords: openai,gpt
 Classifier: Programming Language :: Python
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: openai
+Requires-Dist: tiktoken
 
 # nix-gpt-client
 
 nix-gpt-client is a simple Python library for working with the GPT API. It uses Pydantic to add input and output
 schemas, allowing you to manage data structures with ease.
 
 ## Table of Contents
```

