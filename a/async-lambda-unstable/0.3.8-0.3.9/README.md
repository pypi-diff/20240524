# Comparing `tmp/async-lambda-unstable-0.3.8.tar.gz` & `tmp/async-lambda-unstable-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-lambda-unstable-0.3.8.tar", last modified: Fri Apr 19 11:17:09 2024, max compression
+gzip compressed data, was "async-lambda-unstable-0.3.9.tar", last modified: Tue Apr 30 20:58:19 2024, max compression
```

## Comparing `async-lambda-unstable-0.3.8.tar` & `async-lambda-unstable-0.3.9.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-19 11:17:09.464626 async-lambda-unstable-0.3.8/
--rw-r--r--   0 henryjones   (501) staff       (20)    15801 2024-04-19 11:17:09.464357 async-lambda-unstable-0.3.8/PKG-INFO
--rw-r--r--   0 henryjones   (501) staff       (20)    15541 2024-04-18 15:16:55.000000 async-lambda-unstable-0.3.8/README.md
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-19 11:17:09.461396 async-lambda-unstable-0.3.8/async_lambda/
--rw-r--r--   0 henryjones   (501) staff       (20)      726 2024-04-19 11:11:11.000000 async-lambda-unstable-0.3.8/async_lambda/__init__.py
--rw-r--r--   0 henryjones   (501) staff       (20)     3388 2024-04-18 10:25:44.000000 async-lambda-unstable-0.3.8/async_lambda/build_config.py
--rw-r--r--   0 henryjones   (501) staff       (20)    11395 2024-04-18 10:25:44.000000 async-lambda-unstable-0.3.8/async_lambda/cli.py
--rw-r--r--   0 henryjones   (501) staff       (20)      750 2024-03-15 17:38:55.000000 async-lambda-unstable-0.3.8/async_lambda/client.py
--rw-r--r--   0 henryjones   (501) staff       (20)      350 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.8/async_lambda/config.py
--rw-r--r--   0 henryjones   (501) staff       (20)    19117 2024-04-18 15:06:27.000000 async-lambda-unstable-0.3.8/async_lambda/controller.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1206 2024-04-19 11:10:54.000000 async-lambda-unstable-0.3.8/async_lambda/defer.py
--rw-r--r--   0 henryjones   (501) staff       (20)      809 2024-04-18 10:34:41.000000 async-lambda-unstable-0.3.8/async_lambda/env.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-19 11:17:09.461633 async-lambda-unstable-0.3.8/async_lambda/models/
--rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.8/async_lambda/models/__init__.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-19 11:17:09.462674 async-lambda-unstable-0.3.8/async_lambda/models/events/
--rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.8/async_lambda/models/events/__init__.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1118 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.8/async_lambda/models/events/api_event.py
--rw-r--r--   0 henryjones   (501) staff       (20)      929 2024-03-15 17:38:55.000000 async-lambda-unstable-0.3.8/async_lambda/models/events/base_event.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1884 2024-03-18 21:28:52.000000 async-lambda-unstable-0.3.8/async_lambda/models/events/managed_sqs_event.py
--rw-r--r--   0 henryjones   (501) staff       (20)       77 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.8/async_lambda/models/events/scheduled_event.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1086 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.8/async_lambda/models/events/unmanaged_sqs_event.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-19 11:17:09.462941 async-lambda-unstable-0.3.8/async_lambda/models/mock/
--rw-r--r--   0 henryjones   (501) staff       (20)      508 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.8/async_lambda/models/mock/mock_context.py
--rw-r--r--   0 henryjones   (501) staff       (20)     2030 2024-03-25 19:06:55.000000 async-lambda-unstable-0.3.8/async_lambda/models/mock/mock_event.py
--rw-r--r--   0 henryjones   (501) staff       (20)    18748 2024-04-18 14:49:06.000000 async-lambda-unstable-0.3.8/async_lambda/models/task.py
--rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.8/async_lambda/py.typed
--rw-r--r--   0 henryjones   (501) staff       (20)      514 2024-04-18 10:25:44.000000 async-lambda-unstable-0.3.8/async_lambda/util.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-19 11:17:09.464045 async-lambda-unstable-0.3.8/async_lambda_unstable.egg-info/
--rw-r--r--   0 henryjones   (501) staff       (20)    15801 2024-04-19 11:17:09.000000 async-lambda-unstable-0.3.8/async_lambda_unstable.egg-info/PKG-INFO
--rw-r--r--   0 henryjones   (501) staff       (20)      932 2024-04-19 11:17:09.000000 async-lambda-unstable-0.3.8/async_lambda_unstable.egg-info/SOURCES.txt
--rw-r--r--   0 henryjones   (501) staff       (20)        1 2024-04-19 11:17:09.000000 async-lambda-unstable-0.3.8/async_lambda_unstable.egg-info/dependency_links.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       54 2024-04-19 11:17:09.000000 async-lambda-unstable-0.3.8/async_lambda_unstable.egg-info/entry_points.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       73 2024-04-19 11:17:09.000000 async-lambda-unstable-0.3.8/async_lambda_unstable.egg-info/requires.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       13 2024-04-19 11:17:09.000000 async-lambda-unstable-0.3.8/async_lambda_unstable.egg-info/top_level.txt
--rw-r--r--   0 henryjones   (501) staff       (20)      849 2024-04-19 11:10:24.000000 async-lambda-unstable-0.3.8/pyproject.toml
--rw-r--r--   0 henryjones   (501) staff       (20)       38 2024-04-19 11:17:09.464687 async-lambda-unstable-0.3.8/setup.cfg
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-30 20:58:19.947016 async-lambda-unstable-0.3.9/
+-rw-r--r--   0 henryjones   (501) staff       (20)    15801 2024-04-30 20:58:19.946722 async-lambda-unstable-0.3.9/PKG-INFO
+-rw-r--r--   0 henryjones   (501) staff       (20)    15541 2024-04-30 20:57:54.000000 async-lambda-unstable-0.3.9/README.md
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-30 20:58:19.942615 async-lambda-unstable-0.3.9/async_lambda/
+-rw-r--r--   0 henryjones   (501) staff       (20)      799 2024-04-30 20:57:54.000000 async-lambda-unstable-0.3.9/async_lambda/__init__.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     3388 2024-04-18 10:25:44.000000 async-lambda-unstable-0.3.9/async_lambda/build_config.py
+-rw-r--r--   0 henryjones   (501) staff       (20)    11395 2024-04-18 10:25:44.000000 async-lambda-unstable-0.3.9/async_lambda/cli.py
+-rw-r--r--   0 henryjones   (501) staff       (20)      750 2024-03-15 17:38:55.000000 async-lambda-unstable-0.3.9/async_lambda/client.py
+-rw-r--r--   0 henryjones   (501) staff       (20)      350 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.9/async_lambda/config.py
+-rw-r--r--   0 henryjones   (501) staff       (20)    20318 2024-04-30 20:57:54.000000 async-lambda-unstable-0.3.9/async_lambda/controller.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1206 2024-04-30 20:57:54.000000 async-lambda-unstable-0.3.9/async_lambda/defer.py
+-rw-r--r--   0 henryjones   (501) staff       (20)      809 2024-04-30 20:57:54.000000 async-lambda-unstable-0.3.9/async_lambda/env.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-30 20:58:19.943034 async-lambda-unstable-0.3.9/async_lambda/models/
+-rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.9/async_lambda/models/__init__.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-30 20:58:19.944793 async-lambda-unstable-0.3.9/async_lambda/models/events/
+-rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.9/async_lambda/models/events/__init__.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1118 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.9/async_lambda/models/events/api_event.py
+-rw-r--r--   0 henryjones   (501) staff       (20)      929 2024-03-15 17:38:55.000000 async-lambda-unstable-0.3.9/async_lambda/models/events/base_event.py
+-rw-r--r--   0 henryjones   (501) staff       (20)      519 2024-04-30 20:57:54.000000 async-lambda-unstable-0.3.9/async_lambda/models/events/dynamodb_event.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1884 2024-03-18 21:28:52.000000 async-lambda-unstable-0.3.9/async_lambda/models/events/managed_sqs_event.py
+-rw-r--r--   0 henryjones   (501) staff       (20)       77 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.9/async_lambda/models/events/scheduled_event.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1086 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.9/async_lambda/models/events/unmanaged_sqs_event.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-30 20:58:19.945288 async-lambda-unstable-0.3.9/async_lambda/models/mock/
+-rw-r--r--   0 henryjones   (501) staff       (20)      508 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.9/async_lambda/models/mock/mock_context.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     2030 2024-03-25 19:06:55.000000 async-lambda-unstable-0.3.9/async_lambda/models/mock/mock_event.py
+-rw-r--r--   0 henryjones   (501) staff       (20)    19335 2024-04-30 20:57:54.000000 async-lambda-unstable-0.3.9/async_lambda/models/task.py
+-rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-12-11 20:47:05.000000 async-lambda-unstable-0.3.9/async_lambda/py.typed
+-rw-r--r--   0 henryjones   (501) staff       (20)      514 2024-04-18 10:25:44.000000 async-lambda-unstable-0.3.9/async_lambda/util.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2024-04-30 20:58:19.946511 async-lambda-unstable-0.3.9/async_lambda_unstable.egg-info/
+-rw-r--r--   0 henryjones   (501) staff       (20)    15801 2024-04-30 20:58:19.000000 async-lambda-unstable-0.3.9/async_lambda_unstable.egg-info/PKG-INFO
+-rw-r--r--   0 henryjones   (501) staff       (20)      977 2024-04-30 20:58:19.000000 async-lambda-unstable-0.3.9/async_lambda_unstable.egg-info/SOURCES.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)        1 2024-04-30 20:58:19.000000 async-lambda-unstable-0.3.9/async_lambda_unstable.egg-info/dependency_links.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)       54 2024-04-30 20:58:19.000000 async-lambda-unstable-0.3.9/async_lambda_unstable.egg-info/entry_points.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)       73 2024-04-30 20:58:19.000000 async-lambda-unstable-0.3.9/async_lambda_unstable.egg-info/requires.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)       13 2024-04-30 20:58:19.000000 async-lambda-unstable-0.3.9/async_lambda_unstable.egg-info/top_level.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)      849 2024-04-30 20:57:54.000000 async-lambda-unstable-0.3.9/pyproject.toml
+-rw-r--r--   0 henryjones   (501) staff       (20)       38 2024-04-30 20:58:19.947073 async-lambda-unstable-0.3.9/setup.cfg
```

### Comparing `async-lambda-unstable-0.3.8/PKG-INFO` & `async-lambda-unstable-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-lambda-unstable
-Version: 0.3.8
+Version: 0.3.9
 Summary: A framework for creating AWS Lambda Async Workflows. - Unstable Branch
 Author-email: "Nuclei, Inc" <engineering@nuclei.ai>
 Description-Content-Type: text/markdown
 Provides-Extra: local
 
 # async-lambda
