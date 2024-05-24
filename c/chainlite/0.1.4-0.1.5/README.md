# Comparing `tmp/chainlite-0.1.4.tar.gz` & `tmp/chainlite-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlite-0.1.4.tar", last modified: Thu May 23 07:26:02 2024, max compression
+gzip compressed data, was "chainlite-0.1.5.tar", last modified: Fri May 24 01:22:55 2024, max compression
```

## Comparing `chainlite-0.1.4.tar` & `chainlite-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:26:02.128672 chainlite-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 07:25:58.000000 chainlite-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-23 07:26:02.128672 chainlite-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-23 07:25:58.000000 chainlite-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:26:02.124672 chainlite-0.1.4/chainlite/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-23 07:25:58.000000 chainlite-0.1.4/chainlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-23 07:25:58.000000 chainlite-0.1.4/chainlite/llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10689 2024-05-23 07:25:58.000000 chainlite-0.1.4/chainlite/llm_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7938 2024-05-23 07:25:58.000000 chainlite-0.1.4/chainlite/load_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-23 07:25:58.000000 chainlite-0.1.4/chainlite/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:26:02.124672 chainlite-0.1.4/chainlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-23 07:26:02.000000 chainlite-0.1.4/chainlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-23 07:26:02.000000 chainlite-0.1.4/chainlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 07:26:02.000000 chainlite-0.1.4/chainlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-23 07:26:02.000000 chainlite-0.1.4/chainlite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 07:26:02.000000 chainlite-0.1.4/chainlite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-23 07:25:58.000000 chainlite-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 07:26:02.128672 chainlite-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-23 07:25:58.000000 chainlite-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:26:02.124672 chainlite-0.1.4/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 07:25:58.000000 chainlite-0.1.4/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-23 07:25:58.000000 chainlite-0.1.4/tasks/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:26:02.124672 chainlite-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-23 07:25:58.000000 chainlite-0.1.4/tests/test_llm_generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:22:55.651161 chainlite-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 01:22:47.000000 chainlite-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-24 01:22:55.651161 chainlite-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-24 01:22:47.000000 chainlite-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:22:55.647161 chainlite-0.1.5/chainlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-24 01:22:47.000000 chainlite-0.1.5/chainlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-05-24 01:22:47.000000 chainlite-0.1.5/chainlite/llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10689 2024-05-24 01:22:47.000000 chainlite-0.1.5/chainlite/llm_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-24 01:22:47.000000 chainlite-0.1.5/chainlite/load_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-24 01:22:47.000000 chainlite-0.1.5/chainlite/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:22:55.651161 chainlite-0.1.5/chainlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-24 01:22:55.000000 chainlite-0.1.5/chainlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-24 01:22:55.000000 chainlite-0.1.5/chainlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 01:22:55.000000 chainlite-0.1.5/chainlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-24 01:22:55.000000 chainlite-0.1.5/chainlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-24 01:22:55.000000 chainlite-0.1.5/chainlite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-24 01:22:47.000000 chainlite-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 01:22:55.651161 chainlite-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-24 01:22:47.000000 chainlite-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:22:55.651161 chainlite-0.1.5/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-24 01:22:47.000000 chainlite-0.1.5/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-24 01:22:47.000000 chainlite-0.1.5/tasks/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:22:55.651161 chainlite-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-24 01:22:47.000000 chainlite-0.1.5/tests/test_llm_generate.py
```

### Comparing `chainlite-0.1.4/LICENSE` & `chainlite-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.4/PKG-INFO` & `chainlite-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlite
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package that uses LangChain and LiteLLM to call large language model APIs easily
 Home-page: https://github.com/stanford-oval/chainlite
 Author: Sina Semnani
 Author-email: sinaj@cs.stanford.edu
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `chainlite-0.1.4/README.md` & `chainlite-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.4/chainlite/llm_config.py` & `chainlite-0.1.5/chainlite/llm_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import os
 import os
 import litellm
 from langchain.cache import RedisCache
 from langchain.globals import set_llm_cache
 import redis
 
+from .load_prompt import set_custom_template_paths
+
 # TODO move cache setting to the config file
 # We do not use LiteLLM's cache, use LangChain's instead
 # litellm.enable_cache(type="redis", url="redis://localhost:6379")
 redis_client = redis.Redis.from_url("redis://localhost:6379")
 set_llm_cache(RedisCache(redis_client))
 
 litellm.drop_params = (
@@ -88,14 +90,16 @@
 
     for endpoint in all_llm_endpoints:
         for engine, model in endpoint["engine_map"].items():
             all_configured_engines.append(engine)
             if model.startswith("huggingface/"):
                 local_engine_set.add(engine)
 
+    set_custom_template_paths(prompt_dirs)
+
 
 # this code is not safe to use with multiprocessing, only multithreading
 thread_lock = threading.Lock()
 
 
 total_cost = 0  # in USD
```

### Comparing `chainlite-0.1.4/chainlite/llm_generate.py` & `chainlite-0.1.5/chainlite/llm_generate.py`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.4/chainlite/load_prompt.py` & `chainlite-0.1.5/chainlite/load_prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,31 +24,25 @@
         "# DISTILLATION INSTRUCTION\n",
     ],
 }
 
 jinja_environment = None  # Global variable to hold the Jinja2 environment
 
 
-def initialize_jinja_environment(loader_paths=None):
+def initialize_jinja_environment(loader_paths):
     global jinja_environment
-    if loader_paths is None:
-        loader_paths = ["./", "./pipelines/", "./pipelines/prompts/"]
 
     loader = FileSystemLoader(loader_paths)
     jinja_environment = Environment(
         loader=loader,
         trim_blocks=True,
         lstrip_blocks=True,
     )
 
 
-# Initialize the environment with default paths
-initialize_jinja_environment()
-
-
 def set_custom_template_paths(paths):
     """
     Allows the user to set custom paths for the Jinja2 FileSystemLoader.
 
     Args:
         paths (list of str): List of directory paths to use for loading templates.
     """
```

### Comparing `chainlite-0.1.4/chainlite.egg-info/PKG-INFO` & `chainlite-0.1.5/chainlite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlite
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package that uses LangChain and LiteLLM to call large language model APIs easily
 Home-page: https://github.com/stanford-oval/chainlite
 Author: Sina Semnani
 Author-email: sinaj@cs.stanford.edu
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `chainlite-0.1.4/setup.py` & `chainlite-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chainlite",
-    version="0.1.4",
+    version="0.1.5",
     author="Sina Semnani",
     author_email="sinaj@cs.stanford.edu",
     description="A Python package that uses LangChain and LiteLLM to call large language model APIs easily",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/stanford-oval/chainlite",
     packages=find_packages(),
```

### Comparing `chainlite-0.1.4/tasks/main.py` & `chainlite-0.1.5/tasks/main.py`

 * *Files identical despite different names*

### Comparing `chainlite-0.1.4/tests/test_llm_generate.py` & `chainlite-0.1.5/tests/test_llm_generate.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 load_config_from_file("./chainlite_config.yaml")
 
 @pytest.mark.asyncio(scope="session")
 async def test_llm_generate():
 
     response = await llm_generation_chain(
-        template_file="tests/test.prompt",
+        template_file="test.prompt", # prompt path relative to one of the paths specified in `prompt_dirs`
         engine="gpt-35-turbo",
         max_tokens=100,
     ).ainvoke({})
     logger.info(response)
 
     assert response is not None, "The response should not be None"
     assert isinstance(response, str), "The response should be a string"
```

