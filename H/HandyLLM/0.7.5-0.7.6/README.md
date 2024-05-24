# Comparing `tmp/handyllm-0.7.5.tar.gz` & `tmp/handyllm-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "handyllm-0.7.5.tar", last modified: Thu May 23 10:29:38 2024, max compression
+gzip compressed data, was "handyllm-0.7.6.tar", last modified: Fri May 24 16:03:10 2024, max compression
```

## Comparing `handyllm-0.7.5.tar` & `handyllm-0.7.6.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:29:38.960876 handyllm-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-23 10:29:35.000000 handyllm-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-23 10:29:38.960876 handyllm-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-23 10:29:35.000000 handyllm-0.7.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-23 10:29:35.000000 handyllm-0.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 10:29:38.960876 handyllm-0.7.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:29:38.952875 handyllm-0.7.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:29:38.960876 handyllm-0.7.5/src/HandyLLM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-23 10:29:38.000000 handyllm-0.7.5/src/HandyLLM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-23 10:29:38.000000 handyllm-0.7.5/src/HandyLLM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:29:38.000000 handyllm-0.7.5/src/HandyLLM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-23 10:29:38.000000 handyllm-0.7.5/src/HandyLLM.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-23 10:29:38.000000 handyllm-0.7.5/src/HandyLLM.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 10:29:38.000000 handyllm-0.7.5/src/HandyLLM.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:29:38.956875 handyllm-0.7.5/src/handyllm/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/_str_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:29:38.960876 handyllm-0.7.5/src/handyllm/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/deprecated/api_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14098 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/deprecated/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/endpoint_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    32282 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/hprompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    16985 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/openai_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/prompt_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12431 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/requestor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-23 10:29:35.000000 handyllm-0.7.5/src/handyllm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:29:38.960876 handyllm-0.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-23 10:29:35.000000 handyllm-0.7.5/tests/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-23 10:29:35.000000 handyllm-0.7.5/tests/test_client_async_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-23 10:29:35.000000 handyllm-0.7.5/tests/test_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-23 10:29:35.000000 handyllm-0.7.5/tests/test_hprompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-23 10:29:35.000000 handyllm-0.7.5/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-23 10:29:35.000000 handyllm-0.7.5/tests/test_tts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:03:10.568071 handyllm-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-24 16:03:05.000000 handyllm-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-24 16:03:10.568071 handyllm-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-24 16:03:05.000000 handyllm-0.7.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-24 16:03:05.000000 handyllm-0.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 16:03:10.568071 handyllm-0.7.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:03:10.560071 handyllm-0.7.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:03:10.568071 handyllm-0.7.6/src/HandyLLM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-24 16:03:10.000000 handyllm-0.7.6/src/HandyLLM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-24 16:03:10.000000 handyllm-0.7.6/src/HandyLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 16:03:10.000000 handyllm-0.7.6/src/HandyLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-24 16:03:10.000000 handyllm-0.7.6/src/HandyLLM.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-24 16:03:10.000000 handyllm-0.7.6/src/HandyLLM.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 16:03:10.000000 handyllm-0.7.6/src/HandyLLM.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:03:10.564071 handyllm-0.7.6/src/handyllm/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-24 16:03:05.000000 handyllm-0.7.6/src/handyllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-24 16:03:05.000000 handyllm-0.7.6/src/handyllm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-24 16:03:05.000000 handyllm-0.7.6/src/handyllm/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-24 16:03:05.000000 handyllm-0.7.6/src/handyllm/_str_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-05-24 16:03:05.000000 handyllm-0.7.6/src/handyllm/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-24 16:03:05.000000 handyllm-0.7.6/src/handyllm/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:03:10.564071 handyllm-0.7.6/src/handyllm/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-24 16:03:05.000000 handyllm-0.7.6/src/handyllm/deprecated/api_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14098 2024-05-24 16:03:05.000000 handyllm-0.7.6/src/handyllm/deprecated/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-24 16:03:05.000000 handyllm-0.7.6/src/handyllm/endpoint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28379 2024-05-24 16:03:05.000000 handyllm-0.7.6/src/handyllm/hprompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-24 16:03:05.000000 handyllm-0.7.6/src/handyllm/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16985 2024-05-24 16:03:05.000000 handyllm-0.7.6/src/handyllm/openai_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-05-24 16:03:05.000000 handyllm-0.7.6/src/handyllm/prompt_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12431 2024-05-24 16:03:05.000000 handyllm-0.7.6/src/handyllm/requestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-05-24 16:03:05.000000 handyllm-0.7.6/src/handyllm/run_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-05-24 16:03:05.000000 handyllm-0.7.6/src/handyllm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:03:10.568071 handyllm-0.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-24 16:03:05.000000 handyllm-0.7.6/tests/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-24 16:03:05.000000 handyllm-0.7.6/tests/test_client_async_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-24 16:03:05.000000 handyllm-0.7.6/tests/test_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-24 16:03:05.000000 handyllm-0.7.6/tests/test_hprompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-24 16:03:05.000000 handyllm-0.7.6/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-24 16:03:05.000000 handyllm-0.7.6/tests/test_tts.py
```

### Comparing `handyllm-0.7.5/LICENSE` & `handyllm-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.5/PKG-INFO` & `handyllm-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.7.5
+Version: 0.7.6
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `handyllm-0.7.5/README.md` & `handyllm-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.5/pyproject.toml` & `handyllm-0.7.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HandyLLM"
-version = "0.7.5"
+version = "0.7.6"
 authors = [
   { name="Atomie CHEN", email="atomic_cwh@163.com" },
 ]
 description = "A handy toolkit for using LLM."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `handyllm-0.7.5/src/HandyLLM.egg-info/PKG-INFO` & `handyllm-0.7.6/src/HandyLLM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.7.5