```

### Comparing `async-lambda-unstable-0.3.8/README.md` & `async-lambda-unstable-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.8/async_lambda/__init__.py` & `async-lambda-unstable-0.3.9/async_lambda/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,12 +2,13 @@
 from .config import config_set_runtime as config_set_runtime
 from .controller import AsyncLambdaController as AsyncLambdaController
 from .defer import Defer as Defer
 from .env import disable_force_sync_mode as disable_force_sync_mode
 from .env import enable_force_sync_mode as enable_force_sync_mode
 from .env import is_build_mode as is_build_mode
 from .models.events.api_event import APIEvent as APIEvent
+from .models.events.dynamodb_event import DynamoDBEvent as DynamoDBEvent
 from .models.events.managed_sqs_event import ManagedSQSEvent as ManagedSQSEvent
 from .models.events.scheduled_event import ScheduledEvent as ScheduledEvent
 from .models.events.unmanaged_sqs_event import UnmanagedSQSEvent as UnmanagedSQSEvent
 
-__version__ = "0.3.8"
+__version__ = "0.3.9"
```

### Comparing `async-lambda-unstable-0.3.8/async_lambda/build_config.py` & `async-lambda-unstable-0.3.9/async_lambda/build_config.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.8/async_lambda/cli.py` & `async-lambda-unstable-0.3.9/async_lambda/cli.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.8/async_lambda/client.py` & `async-lambda-unstable-0.3.9/async_lambda/client.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.8/async_lambda/controller.py` & `async-lambda-unstable-0.3.9/async_lambda/controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Any, Callable, Dict, Optional, Tuple
 from uuid import uuid4
 
 from . import env
 from .build_config import get_build_config_for_stage
 from .client import get_s3_client, get_sqs_client
 from .models.events.api_event import APIEvent
