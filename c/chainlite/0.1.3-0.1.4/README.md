# Comparing `tmp/chainlite-0.1.3.tar.gz` & `tmp/chainlite-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlite-0.1.3.tar", last modified: Wed May 22 02:26:35 2024, max compression
+gzip compressed data, was "chainlite-0.1.4.tar", last modified: Thu May 23 07:26:02 2024, max compression
```

## Comparing `chainlite-0.1.3.tar` & `chainlite-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:26:35.221000 chainlite-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 02:26:31.000000 chainlite-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-05-22 02:26:35.221000 chainlite-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-22 02:26:31.000000 chainlite-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:26:35.221000 chainlite-0.1.3/chainlite/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-22 02:26:31.000000 chainlite-0.1.3/chainlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-22 02:26:31.000000 chainlite-0.1.3/chainlite/llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9245 2024-05-22 02:26:31.000000 chainlite-0.1.3/chainlite/llm_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7938 2024-05-22 02:26:31.000000 chainlite-0.1.3/chainlite/load_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-22 02:26:31.000000 chainlite-0.1.3/chainlite/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:26:35.221000 chainlite-0.1.3/chainlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-05-22 02:26:35.000000 chainlite-0.1.3/chainlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-22 02:26:35.000000 chainlite-0.1.3/chainlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:26:35.000000 chainlite-0.1.3/chainlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-22 02:26:35.000000 chainlite-0.1.3/chainlite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 02:26:35.000000 chainlite-0.1.3/chainlite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-22 02:26:31.000000 chainlite-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 02:26:35.221000 chainlite-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-22 02:26:31.000000 chainlite-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:26:35.221000 chainlite-0.1.3/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 02:26:31.000000 chainlite-0.1.3/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-22 02:26:31.000000 chainlite-0.1.3/tasks/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:26:35.221000 chainlite-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-22 02:26:31.000000 chainlite-0.1.3/tests/test_llm_generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:26:02.128672 chainlite-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 07:25:58.000000 chainlite-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-23 07:26:02.128672 chainlite-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-23 07:25:58.000000 chainlite-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:26:02.124672 chainlite-0.1.4/chainlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-23 07:25:58.000000 chainlite-0.1.4/chainlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-23 07:25:58.000000 chainlite-0.1.4/chainlite/llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10689 2024-05-23 07:25:58.000000 chainlite-0.1.4/chainlite/llm_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7938 2024-05-23 07:25:58.000000 chainlite-0.1.4/chainlite/load_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-23 07:25:58.000000 chainlite-0.1.4/chainlite/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:26:02.124672 chainlite-0.1.4/chainlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-23 07:26:02.000000 chainlite-0.1.4/chainlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-23 07:26:02.000000 chainlite-0.1.4/chainlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 07:26:02.000000 chainlite-0.1.4/chainlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-23 07:26:02.000000 chainlite-0.1.4/chainlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 07:26:02.000000 chainlite-0.1.4/chainlite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-23 07:25:58.000000 chainlite-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 07:26:02.128672 chainlite-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-23 07:25:58.000000 chainlite-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:26:02.124672 chainlite-0.1.4/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 07:25:58.000000 chainlite-0.1.4/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-23 07:25:58.000000 chainlite-0.1.4/tasks/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:26:02.124672 chainlite-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-23 07:25:58.000000 chainlite-0.1.4/tests/test_llm_generate.py
```

### Comparing `chainlite-0.1.3/LICENSE` & `chainlite-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.3/PKG-INFO` & `chainlite-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlite
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package that uses LangChain and LiteLLM to call large language model APIs easily
 Home-page: https://github.com/stanford-oval/chainlite
 Author: Sina Semnani
 Author-email: sinaj@cs.stanford.edu
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -82,15 +82,18 @@
 
 ## Full Example
 
 `joke.prompt` with a 1-shot example:
 
 ```markdown
 # instruction
-Tell a joke about the input topic.
+Tell a joke about the input topic. The format of the joke should be a question and response, separated by a line break.
+
+# distillation instruction
+Tell a joke.
 
 # input
 Physics
 
 # output
 Why don't scientists trust atoms?
 Because they make up everything!
@@ -108,15 +111,21 @@
     response = await llm_generation_chain(
         template_file="joke.prompt",
         engine="gpt-35-turbo",
         max_tokens=100,
     ).ainvoke({"topic": topic})
     print(response)
 
-asyncio.run(tell_joke("Life as a PhD student"))
+asyncio.run(tell_joke("Life as a PhD student")) # prints "Why did the PhD student bring a ladder to the library?\nTo take their research to the next level!"
+write_prompt_logs_to_file("llm_input_outputs.jsonl")
+```
+
+Then you will have `llm_input_outputs.jsonl`:
+```json
+{"template_name": "joke.prompt", "instruction": "Tell a joke.", "input": "Life as a PhD student", "output": "Why did the PhD student bring a ladder to the library?\nTo take their research to the next level!"}
 ```
 
 ## Configuration
 
 The `chainlite_config.yaml` file allows you to customize the behavior of ChainLite. Modify the file to set your preferences for the LangChain and LiteLLM integrations.
 
 ## Contributing