+Version: 0.7.6
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `handyllm-0.7.5/src/HandyLLM.egg-info/SOURCES.txt` & `handyllm-0.7.6/src/HandyLLM.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 src/handyllm/cli.py
 src/handyllm/endpoint_manager.py
 src/handyllm/hprompt.py
 src/handyllm/openai_api.py
 src/handyllm/openai_client.py
 src/handyllm/prompt_converter.py
 src/handyllm/requestor.py
+src/handyllm/run_config.py
 src/handyllm/utils.py
 src/handyllm/deprecated/api_request.py
 src/handyllm/deprecated/openai_api.py
 tests/test_azure.py
 tests/test_client_async_sync.py
 tests/test_endpoint.py
 tests/test_hprompt.py
```

### Comparing `handyllm-0.7.5/src/handyllm/_str_enum.py` & `handyllm-0.7.6/src/handyllm/_str_enum.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.5/src/handyllm/_utils.py` & `handyllm-0.7.6/src/handyllm/_utils.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.5/src/handyllm/cli.py` & `handyllm-0.7.6/src/handyllm/cli.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.5/src/handyllm/deprecated/api_request.py` & `handyllm-0.7.6/src/handyllm/deprecated/api_request.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.5/src/handyllm/deprecated/openai_api.py` & `handyllm-0.7.6/src/handyllm/deprecated/openai_api.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.5/src/handyllm/endpoint_manager.py` & `handyllm-0.7.6/src/handyllm/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.5/src/handyllm/hprompt.py` & `handyllm-0.7.6/src/handyllm/hprompt.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,51 +11,48 @@
     "dump_to",
     "load_var_map",
     "RunConfig",
     "RecordRequestMode",
     "CredentialType",
 ]
 
+import inspect
 import json
 import re
 import copy
 import io
-import os
 import sys
 from pathlib import Path
 from datetime import datetime
-from typing import Optional, Union, TypeVar
-from enum import auto
+from typing import Dict, Optional, Union, TypeVar
 from abc import abstractmethod, ABC