+from .models.events.dynamodb_event import DynamoDBEvent
 from .models.events.managed_sqs_event import ManagedSQSEvent
 from .models.events.scheduled_event import ScheduledEvent
 from .models.events.unmanaged_sqs_event import UnmanagedSQSEvent
 from .models.mock.mock_context import MockLambdaContext
 from .models.mock.mock_event import MockSQSLambdaEvent
 from .models.task import AsyncLambdaTask, TaskTriggerType
 from .util import make_cf_tags
@@ -234,14 +235,16 @@
             self.set_current_invocation_id(_event.invocation_id)
         elif task.trigger_type == TaskTriggerType.UNMANAGED_SQS:
             _event = UnmanagedSQSEvent(*args)
         elif task.trigger_type == TaskTriggerType.SCHEDULED_EVENT:
             _event = ScheduledEvent(*args)
         elif task.trigger_type == TaskTriggerType.API_EVENT:
             _event = APIEvent(*args)
+        elif task.trigger_type == TaskTriggerType.DYNAMODB_EVENT:
+            _event = DynamoDBEvent(*args)
         else:
             raise NotImplementedError(
                 f"Trigger type of {task.trigger_type} is not supported."
             )
         response = task.execute(_event)
         if isinstance(_event, ManagedSQSEvent) and _event.s3_payload_key is not None:
             get_s3_client().delete_object(
@@ -521,7 +524,36 @@
                     **kwargs,
                 )
             )
 
             return inner
 
         return _task