```

### Comparing `chainlite-0.1.3/README.md` & `chainlite-0.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -50,15 +50,18 @@
 
 ## Full Example
 
 `joke.prompt` with a 1-shot example:
 
 ```markdown
 # instruction
-Tell a joke about the input topic.
+Tell a joke about the input topic. The format of the joke should be a question and response, separated by a line break.
+
+# distillation instruction
+Tell a joke.
 
 # input
 Physics
 
 # output
 Why don't scientists trust atoms?
 Because they make up everything!
@@ -76,15 +79,21 @@
     response = await llm_generation_chain(
         template_file="joke.prompt",
         engine="gpt-35-turbo",
         max_tokens=100,
     ).ainvoke({"topic": topic})
     print(response)
 
-asyncio.run(tell_joke("Life as a PhD student"))
+asyncio.run(tell_joke("Life as a PhD student")) # prints "Why did the PhD student bring a ladder to the library?\nTo take their research to the next level!"
+write_prompt_logs_to_file("llm_input_outputs.jsonl")
+```
+
+Then you will have `llm_input_outputs.jsonl`:
+```json
+{"template_name": "joke.prompt", "instruction": "Tell a joke.", "input": "Life as a PhD student", "output": "Why did the PhD student bring a ladder to the library?\nTo take their research to the next level!"}
 ```
 
 ## Configuration
 
 The `chainlite_config.yaml` file allows you to customize the behavior of ChainLite. Modify the file to set your preferences for the LangChain and LiteLLM integrations.
 
 ## Contributing