-from dataclasses import dataclass, asdict, fields, replace
+from dataclasses import replace
 
 import yaml
 import frontmatter
-from mergedeep import merge, Strategy
+from mergedeep import merge as merge_dict, Strategy
 from dotenv import load_dotenv
 
 from .prompt_converter import PromptConverter
 from .openai_client import ClientMode, OpenAIClient
 from .utils import (
     astream_chat_all, astream_completions, 
     stream_chat_all, stream_completions, 
 )
-from ._str_enum import AutoStrEnum
+from .run_config import RunConfig, RecordRequestMode, PathType, VarMapType, CredentialType
 
 
 PromptType = TypeVar('PromptType', bound='HandyPrompt')
-if sys.version_info >= (3, 9):
-    PathType = Union[str, os.PathLike[str]]
-else:
-    PathType = Union[str, os.PathLike]
+
 
 converter = PromptConverter()
 handler = frontmatter.YAMLHandler()
 p_var_map = re.compile(r'(%\w+%)')
 
+DEFAULT_CONFIG = RunConfig()
 DEFAULT_BLACKLIST = (
     "api_key", "organization", "api_base", "api_type", "api_version", 
     "endpoint_manager", "endpoint", "engine", "deployment_id", 
     "model_engine_map", "dest_url", 
 )
 
 
@@ -132,154 +129,14 @@
     blocks = p_var_map.split(content)
     for idx in range(1, len(blocks), 2):
         key = blocks[idx]
         value = blocks[idx+1]
         substitute_map[key] = value.strip()
     return substitute_map
 
