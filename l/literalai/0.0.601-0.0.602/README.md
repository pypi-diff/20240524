# Comparing `tmp/literalai-0.0.601.tar.gz` & `tmp/literalai-0.0.602.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "literalai-0.0.601.tar", last modified: Mon May 13 13:05:50 2024, max compression
+gzip compressed data, was "literalai-0.0.602.tar", last modified: Fri May 24 10:01:09 2024, max compression
```

## Comparing `literalai-0.0.601.tar` & `literalai-0.0.602.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:50.921444 literalai-0.0.601/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 13:05:39.000000 literalai-0.0.601/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-13 13:05:50.921444 literalai-0.0.601/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-13 13:05:39.000000 literalai-0.0.601/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:50.917444 literalai-0.0.601/literalai/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:50.917444 literalai-0.0.601/literalai/api/
--rw-r--r--   0 runner    (1001) docker     (127)    84378 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/api/attachment_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/api/dataset_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/api/generation_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20998 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/api/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/api/prompt_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/api/score_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/api/step_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/api/thread_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/api/user_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:50.921444 literalai-0.0.601/literalai/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17193 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/callback/langchain_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/callback/llama_index_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/dataset_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/event_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:50.921444 literalai-0.0.601/literalai/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18454 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/instrumentation/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/my_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)    10115 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:50.917444 literalai-0.0.601/literalai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-13 13:05:50.000000 literalai-0.0.601/literalai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-13 13:05:50.000000 literalai-0.0.601/literalai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:05:50.000000 literalai-0.0.601/literalai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-13 13:05:50.000000 literalai-0.0.601/literalai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 13:05:50.000000 literalai-0.0.601/literalai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:05:50.921444 literalai-0.0.601/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-13 13:05:39.000000 literalai-0.0.601/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:50.921444 literalai-0.0.601/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:39.000000 literalai-0.0.601/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:01:09.036695 literalai-0.0.602/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 10:01:01.000000 literalai-0.0.602/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-24 10:01:09.036695 literalai-0.0.602/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-24 10:01:01.000000 literalai-0.0.602/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:01:09.032695 literalai-0.0.602/literalai/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:01:09.032695 literalai-0.0.602/literalai/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    84883 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/api/attachment_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/api/dataset_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/api/generation_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20968 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/api/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/api/prompt_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/api/score_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/api/step_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/api/thread_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/api/user_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:01:09.032695 literalai-0.0.602/literalai/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17193 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/callback/langchain_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/callback/llama_index_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/dataset_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/event_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:01:09.036695 literalai-0.0.602/literalai/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18454 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/instrumentation/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12560 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/my_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:01:09.032695 literalai-0.0.602/literalai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-24 10:01:08.000000 literalai-0.0.602/literalai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-24 10:01:09.000000 literalai-0.0.602/literalai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 10:01:08.000000 literalai-0.0.602/literalai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-24 10:01:08.000000 literalai-0.0.602/literalai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-24 10:01:08.000000 literalai-0.0.602/literalai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 10:01:09.036695 literalai-0.0.602/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-24 10:01:01.000000 literalai-0.0.602/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:01:09.036695 literalai-0.0.602/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 10:01:01.000000 literalai-0.0.602/tests/__init__.py
```

### Comparing `literalai-0.0.601/LICENSE` & `literalai-0.0.602/LICENSE`

 * *Files identical despite different names*

### Comparing `literalai-0.0.601/README.md` & `literalai-0.0.602/README.md`

 * *Files identical despite different names*

### Comparing `literalai-0.0.601/literalai/api/__init__.py` & `literalai-0.0.602/literalai/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 from literalai.dataset import DatasetType
 from literalai.dataset_experiment import DatasetExperiment, DatasetExperimentItem
 from literalai.filter import (
     generations_filters,
     generations_order_by,
     scores_filters,
     scores_order_by,
+    steps_filters,
+    steps_order_by,
     threads_filters,
     threads_order_by,
     users_filters,
 )