```

### Comparing `chainlite-0.1.3/chainlite/llm_config.py` & `chainlite-0.1.4/chainlite/llm_config.py`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.3/chainlite/llm_generate.py` & `chainlite-0.1.4/chainlite/llm_generate.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from langchain_core.output_parsers import StrOutputParser
 
 from .load_prompt import load_fewshot_prompt_template
 from langchain_community.chat_models import ChatLiteLLM
 from langchain_core.callbacks import AsyncCallbackHandler
 from langchain_core.outputs import LLMResult
 from langchain_core.messages import BaseMessage
-from langchain_core.runnables import chain
+from langchain_core.runnables import chain, Runnable
 
 from .utils import get_logger
 
 
 logging.getLogger("LiteLLM").setLevel(logging.WARNING)
 logging.getLogger("LiteLLM Router").setLevel(logging.WARNING)
 logging.getLogger("LiteLLM Proxy").setLevel(logging.WARNING)
@@ -195,19 +195,38 @@
 
 
 def llm_generation_chain(
     template_file: str,
     engine: str,
     max_tokens: int,
     temperature: float = 0.0,
-    stop_tokens=None,
+    stop_tokens: Optional[list[str]] = None,
     top_p: float = 0.9,
     postprocess: bool = False,
     bind_prompt_values: dict = {},
-):
+) -> Runnable:
+    """
+    Constructs a LangChain generation chain for LLM response utilizing LLM APIs prescribed in the ChainLite config file.
+
+    Parameters:
+        template_file (str): The path to the generation template file. Must be a .prompt file.
+        engine (str): The language model engine to employ. An engine represents the left-hand value of an `engine_map` in the ChainLite config file.
+        max_tokens (int): The upper limit of tokens the LLM can generate.
+        temperature (float, optional): Dictates the randomness in the generation. Must be >= 0.0. Defaults to 0.0 (deterministic).
+        stop_tokens (list[str], optional): The list of tokens causing the LLM to stop generating. Defaults to None.
+        top_p (float, optional): The max cumulative probability for nucleus sampling, must be within 0.0 - 1.0. Defaults to 0.9.
+        postprocess (bool, optional): If true, postprocessing deletes incomplete sentences from the end of the generation. Defaults to False.
+        bind_prompt_values (dict, optional): A dictionary containing {Variable: str : Value}. Binds values to the prompt. Additional variables can be provided when the chain is called. Defaults to {}.
+
+    Returns:
+        Runnable: The language model generation chain
+
+    Raises:
+        IndexError: Raised when no engine matches the provided string in the LLM APIs configured, or the API key is not found.
+    """
     # Decide which LLM resource to send this request to.
     potential_llm_resources = [
         resource
         for resource in llm_config.all_llm_endpoints
         if engine in resource["engine_map"]
     ]
     if len(potential_llm_resources) == 0:
```

### Comparing `chainlite-0.1.3/chainlite/load_prompt.py` & `chainlite-0.1.4/chainlite/load_prompt.py`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.3/chainlite.egg-info/PKG-INFO` & `chainlite-0.1.4/chainlite.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlite
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package that uses LangChain and LiteLLM to call large language model APIs easily
 Home-page: https://github.com/stanford-oval/chainlite
 Author: Sina Semnani
 Author-email: sinaj@cs.stanford.edu
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -82,15 +82,18 @@
 
 ## Full Example
 
 `joke.prompt` with a 1-shot example:
 
 ```markdown
 # instruction
-Tell a joke about the input topic.
+Tell a joke about the input topic. The format of the joke should be a question and response, separated by a line break.
+
+# distillation instruction
+Tell a joke.
 
 # input
 Physics
 
 # output
 Why don't scientists trust atoms?
 Because they make up everything!
@@ -108,15 +111,21 @@
     response = await llm_generation_chain(
         template_file="joke.prompt",
         engine="gpt-35-turbo",
         max_tokens=100,
     ).ainvoke({"topic": topic})
     print(response)
 
-asyncio.run(tell_joke("Life as a PhD student"))
+asyncio.run(tell_joke("Life as a PhD student")) # prints "Why did the PhD student bring a ladder to the library?\nTo take their research to the next level!"
+write_prompt_logs_to_file("llm_input_outputs.jsonl")
+```
+
+Then you will have `llm_input_outputs.jsonl`:
+```json
+{"template_name": "joke.prompt", "instruction": "Tell a joke.", "input": "Life as a PhD student", "output": "Why did the PhD student bring a ladder to the library?\nTo take their research to the next level!"}
 ```
 
 ## Configuration
 
 The `chainlite_config.yaml` file allows you to customize the behavior of ChainLite. Modify the file to set your preferences for the LangChain and LiteLLM integrations.
 
 ## Contributing
```

### Comparing `chainlite-0.1.3/setup.py` & `chainlite-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chainlite",
-    version="0.1.3",
+    version="0.1.4",
     author="Sina Semnani",
     author_email="sinaj@cs.stanford.edu",
     description="A Python package that uses LangChain and LiteLLM to call large language model APIs easily",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/stanford-oval/chainlite",
     packages=find_packages(),
```

### Comparing `chainlite-0.1.3/tasks/main.py` & `chainlite-0.1.4/tasks/main.py`

 * *Files identical despite different names*