-class RecordRequestMode(AutoStrEnum):
-    BLACKLIST = auto()  # record all request arguments except specified ones
-    WHITELIST = auto()  # record only specified request arguments
-    NONE = auto()  # record no request arguments
-    ALL = auto()  # record all request arguments
-
-
-class CredentialType(AutoStrEnum):
-    # load environment variables from the credential file
-    ENV = auto()
-    # load the content of the file as request arguments
-    JSON = auto()
-    YAML = auto()
-
-
-@dataclass
-class RunConfig:
-    # record request arguments
-    record_request: Optional[RecordRequestMode] = None  # default: RecordRequestMode.BLACKLIST
-    record_blacklist: Optional[list[str]] = None  # default: DEFAULT_BLACKLIST
-    record_whitelist: Optional[list[str]] = None
-    # variable map
-    var_map: Optional[dict[str, str]] = None
-    # variable map file path
-    var_map_path: Optional[PathType] = None
-    # output the result to a file or a file descriptor
-    output_path: Optional[PathType] = None
-    output_fd: Optional[io.IOBase] = None
-    # output the evaluated prompt to a file or a file descriptor
-    output_evaled_prompt_path: Optional[PathType] = None
-    output_evaled_prompt_fd: Optional[io.IOBase] = None
-    # credential file path
-    credential_path: Optional[PathType] = None
-    # credential type: env, json, yaml
-    # if env, load environment variables from the credential file
-    # if json or yaml, load the content of the file as request arguments
-    credential_type: Optional[CredentialType] = None  # default: guess from the file extension
-    
-    # verbose output to stderr
-    verbose: Optional[bool] = None  # default: False
-    
-    def __setattr__(self, name: str, value: object):
-        if name == "record_request":
-            # validate record_request value
-            if isinstance(value, str):
-                if value not in RecordRequestMode:
-                    raise ValueError(f"unsupported record_request value: {value}")
-            elif isinstance(value, RecordRequestMode):
-                value = value.value
-            elif value is None:  # this field is optional
-                pass
-            else:
-                raise ValueError(f"unsupported record_request value: {value}")
-        elif name == "credential_type":
-            # validate credential_type value
-            if isinstance(value, str):
-                if value == 'yml':
-                    value = CredentialType.YAML.value
-                elif value not in CredentialType:
-                    raise ValueError(f"unsupported credential_type value: {value}")
-            elif isinstance(value, CredentialType):
-                value = value.value
-            elif value is None:  # this field is optional
-                pass
-            else:
-                raise ValueError(f"unsupported credential_type value: {value}")
-        super().__setattr__(name, value)
-    
-    def __len__(self):
-        return len([f for f in fields(self) if getattr(self, f.name) is not None])
-    
-    @classmethod
-    def from_dict(cls, obj: dict, base_path: Optional[PathType] = None):
-        input_kwargs = {}
-        for field in fields(cls):
-            if field.name in obj:
-                input_kwargs[field.name] = obj[field.name]
-        # add base_path to path fields and convert to resolved path
-        if base_path:
-            for path_field in ("output_path", "output_evaled_prompt_path", "var_map_path", "credential_path"):
-                if path_field in input_kwargs:
-                    org_path = input_kwargs[path_field]
-                    new_path = str(Path(base_path, org_path).resolve())
-                    # retain trailing slash
-                    if org_path.endswith(('/')):
-                        new_path += '/'
-                    input_kwargs[path_field] = new_path
-        return cls(**input_kwargs)
-    
-    def pretty_print(self, file=sys.stderr):
-        print("RunConfig:", file=file)
-        for field in fields(self):
-            value = getattr(self, field.name)
-            if value is not None:
-                print(f"  {field.name}: {value}", file=file)
-    
-    def to_dict(self, retain_fd=False, base_path: Optional[PathType] = None) -> dict:
-        # record and remove file descriptors
-        tmp_output_fd = self.output_fd
-        tmp_output_evaled_prompt_fd = self.output_evaled_prompt_fd
-        self.output_fd = None
-        self.output_evaled_prompt_fd = None
-        # convert to dict
-        obj = asdict(self, dict_factory=lambda x: { k: v for k, v in x if v is not None })
-        # restore file descriptors
-        self.output_fd = tmp_output_fd
-        self.output_evaled_prompt_fd = tmp_output_evaled_prompt_fd
-        if retain_fd:
-            # keep file descriptors
-            obj["output_fd"] = self.output_fd
-            obj["output_evaled_prompt_fd"] = self.output_evaled_prompt_fd
-        # convert path to relative path
-        if base_path:
-            for path_field in ("output_path", "output_evaled_prompt_path", "var_map_path", "credential_path"):
-                if path_field in obj:
-                    org_path = obj[path_field]
-                    try:
-                        new_path = str(Path(org_path).relative_to(base_path))
-                        obj[path_field] = new_path
-                    except ValueError:
-                        # org_path is not under base_path, keep the original path
-                        pass
-        return obj
-
-    def merge(self, other: RunConfig, inplace=False) -> RunConfig:
-        # merge the RunConfig object with another RunConfig object
-        # return a new RunConfig object if inplace is False
-        if not inplace:
-            new_run_config = replace(self)
-        else:
-            new_run_config = self
-        for field in fields(new_run_config):
-            v = getattr(other, field.name)
-            if v is not None:
-                setattr(new_run_config, field.name, v)
-        return new_run_config
-
-
-DEFAULT_CONFIG = RunConfig()
-
 
 class HandyPrompt(ABC):
     
     TEMPLATE_OUTPUT_FILENAME = "result.%Y%m%d-%H%M%S.hprompt"
     TEMPLATE_OUTPUT_EVAL_FILENAME = "evaled.%Y%m%d-%H%M%S.hprompt"
     
     def __init__(
@@ -324,15 +181,15 @@
     def _dumps_frontmatter(cls, request: dict, run_config: RunConfig, base_path: Optional[PathType] = None) -> str:
         # dump frontmatter
         if not run_config and not request:
             return ""
         # need to filter the request
         front_data = cls._filter_request(request, run_config)
         if run_config:
-            front_data['meta'] = run_config.to_dict(retain_fd=False, base_path=base_path)
+            front_data['meta'] = run_config.to_dict(retain_object=False, base_path=base_path)
         post = frontmatter.Post("", None, **front_data)
         return frontmatter.dumps(post, handler).strip() + "\n\n"
     
     def dumps(self, base_path: Optional[PathType] = None) -> str:
         serialized_data = self._serialize_data(self.data)
         base_path = base_path or self.base_path
         return self._dumps_frontmatter(self.request, self.run_config, base_path) + serialized_data
@@ -348,20 +205,26 @@
     @abstractmethod
     def _eval_data(self: PromptType, run_config: RunConfig) -> Union[str, list]:
         ...
     
     def eval(
         self: PromptType, 
         run_config: RunConfig = DEFAULT_CONFIG,
+        var_map: Optional[VarMapType] = None,
         **kwargs) -> PromptType:
         '''
-        Evaluate the prompt with the given run_config. 
+        Evaluate the prompt with the given run_config. var_map is for convenience.
         A new prompt object is returned.
         '''
         new_run_config = self.eval_run_config(run_config)
+        if var_map:
+            if new_run_config.var_map is None:
+                new_run_config.var_map = {}
+            # merge var_map instead of replacing as a whole
+            merge_dict(new_run_config.var_map, var_map, strategy=Strategy.REPLACE)
         new_data = self._eval_data(new_run_config)
         # update the request with the keyword arguments
         evaled_request = copy.deepcopy(self.request)
         evaled_request.update(kwargs)
         return self.__class__(
             new_data,
             evaled_request,
@@ -404,18 +267,19 @@
         evaled_prompt: PromptType,
         stream: bool,
         ) -> PromptType:
         ...
     
     def run(
         self: PromptType, 
-        client: OpenAIClient = None, 
+        client: Optional[OpenAIClient] = None, 
         run_config: RunConfig = DEFAULT_CONFIG,
+        var_map: Optional[VarMapType] = None,
         **kwargs) -> PromptType:
-        evaled_prompt, stream = self._prepare_run(run_config, kwargs)
+        evaled_prompt, stream = self._prepare_run(run_config, var_map, kwargs)
         if client:
             new_prompt = self._run_with_client(client, evaled_prompt, stream)
         else:
             with OpenAIClient(ClientMode.SYNC) as client:
                 new_prompt = self._run_with_client(client, evaled_prompt, stream)
         self._post_check_output(stream, run_config, new_prompt)
         return new_prompt
@@ -428,18 +292,19 @@
         evaled_prompt: PromptType,
         stream: bool,
         ) -> PromptType:
         ...
     
     async def arun(
         self: PromptType, 
-        client: OpenAIClient = None, 
+        client: Optional[OpenAIClient] = None, 
         run_config: RunConfig = DEFAULT_CONFIG,
+        var_map: Optional[VarMapType] = None,
         **kwargs) -> PromptType:
-        evaled_prompt, stream = self._prepare_run(run_config, kwargs)
+        evaled_prompt, stream = self._prepare_run(run_config, var_map, kwargs)
         if client:
             new_prompt = await self._arun_with_client(client, evaled_prompt, stream)
         else:
             async with OpenAIClient(ClientMode.ASYNC) as client:
                 new_prompt = await self._arun_with_client(client, evaled_prompt, stream)
         self._post_check_output(stream, run_config, new_prompt)
         return new_prompt
@@ -454,17 +319,17 @@
             output_path = Path(output_path, template_filename)
         # format output_path with the current time
         output_path = start_time.strftime(str(output_path))
         # create the parent directory if it does not exist
         Path(output_path).parent.mkdir(parents=True, exist_ok=True)
         return output_path
     
-    def _prepare_run(self: PromptType, run_config: RunConfig, kwargs: dict):
+    def _prepare_run(self: PromptType, run_config: RunConfig, var_map: Optional[Dict], kwargs: dict):
         # evaluate the prompt with the given run_config
-        evaled_prompt = self.eval(run_config=run_config, **kwargs)
+        evaled_prompt = self.eval(run_config=run_config, var_map=var_map, **kwargs)
         evaled_run_config = evaled_prompt.run_config
         evaled_request = evaled_prompt.request
         
         # get the stream flag
         stream = evaled_request.get("stream", False)
         
         # verbose output