+
+    def dynamodb_task(self, task_id: str, *, stream_arn: str, batch_size: int):
+        """
+        Decorate a function to register it as a DynamoDB task.
+        These tasks will be triggered by the given DynamoDB stream.
+        """
+        logger.debug(
+            f"Registered dynamodb task '{task_id}' with stream_arn '{stream_arn}' and batch_size '{batch_size}' with the controller."
+        )
+
+        def _task(func: Callable[[DynamoDBEvent], Any]):
+            @functools.wraps(func)
+            def inner(*args, **kwargs):
+                self.set_current_task_id(task_id)
+                return func(*args, **kwargs)
+
+            self.add_task(
+                AsyncLambdaTask(
+                    controller=self,
+                    executable=inner,
+                    task_id=task_id,
+                    trigger_type=TaskTriggerType.DYNAMODB_EVENT,
+                    trigger_config={"stream_arn": stream_arn, "batch_size": batch_size},
+                )
+            )
+
+            return inner
+
+        return _task
```

### Comparing `async-lambda-unstable-0.3.8/async_lambda/defer.py` & `async-lambda-unstable-0.3.9/async_lambda/defer.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.8/async_lambda/env.py` & `async-lambda-unstable-0.3.9/async_lambda/env.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.8/async_lambda/models/events/api_event.py` & `async-lambda-unstable-0.3.9/async_lambda/models/events/api_event.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.8/async_lambda/models/events/base_event.py` & `async-lambda-unstable-0.3.9/async_lambda/models/events/base_event.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.8/async_lambda/models/events/managed_sqs_event.py` & `async-lambda-unstable-0.3.9/async_lambda/models/events/managed_sqs_event.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.8/async_lambda/models/events/unmanaged_sqs_event.py` & `async-lambda-unstable-0.3.9/async_lambda/models/events/unmanaged_sqs_event.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.8/async_lambda/models/mock/mock_event.py` & `async-lambda-unstable-0.3.9/async_lambda/models/mock/mock_event.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.8/async_lambda/models/task.py` & `async-lambda-unstable-0.3.9/async_lambda/models/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,31 @@
 from .. import env
 from ..build_config import get_build_config_for_task
 from ..config import config
 
 if TYPE_CHECKING:
     from ..controller import AsyncLambdaController  # pragma: not covered
 