-
-from literalai.filter import steps_filters, steps_order_by
 from literalai.prompt import Prompt, ProviderSettings
 
 from .attachment_helpers import (
     AttachmentUpload,
     create_attachment_helper,
     delete_attachment_helper,
     get_attachment_helper,
@@ -1289,14 +1289,26 @@
         if id:
             return self.gql_helper(*get_prompt_helper(self, id=id))
         elif name:
             return self.gql_helper(*get_prompt_helper(self, name=name, version=version))
         else:
             raise ValueError("Either the `id` or the `name` must be provided.")
 
+    # Misc API
+
+    def get_my_project_id(self):
+        """
+        Retrieves the projectId associated to the API key.
+
+        Returns:
+            The projectId associated to the API key.
+        """
+        response = self.make_rest_call("/my-project", {})
+        return response["projectId"]
+
 
 class AsyncLiteralAPI(BaseLiteralAPI):
     R = TypeVar("R")
 
     async def make_gql_call(
         self, description: str, query: str, variables: Dict[str, Any]
     ) -> Dict:
@@ -2425,7 +2437,15 @@
             return await self.gql_helper(
                 *get_prompt_helper(sync_api, name=name, version=version)
             )
         else:
             raise ValueError("Either the `id` or the `name` must be provided.")
 
     get_prompt.__doc__ = LiteralAPI.get_prompt.__doc__
+
+    # Misc API
+
+    async def get_my_project_id(self):
+        response = await self.make_rest_call("/my-project", {})
+        return response["projectId"]
+
+    get_my_project_id.__doc__ = LiteralAPI.get_my_project_id.__doc__
```

### Comparing `literalai-0.0.601/literalai/api/attachment_helpers.py` & `literalai-0.0.602/literalai/api/attachment_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.601/literalai/api/dataset_helpers.py` & `literalai-0.0.602/literalai/api/dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.601/literalai/api/generation_helpers.py` & `literalai-0.0.602/literalai/api/generation_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.601/literalai/api/gql.py` & `literalai-0.0.602/literalai/api/gql.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 STEP_FIELDS = """
         id
         threadId
         parentId
         startTime
         endTime
         createdAt
-        participantIdentifier
         type
         error
         input
         output
         metadata
         scores {
             id
```

### Comparing `literalai-0.0.601/literalai/api/prompt_helpers.py` & `literalai-0.0.602/literalai/api/prompt_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.601/literalai/api/score_helpers.py` & `literalai-0.0.602/literalai/api/score_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.601/literalai/api/step_helpers.py` & `literalai-0.0.602/literalai/api/step_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.601/literalai/api/thread_helpers.py` & `literalai-0.0.602/literalai/api/thread_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.601/literalai/api/user_helpers.py` & `literalai-0.0.602/literalai/api/user_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.601/literalai/callback/langchain_callback.py` & `literalai-0.0.602/literalai/callback/langchain_callback.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.601/literalai/callback/llama_index_callback.py` & `literalai-0.0.602/literalai/callback/llama_index_callback.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.601/literalai/client.py` & `literalai-0.0.602/literalai/client.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.601/literalai/dataset.py` & `literalai-0.0.602/literalai/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import sys
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Dict, List, Literal, Optional
 
+from literalai.my_types import Utils
+
 if sys.version_info < (3, 12):
     from typing_extensions import TypedDict
 else:
     from typing import TypedDict
 
 if TYPE_CHECKING:
     from literalai.api import LiteralAPI
@@ -22,16 +24,16 @@
     metadata: Dict
     name: Optional[str]
     description: Optional[str]
     items: Optional[List[DatasetItemDict]]
     type: DatasetType
 
 
-@dataclass
-class Dataset:
+@dataclass(repr=False)
+class Dataset(Utils):
     api: "LiteralAPI"
     id: str
     created_at: str
     metadata: Dict
     name: Optional[str] = None
     description: Optional[str] = None
     items: List[DatasetItem] = field(default_factory=lambda: [])
```

### Comparing `literalai-0.0.601/literalai/dataset_experiment.py` & `literalai-0.0.602/literalai/dataset_experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from dataclasses import dataclass, field
 from typing import Dict, List, Optional, TypedDict
 from typing import TYPE_CHECKING
 
-from literalai.my_types import ScoreDict
+from literalai.my_types import ScoreDict, Utils
 
 if TYPE_CHECKING:
     from literalai.api import LiteralAPI
 
 
 class DatasetExperimentItemDict(TypedDict, total=False):
     id: str
     datasetExperimentId: str
     datasetItemId: str
     scores: List[ScoreDict]
     input: Optional[Dict]
     output: Optional[Dict]
 
 
-@dataclass
-class DatasetExperimentItem:
+@dataclass(repr=False)
+class DatasetExperimentItem(Utils):
     id: str
     dataset_experiment_id: str
     dataset_item_id: str
     scores: List[ScoreDict]
     input: Optional[Dict]
     output: Optional[Dict]
 
@@ -54,16 +54,16 @@
     name: str
     datasetId: str
     params: Dict
     promptId: Optional[str]
     items: Optional[List[DatasetExperimentItemDict]]
 
 
-@dataclass
-class DatasetExperiment:
+@dataclass(repr=False)
+class DatasetExperiment(Utils):
     api: "LiteralAPI"
     id: str
     created_at: str
     name: str
     dataset_id: str
     params: Optional[Dict]
     prompt_id: Optional[str] = None
```

### Comparing `literalai-0.0.601/literalai/dataset_item.py` & `literalai-0.0.602/literalai/dataset_item.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from dataclasses import dataclass
 from typing import Dict, List, Optional, TypedDict
 
+from literalai.my_types import Utils
+
 
 class DatasetItemDict(TypedDict, total=False):
     id: str
     createdAt: str
     datasetId: str
     metadata: Dict
     input: Dict
     expectedOutput: Optional[Dict]
     intermediarySteps: Optional[List[Dict]]
 
 
-@dataclass
-class DatasetItem:
+@dataclass(repr=False)
+class DatasetItem(Utils):
     id: str
     created_at: str
     dataset_id: str
     metadata: Dict
     input: Dict
     expected_output: Optional[Dict] = None
     intermediary_steps: Optional[List[Dict]] = None
```

### Comparing `literalai-0.0.601/literalai/event_processor.py` & `literalai-0.0.602/literalai/event_processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     ctx = contextvars.copy_context()
     func_call = functools.partial(ctx.run, func, *args, **kwargs)
     return await loop.run_in_executor(None, func_call)
 
 
 class EventProcessor:
     event_queue: queue.Queue
+    batch: List["StepDict"]
+
 
     def __init__(self, api: "LiteralAPI", batch_size: int = 5, disabled: bool = False):
         self.batch_size = batch_size
         self.api = api
         self.event_queue = queue.Queue()
         self.processing_thread = threading.Thread(
             target=self._process_events, daemon=True
@@ -45,55 +47,55 @@
         self.event_queue.put(event)
 
     async def a_add_events(self, event: "StepDict"):
         await to_thread(self.event_queue.put, event)
 
     def _process_events(self):
         while True:
-            batch: List["StepDict"] = []
+            self.batch = []
             try:
                 # Try to fill the batch up to the batch_size
-                while len(batch) < self.batch_size:
+                while len(self.batch) < self.batch_size:
                     # Attempt to get events with a timeout
                     event = self.event_queue.get(timeout=0.5)
-                    batch.append(event)
+                    self.batch.append(event)
             except queue.Empty:
                 # No more events at the moment, proceed with processing what's in the batch
                 pass
 
             # Process the batch if any events are present - in a separate thread
-            if batch:
-                self._process_batch(batch)
+            if self.batch:
+                self._process_batch()
 
             # Stop if the stop_event is set and the queue is empty
             if self.stop_event.is_set() and self.event_queue.empty():
                 break
 
-    def _try_process_batch(self, batch):
+    def _try_process_batch(self):
         try:
-            return self.api.send_steps(batch)
+            return self.api.send_steps(self.batch)
         except Exception:
             logger.error(f"Failed to send steps: {traceback.format_exc()}")
         return None
 
-    def _process_batch(self, batch):
+    def _process_batch(self):
         # Simple one-try retry in case of network failure (no retry on graphql errors)
         retries = 0
-        while not self._try_process_batch(batch) and retries < 1:
+        while not self._try_process_batch() and retries < 1:
             retries += 1
             time.sleep(DEFAULT_SLEEP_TIME)
 
     def flush_and_stop(self):
         self.stop_event.set()
         if not self.disabled:
             self.processing_thread.join()
 
     async def aflush(self):
         while not self.event_queue.empty():
             await asyncio.sleep(DEFAULT_SLEEP_TIME)
 
     def flush(self):
-        while not self.event_queue.empty():
+        while not self.event_queue.empty() or len(self.batch) > 0:
             time.sleep(0.2)
 
     def __del__(self):
         self.flush_and_stop()
```

### Comparing `literalai-0.0.601/literalai/filter.py` & `literalai-0.0.602/literalai/filter.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.601/literalai/helper.py` & `literalai-0.0.602/literalai/helper.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.601/literalai/instrumentation/openai.py` & `literalai-0.0.602/literalai/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.601/literalai/message.py` & `literalai-0.0.602/literalai/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from typing import TYPE_CHECKING, Dict, List, Optional
 
 if TYPE_CHECKING:
     from literalai.event_processor import EventProcessor
 
 from literalai.context import active_steps_var, active_thread_var
 from literalai.helper import utc_now
-from literalai.my_types import Attachment, Score
+from literalai.my_types import Attachment, Score, Utils
 from literalai.step import MessageStepType, StepDict
 
 
-class Message:
+class Message(Utils):
     id: Optional[str] = None
     name: Optional[str] = None
     type: Optional[MessageStepType] = None
     metadata: Optional[Dict] = {}
     parent_id: Optional[str] = None
     timestamp: Optional[str] = None
     content: str
```

### Comparing `literalai-0.0.601/literalai/my_types.py` & `literalai-0.0.602/literalai/my_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 import sys
 import uuid
+import json
 from enum import Enum, unique
 from typing import Any, Dict, Generic, List, Literal, Optional, Protocol, TypeVar, Union
 
 if sys.version_info < (3, 12):
     from typing_extensions import TypedDict
 else:
     from typing import TypedDict
 
 from pydantic.dataclasses import Field, dataclass
 
 GenerationMessageRole = Literal["user", "assistant", "tool", "function", "system"]
 ScoreType = Literal["HUMAN", "AI"]
 
 
-@dataclass
-class PageInfo:
+class Utils:
+    def __str__(self):
+        return json.dumps(self.to_dict(), sort_keys=True, indent=4)
+
+    def __repr__(self):
+        return json.dumps(self.to_dict(), sort_keys=True, indent=4)
+
+@dataclass(repr=False)
+class PageInfo(Utils):
     hasNextPage: bool
     startCursor: Optional[str]
     endCursor: Optional[str]
 
     def to_dict(self):
         return {
             "hasNextPage": self.hasNextPage,
@@ -42,16 +50,16 @@
 
 class HasFromDict(Protocol[T]):
     @classmethod
     def from_dict(cls, obj_dict: Any) -> T:
         raise NotImplementedError()
 
 
-@dataclass
-class PaginatedResponse(Generic[T]):
+@dataclass(repr=False)
+class PaginatedResponse(Generic[T], Utils):
     pageInfo: PageInfo
     data: List[T]
     totalCount: Optional[int] = None
 
     def to_dict(self):
         return {
             "pageInfo": self.pageInfo.to_dict(),
@@ -95,16 +103,16 @@
     role: Optional[GenerationMessageRole]
     content: Optional[Union[str, List[Union[TextContent, ImageUrlContent]]]]
     function_call: Optional[Dict]
     tool_calls: Optional[List[Dict]]
     tool_call_id: Optional[str]
 
 
-@dataclass
-class BaseGeneration:
+@dataclass(repr=False)
+class BaseGeneration(Utils):
     id: Optional[str] = None
     prompt_id: Optional[str] = None
     provider: Optional[str] = None
     model: Optional[str] = None
     error: Optional[str] = None
     settings: Optional[Dict] = Field(default_factory=dict)
     variables: Optional[Dict] = Field(default_factory=dict)
@@ -144,16 +152,16 @@
             "outputTokenCount": self.output_token_count,
             "ttFirstToken": self.tt_first_token,
             "tokenThroughputInSeconds": self.token_throughput_in_s,
             "duration": self.duration,
         }
 
 
-@dataclass
-class CompletionGeneration(BaseGeneration):
+@dataclass(repr=False)
+class CompletionGeneration(BaseGeneration, Utils):
     prompt: Optional[str] = None
     completion: Optional[str] = None
     type = GenerationType.COMPLETION
 
     def to_dict(self):
         _dict = super().to_dict()
         _dict.update(
@@ -184,16 +192,16 @@
             token_throughput_in_s=generation_dict.get("tokenThroughputInSeconds"),
             duration=generation_dict.get("duration"),
             prompt=generation_dict.get("prompt"),
             completion=generation_dict.get("completion"),
         )
 
 
-@dataclass
-class ChatGeneration(BaseGeneration):
+@dataclass(repr=False)
+class ChatGeneration(BaseGeneration, Utils):
     type = GenerationType.CHAT
     messages: Optional[List[GenerationMessage]] = Field(default_factory=list)
     message_completion: Optional[GenerationMessage] = None
 
     def to_dict(self):
         _dict = super().to_dict()
         _dict.update(
@@ -247,16 +255,16 @@
     metadata: Optional[Dict]
     mime: Optional[str]
     name: Optional[str]
     objectKey: Optional[str]
     url: Optional[str]
 
 
-@dataclass
-class Score:
+@dataclass(repr=False)
+class Score(Utils):
     name: str
     type: ScoreType
     value: float
     step_id: Optional[str]
     generation_id: Optional[str]
     dataset_experiment_item_id: Optional[str]
     comment: Optional[str]
@@ -299,16 +307,16 @@
             comment=comment,
             tags=tags,
         )
 
         return score
 
 
-@dataclass
-class Attachment:
+@dataclass(repr=False)
+class Attachment(Utils):
     step_id: Optional[str] = None
     thread_id: Optional[str] = None
     id: Optional[str] = Field(default_factory=lambda: str(uuid.uuid4()))
     metadata: Optional[Dict] = Field(default_factory=lambda: {})
     mime: Optional[str] = None
     name: Optional[str] = None
     object_key: Optional[str] = None
@@ -352,16 +360,16 @@
 class UserDict(TypedDict, total=False):
     id: Optional[str]
     metadata: Optional[Dict]
     identifier: Optional[str]
     createdAt: Optional[str]
 
 
-@dataclass
-class User:
+@dataclass(repr=False)
+class User(Utils):
     id: Optional[str] = None
     created_at: Optional[str] = None
     identifier: Optional[str] = Field(default_factory=lambda: str(uuid.uuid4()))
     metadata: Dict = Field(default_factory=lambda: {})
 
     def to_dict(self) -> UserDict:
         return {
```

### Comparing `literalai-0.0.601/literalai/prompt.py` & `literalai-0.0.602/literalai/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from typing import TypedDict
 
 import chevron
 
 if TYPE_CHECKING:
     from literalai.api import LiteralAPI
 
-from literalai.my_types import GenerationMessage, GenerationType
+from literalai.my_types import GenerationMessage, GenerationType, Utils
 
 
 class ProviderSettings(TypedDict, total=False):
     provider: str
     model: str
     frequency_penalty: float
     max_tokens: int
@@ -58,16 +58,16 @@
     tools: Optional[List[Dict]]
     provider: str
     settings: ProviderSettings
     variables: List[PromptVariable]
     variablesDefaultValues: Optional[Dict[str, Any]]
 
 
-@dataclass
-class Prompt:
+@dataclass(repr=False)
+class Prompt(Utils):
     api: "LiteralAPI"
     id: str
     created_at: str
     updated_at: str
     type: "GenerationType"
     name: str
     version: int
```

### Comparing `literalai-0.0.601/literalai/requirements.py` & `literalai-0.0.602/literalai/requirements.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.601/literalai/step.py` & `literalai-0.0.602/literalai/step.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import inspect
-import json
 import uuid
 from copy import deepcopy
 from functools import wraps
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
@@ -25,14 +24,15 @@
     Attachment,
     AttachmentDict,
     BaseGeneration,
     ChatGeneration,
     CompletionGeneration,
     Score,
     ScoreDict,
+    Utils,
 )
 
 TrueStepType = Literal[
     "run", "tool", "llm", "embedding", "retrieval", "rerank", "undefined"
 ]
 
 MessageStepType = Literal["user_message", "assistant_message", "system_message"]
@@ -55,15 +55,15 @@
     startTime: Optional[str]
     endTime: Optional[str]
     generation: Optional[Dict]
     scores: Optional[List[ScoreDict]]
     attachments: Optional[List[AttachmentDict]]
 
 
-class Step:
+class Step(Utils):
     id: Optional[str] = None
     name: Optional[str] = ""
     type: Optional[StepType] = None
     metadata: Optional[Dict] = None
     parent_id: Optional[str] = None
     start_time: Optional[str] = None
     end_time: Optional[str] = None
@@ -157,17 +157,14 @@
             "generation": self.generation.to_dict() if self.generation else None,
             "name": self.name,
             "tags": self.tags,
             "scores": [score.to_dict() for score in self.scores],
             "attachments": [attachment.to_dict() for attachment in self.attachments],
         }
 
-    def __repr__(self):
-        return json.dumps(self.to_dict(), sort_keys=True, indent=4)
-
     @classmethod
     def from_dict(cls, step_dict: StepDict) -> "Step":
         name = step_dict.get("name") or ""
         step_type = step_dict.get("type", "undefined")
         thread_id = step_dict.get("threadId")
 
         step = cls(name=name, type=step_type, thread_id=thread_id)
```

### Comparing `literalai-0.0.601/literalai/thread.py` & `literalai-0.0.602/literalai/thread.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import traceback
 import uuid
 from functools import wraps
 from typing import TYPE_CHECKING, Callable, Dict, List, Optional, TypedDict
 
 from literalai.context import active_thread_var
-from literalai.my_types import UserDict
+from literalai.my_types import UserDict, Utils
 from literalai.step import Step, StepDict
 
 if TYPE_CHECKING:
     from literalai.client import BaseLiteralClient
 
 logger = logging.getLogger(__name__)
 
@@ -21,15 +21,15 @@
     metadata: Optional[Dict]
     tags: Optional[List[str]]
     createdAt: Optional[str]
     steps: Optional[List[StepDict]]
     participant: Optional[UserDict]
 
 
-class Thread:
+class Thread(Utils):
     id: str
     name: Optional[str]
     metadata: Optional[Dict]
     tags: Optional[List[str]]
     steps: Optional[List[Step]]
     participant_id: Optional[str]
     participant_identifier: Optional[str] = None
```

### Comparing `literalai-0.0.601/literalai/wrappers.py` & `literalai-0.0.602/literalai/wrappers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.601/literalai.egg-info/SOURCES.txt` & `literalai-0.0.602/literalai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