@@ -509,18 +374,18 @@
                 new_prompt.dump(run_config.output_fd)
             elif run_config.output_path:
                 new_prompt.dump_to(run_config.output_path)
         return new_prompt
 
     def _merge_non_data(self: PromptType, other: PromptType, inplace=False) -> Union[None, tuple[dict, RunConfig]]:
         if inplace:
-            merge(self.request, other.request, strategy=Strategy.ADDITIVE)
+            merge_dict(self.request, other.request, strategy=Strategy.ADDITIVE)
             self.run_config.merge(other.run_config, inplace=True)
         else:
-            merged_request = merge({}, self.request, other.request, strategy=Strategy.ADDITIVE)
+            merged_request = merge_dict({}, self.request, other.request, strategy=Strategy.ADDITIVE)
             merged_run_config = self.run_config.merge(other.run_config)
             return merged_request, merged_run_config
     
     @staticmethod
     def _filter_request(
         request: dict, 
         run_config: RunConfig,
@@ -541,21 +406,21 @@
             for key in real_blacklist:
                 request.pop(key, None)
         return request
     
     def _parse_var_map(self, run_config: RunConfig):
         var_map = {}
         if run_config.var_map_path:
-            var_map = merge(
+            var_map = merge_dict(
                 var_map, 
                 load_var_map(run_config.var_map_path), 
                 strategy=Strategy.REPLACE
             )
         if run_config.var_map:
-            var_map = merge(
+            var_map = merge_dict(
                 var_map, 
                 run_config.var_map, 
                 strategy=Strategy.REPLACE
             )
         return var_map
 
 
@@ -586,14 +451,31 @@
         return converter.msgs2raw(data)
     
     def _eval_data(self, run_config: RunConfig) -> list:
         var_map = self._parse_var_map(run_config)
         return converter.msgs_replace_variables(
             self.messages, var_map, inplace=False)
     
+    @staticmethod
+    def _wrap_gen_chat(response, run_config: RunConfig):
+        for role, content, tool_call in stream_chat_all(response):
+            if run_config.on_chunk:
+                run_config.on_chunk(role, content, tool_call)
+            yield role, content, tool_call
+    
+    @staticmethod
+    async def _awrap_gen_chat(response, run_config: RunConfig):
+        async for role, content, tool_call in astream_chat_all(response):
+            if run_config.on_chunk:
+                if inspect.iscoroutinefunction(run_config.on_chunk):
+                    await run_config.on_chunk(role, content, tool_call)
+                else:
+                    run_config.on_chunk(role, content, tool_call)
+            yield role, content, tool_call
+
     @classmethod
     def _run_with_client(
         cls, 
         client: OpenAIClient, 
         evaled_prompt: PromptType,
         stream: bool,
         ) -> ChatPrompt:
@@ -605,23 +487,31 @@
             ).call()
         base_path = Path(run_config.output_path).parent.resolve() if run_config.output_path else None
         if stream:
             if run_config.output_fd:
                 # dump frontmatter, no base_path
                 run_config.output_fd.write(cls._dumps_frontmatter(new_request, run_config))
                 # stream response to a file descriptor
-                role, content, tool_calls = converter.stream_msgs2raw(stream_chat_all(response), run_config.output_fd)
+                role, content, tool_calls = converter.stream_msgs2raw(
+                    cls._wrap_gen_chat(response, run_config), 
+                    run_config.output_fd
+                    )
             elif run_config.output_path:
                 # stream response to a file
                 with open(run_config.output_path, 'w', encoding='utf-8') as fout:
                     # dump frontmatter
                     fout.write(cls._dumps_frontmatter(new_request, run_config, base_path))
-                    role, content, tool_calls = converter.stream_msgs2raw(stream_chat_all(response), fout)
+                    role, content, tool_calls = converter.stream_msgs2raw(
+                        cls._wrap_gen_chat(response, run_config), 
+                        fout
+                        )
             else:
-                role, content, tool_calls = converter.stream_msgs2raw(stream_chat_all(response))
+                role, content, tool_calls = converter.stream_msgs2raw(
+                    cls._wrap_gen_chat(response, run_config)
+                    )
         else:
             role = response['choices'][0]['message']['role']
             content = response['choices'][0]['message'].get('content')
             tool_calls = response['choices'][0]['message'].get('tool_calls')
         return ChatPrompt(
             [{"role": role, "content": content, "tool_calls": tool_calls}],
             new_request, run_config, base_path,
@@ -642,22 +532,30 @@
             **new_request
             ).acall()
         base_path = Path(run_config.output_path).parent.resolve() if run_config.output_path else None
         if stream:
             if run_config.output_fd:
                 # stream response to a file descriptor
                 run_config.output_fd.write(cls._dumps_frontmatter(new_request, run_config))
-                role, content, tool_calls = await converter.astream_msgs2raw(astream_chat_all(response), run_config.output_fd)
+                role, content, tool_calls = await converter.astream_msgs2raw(
+                    cls._awrap_gen_chat(response, run_config), 
+                    run_config.output_fd
+                    )
             elif run_config.output_path:
                 # stream response to a file
                 with open(run_config.output_path, 'w', encoding='utf-8') as fout:
                     fout.write(cls._dumps_frontmatter(new_request, run_config, base_path))
-                    role, content, tool_calls = await converter.astream_msgs2raw(astream_chat_all(response), fout)
+                    role, content, tool_calls = await converter.astream_msgs2raw(
+                        cls._awrap_gen_chat(response, run_config), 
+                        fout
+                        )
             else:
-                role, content, tool_calls = await converter.astream_msgs2raw(astream_chat_all(response))
+                role, content, tool_calls = await converter.astream_msgs2raw(
+                    cls._awrap_gen_chat(response, run_config)
+                    )
         else:
             role = response['choices'][0]['message']['role']
             content = response['choices'][0]['message'].get('content')
             tool_calls = response['choices'][0]['message'].get('tool_calls')
         return ChatPrompt(
             [{"role": role, "content": content, "tool_calls": tool_calls}],
             new_request, run_config, base_path,
@@ -726,18 +624,20 @@
         var_map = self._parse_var_map(run_config)
         new_prompt = self.prompt
         for key, value in var_map.items():
             new_prompt = new_prompt.replace(key, value)
         return new_prompt
     
     @staticmethod
-    def _stream_completions_proc(response, fd: Optional[io.IOBase] = None) -> str:
+    def _stream_completions_proc(response, run_config: RunConfig, fd: Optional[io.IOBase] = None) -> str:
         # stream response to fd
         content = ""
         for text in stream_completions(response):
+            if run_config.on_chunk:
+                run_config.on_chunk(text)
             if fd:
                 fd.write(text)
             content += text
         return content
 
     @classmethod
     def _run_with_client(
@@ -753,33 +653,38 @@
             **new_request
             ).call()
         base_path = Path(run_config.output_path).parent.resolve() if run_config.output_path else None
         if stream:
             if run_config.output_fd:
                 # stream response to a file descriptor
                 run_config.output_fd.write(cls._dumps_frontmatter(new_request, run_config))
-                content = cls._stream_completions_proc(response, run_config.output_fd)
+                content = cls._stream_completions_proc(response, run_config, run_config.output_fd)
             elif run_config.output_path:
                 # stream response to a file
                 with open(run_config.output_path, 'w', encoding='utf-8') as fout:
-                    fout.write(cls._dumps_frontmatter(new_request, run_config, base_path))
+                    fout.write(cls._dumps_frontmatter(new_request, run_config, run_config, base_path))
                     content = cls._stream_completions_proc(response, fout)
             else:
-                content = cls._stream_completions_proc(response)
+                content = cls._stream_completions_proc(response, run_config)
         else:
             content = response['choices'][0]['text']
         return CompletionsPrompt(
             content, new_request, run_config, base_path, response=response
             )
 
     @staticmethod
-    async def _astream_completions_proc(response, fd: Optional[io.IOBase] = None) -> str:
+    async def _astream_completions_proc(response, run_config: RunConfig, fd: Optional[io.IOBase] = None) -> str:
         # stream response to fd
         content = ""
         async for text in astream_completions(response):
+            if run_config.on_chunk:
+                if inspect.iscoroutinefunction(run_config.on_chunk):
+                    await run_config.on_chunk(text)
+                else:
+                    run_config.on_chunk(text)
             if fd:
                 fd.write(text)
             content += text
         return content
     
     @classmethod
     async def _arun_with_client(
@@ -795,22 +700,22 @@
             **new_request
             ).acall()
         base_path = Path(run_config.output_path).parent.resolve() if run_config.output_path else None
         if stream:
             if run_config.output_fd:
                 # stream response to a file descriptor
                 run_config.output_fd.write(cls._dumps_frontmatter(new_request, run_config))
-                content = await cls._astream_completions_proc(response, run_config.output_fd)
+                content = await cls._astream_completions_proc(response, run_config, run_config.output_fd)
             elif run_config.output_path:
                 # stream response to a file
                 with open(run_config.output_path, 'w', encoding='utf-8') as fout:
                     fout.write(cls._dumps_frontmatter(new_request, run_config, base_path))
-                    content = await cls._astream_completions_proc(response, fout)
+                    content = await cls._astream_completions_proc(response, run_config, fout)
             else:
-                content = await cls._astream_completions_proc(response)
+                content = await cls._astream_completions_proc(response, run_config)
         else:
             content = response['choices'][0]['text']
         return CompletionsPrompt(
             content, new_request, run_config, base_path, response=response
             )
     
     def __add__(self, other: Union[str, CompletionsPrompt]):
```

### Comparing `handyllm-0.7.5/src/handyllm/openai_api.py` & `handyllm-0.7.6/src/handyllm/openai_api.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.5/src/handyllm/openai_client.py` & `handyllm-0.7.6/src/handyllm/openai_client.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.5/src/handyllm/prompt_converter.py` & `handyllm-0.7.6/src/handyllm/prompt_converter.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.5/src/handyllm/requestor.py` & `handyllm-0.7.6/src/handyllm/requestor.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.5/src/handyllm/utils.py` & `handyllm-0.7.6/src/handyllm/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -119,7 +119,13 @@
 async def astream_to_fd(response, fd: io.IOBase):
     async for data in response:
         fd.write(data)
 
 async def astream_to_file(response, file_path):
     with open(file_path, 'wb') as f:
         await astream_to_fd(response, f)
+
+def VM(**kwargs):
+    # transform kwargs to a variable map dict
+    # change each key to a % wrapped string
+    transformed_vm = {f'%{key}%': value for key, value in kwargs.items()}
+    return transformed_vm
```

### Comparing `handyllm-0.7.5/tests/test_azure.py` & `handyllm-0.7.6/tests/test_azure.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.5/tests/test_client_async_sync.py` & `handyllm-0.7.6/tests/test_client_async_sync.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.5/tests/test_endpoint.py` & `handyllm-0.7.6/tests/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.5/tests/test_hprompt.py` & `handyllm-0.7.6/tests/test_hprompt.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.5/tests/test_prompt.py` & `handyllm-0.7.6/tests/test_prompt.py`

 * *Files identical despite different names*