+from .events.dynamodb_event import DynamoDBEvent
 from .events.managed_sqs_event import ManagedSQSEvent
 from .events.scheduled_event import ScheduledEvent
 from .events.unmanaged_sqs_event import UnmanagedSQSEvent
 
 
 class TaskTriggerType(Enum):
     MANAGED_SQS = 1
     UNMANAGED_SQS = 2
     SCHEDULED_EVENT = 3
     API_EVENT = 4
+    DYNAMODB_EVENT = 5
 
 
 EventType = TypeVar(
-    "EventType", bound=Union[ManagedSQSEvent, ScheduledEvent, UnmanagedSQSEvent]
+    "EventType",
+    bound=Union[ManagedSQSEvent, ScheduledEvent, UnmanagedSQSEvent, DynamoDBEvent],
 )
 
 
 class AsyncLambdaTask(Generic[EventType]):
     controller: "AsyncLambdaController"
     task_id: str
     trigger_type: TaskTriggerType
@@ -258,14 +261,26 @@
                     "Properties": {
                         "Path": self.trigger_config["path"],
                         "Method": self.trigger_config["method"].lower(),
                         "RestApiId": {"Ref": "AsyncLambdaAPIGateway"},
                     },
                 }
             }
+        elif self.trigger_type == TaskTriggerType.DYNAMODB_EVENT:
+            return {
+                "DynamoDBEvent": {
+                    "Type": "DynamoDB",
+                    "Properties": {
+                        "Stream": self.trigger_config["stream_arn"],
+                        "StartingPosition": "TRIM_HORIZON",
+                        "BatchSize": self.trigger_config["batch_size"],
+                        "Enabled": True,
+                    },
+                }
+            }
         raise NotImplementedError()
 
     def get_policy_sqs_resources(self) -> List[dict]:
         if self.trigger_type == TaskTriggerType.MANAGED_SQS:
             return [
                 {
                     "Fn::GetAtt": [
```

### Comparing `async-lambda-unstable-0.3.8/async_lambda/util.py` & `async-lambda-unstable-0.3.9/async_lambda/util.py`

 * *Files identical despite different names*

### Comparing `async-lambda-unstable-0.3.8/async_lambda_unstable.egg-info/PKG-INFO` & `async-lambda-unstable-0.3.9/async_lambda_unstable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-lambda-unstable
-Version: 0.3.8
+Version: 0.3.9
 Summary: A framework for creating AWS Lambda Async Workflows. - Unstable Branch
 Author-email: "Nuclei, Inc" <engineering@nuclei.ai>
 Description-Content-Type: text/markdown
 Provides-Extra: local
 
 # async-lambda
```

### Comparing `async-lambda-unstable-0.3.8/async_lambda_unstable.egg-info/SOURCES.txt` & `async-lambda-unstable-0.3.9/async_lambda_unstable.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 async_lambda/py.typed
 async_lambda/util.py
 async_lambda/models/__init__.py
 async_lambda/models/task.py
 async_lambda/models/events/__init__.py
 async_lambda/models/events/api_event.py
 async_lambda/models/events/base_event.py
+async_lambda/models/events/dynamodb_event.py
 async_lambda/models/events/managed_sqs_event.py
 async_lambda/models/events/scheduled_event.py
 async_lambda/models/events/unmanaged_sqs_event.py
 async_lambda/models/mock/mock_context.py
 async_lambda/models/mock/mock_event.py
 async_lambda_unstable.egg-info/PKG-INFO
 async_lambda_unstable.egg-info/SOURCES.txt
```

### Comparing `async-lambda-unstable-0.3.8/pyproject.toml` & `async-lambda-unstable-0.3.9/pyproject.toml`

 * *Files identical despite different names*

