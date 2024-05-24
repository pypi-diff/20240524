# Comparing `tmp/hamming_sdk-0.0.5.tar.gz` & `tmp/hamming_sdk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hamming_sdk-0.0.5.tar", last modified: Sat May 18 23:45:46 2024, max compression
+gzip compressed data, was "hamming_sdk-0.0.6.tar", last modified: Fri May 24 01:03:52 2024, max compression
```

## Comparing `hamming_sdk-0.0.5.tar` & `hamming_sdk-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-05-18 23:45:46.753833 hamming_sdk-0.0.5/
--rw-r--r--   0 marius     (501) staff       (20)     1074 2024-02-11 14:45:52.000000 hamming_sdk-0.0.5/LICENSE
--rw-r--r--   0 marius     (501) staff       (20)      988 2024-05-18 23:45:46.753611 hamming_sdk-0.0.5/PKG-INFO
--rw-r--r--   0 marius     (501) staff       (20)      414 2024-02-19 20:22:09.000000 hamming_sdk-0.0.5/README.md
--rw-r--r--   0 marius     (501) staff       (20)      647 2024-05-18 23:45:32.000000 hamming_sdk-0.0.5/pyproject.toml
--rw-r--r--   0 marius     (501) staff       (20)       38 2024-05-18 23:45:46.753871 hamming_sdk-0.0.5/setup.cfg
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-05-18 23:45:46.748804 hamming_sdk-0.0.5/src/
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-05-18 23:45:46.750967 hamming_sdk-0.0.5/src/hamming/
--rw-r--r--   0 marius     (501) staff       (20)       46 2024-02-13 02:06:22.000000 hamming_sdk-0.0.5/src/hamming/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)      879 2024-03-01 03:07:45.000000 hamming_sdk-0.0.5/src/hamming/framework.py
--rw-r--r--   0 marius     (501) staff       (20)     1601 2024-02-15 01:54:38.000000 hamming_sdk-0.0.5/src/hamming/http_client.py
--rw-r--r--   0 marius     (501) staff       (20)     6944 2024-03-01 03:07:45.000000 hamming_sdk-0.0.5/src/hamming/oai.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-05-18 23:45:46.752563 hamming_sdk-0.0.5/src/hamming/resources/
--rw-r--r--   0 marius     (501) staff       (20)      122 2024-03-01 03:07:45.000000 hamming_sdk-0.0.5/src/hamming/resources/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)      251 2024-03-01 03:07:45.000000 hamming_sdk-0.0.5/src/hamming/resources/api_resource.py
--rw-r--r--   0 marius     (501) staff       (20)      701 2024-03-01 03:07:45.000000 hamming_sdk-0.0.5/src/hamming/resources/datasets.py
--rw-r--r--   0 marius     (501) staff       (20)     4102 2024-05-18 23:45:32.000000 hamming_sdk-0.0.5/src/hamming/resources/experiments.py
--rw-r--r--   0 marius     (501) staff       (20)     2561 2024-03-27 03:15:06.000000 hamming_sdk-0.0.5/src/hamming/resources/logger.py
--rw-r--r--   0 marius     (501) staff       (20)     4355 2024-03-01 03:07:45.000000 hamming_sdk-0.0.5/src/hamming/resources/monitoring.py
--rw-r--r--   0 marius     (501) staff       (20)     3505 2024-03-27 03:15:06.000000 hamming_sdk-0.0.5/src/hamming/resources/tracing.py
--rw-r--r--   0 marius     (501) staff       (20)     4276 2024-03-01 03:07:45.000000 hamming_sdk-0.0.5/src/hamming/types.py
--rw-r--r--   0 marius     (501) staff       (20)      148 2024-02-14 04:37:24.000000 hamming_sdk-0.0.5/src/hamming/utils.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-05-18 23:45:46.753415 hamming_sdk-0.0.5/src/hamming_sdk.egg-info/
--rw-r--r--   0 marius     (501) staff       (20)      988 2024-05-18 23:45:46.000000 hamming_sdk-0.0.5/src/hamming_sdk.egg-info/PKG-INFO
--rw-r--r--   0 marius     (501) staff       (20)      607 2024-05-18 23:45:46.000000 hamming_sdk-0.0.5/src/hamming_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 marius     (501) staff       (20)        1 2024-05-18 23:45:46.000000 hamming_sdk-0.0.5/src/hamming_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 marius     (501) staff       (20)       33 2024-05-18 23:45:46.000000 hamming_sdk-0.0.5/src/hamming_sdk.egg-info/requires.txt
--rw-r--r--   0 marius     (501) staff       (20)        8 2024-05-18 23:45:46.000000 hamming_sdk-0.0.5/src/hamming_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-05-24 01:03:52.473662 hamming_sdk-0.0.6/
+-rw-r--r--   0 marius     (501) staff       (20)     1074 2024-02-11 14:45:52.000000 hamming_sdk-0.0.6/LICENSE
+-rw-r--r--   0 marius     (501) staff       (20)      988 2024-05-24 01:03:52.473458 hamming_sdk-0.0.6/PKG-INFO
+-rw-r--r--   0 marius     (501) staff       (20)      414 2024-02-19 20:22:09.000000 hamming_sdk-0.0.6/README.md
+-rw-r--r--   0 marius     (501) staff       (20)      647 2024-05-24 01:03:38.000000 hamming_sdk-0.0.6/pyproject.toml
+-rw-r--r--   0 marius     (501) staff       (20)       38 2024-05-24 01:03:52.473696 hamming_sdk-0.0.6/setup.cfg
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-05-24 01:03:52.468296 hamming_sdk-0.0.6/src/
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-05-24 01:03:52.470548 hamming_sdk-0.0.6/src/hamming/
+-rw-r--r--   0 marius     (501) staff       (20)       46 2024-02-13 02:06:22.000000 hamming_sdk-0.0.6/src/hamming/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)      879 2024-03-01 03:07:45.000000 hamming_sdk-0.0.6/src/hamming/framework.py
+-rw-r--r--   0 marius     (501) staff       (20)     1601 2024-02-15 01:54:38.000000 hamming_sdk-0.0.6/src/hamming/http_client.py
+-rw-r--r--   0 marius     (501) staff       (20)     6944 2024-03-01 03:07:45.000000 hamming_sdk-0.0.6/src/hamming/oai.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-05-24 01:03:52.472449 hamming_sdk-0.0.6/src/hamming/resources/
+-rw-r--r--   0 marius     (501) staff       (20)      122 2024-03-01 03:07:45.000000 hamming_sdk-0.0.6/src/hamming/resources/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)      251 2024-03-01 03:07:45.000000 hamming_sdk-0.0.6/src/hamming/resources/api_resource.py
+-rw-r--r--   0 marius     (501) staff       (20)      701 2024-03-01 03:07:45.000000 hamming_sdk-0.0.6/src/hamming/resources/datasets.py
+-rw-r--r--   0 marius     (501) staff       (20)     4816 2024-05-24 01:01:37.000000 hamming_sdk-0.0.6/src/hamming/resources/experiments.py
+-rw-r--r--   0 marius     (501) staff       (20)     2561 2024-03-27 03:15:06.000000 hamming_sdk-0.0.6/src/hamming/resources/logger.py
+-rw-r--r--   0 marius     (501) staff       (20)     4355 2024-03-01 03:07:45.000000 hamming_sdk-0.0.6/src/hamming/resources/monitoring.py
+-rw-r--r--   0 marius     (501) staff       (20)     2351 2024-05-24 01:01:37.000000 hamming_sdk-0.0.6/src/hamming/resources/scoring.py
+-rw-r--r--   0 marius     (501) staff       (20)     3505 2024-03-27 03:15:06.000000 hamming_sdk-0.0.6/src/hamming/resources/tracing.py
+-rw-r--r--   0 marius     (501) staff       (20)     5686 2024-05-24 01:01:37.000000 hamming_sdk-0.0.6/src/hamming/types.py
+-rw-r--r--   0 marius     (501) staff       (20)      148 2024-02-14 04:37:24.000000 hamming_sdk-0.0.6/src/hamming/utils.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2024-05-24 01:03:52.473275 hamming_sdk-0.0.6/src/hamming_sdk.egg-info/
+-rw-r--r--   0 marius     (501) staff       (20)      988 2024-05-24 01:03:52.000000 hamming_sdk-0.0.6/src/hamming_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 marius     (501) staff       (20)      640 2024-05-24 01:03:52.000000 hamming_sdk-0.0.6/src/hamming_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 marius     (501) staff       (20)        1 2024-05-24 01:03:52.000000 hamming_sdk-0.0.6/src/hamming_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 marius     (501) staff       (20)       33 2024-05-24 01:03:52.000000 hamming_sdk-0.0.6/src/hamming_sdk.egg-info/requires.txt
+-rw-r--r--   0 marius     (501) staff       (20)        8 2024-05-24 01:03:52.000000 hamming_sdk-0.0.6/src/hamming_sdk.egg-info/top_level.txt
```

### Comparing `hamming_sdk-0.0.5/LICENSE` & `hamming_sdk-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hamming_sdk-0.0.5/PKG-INFO` & `hamming_sdk-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hamming-sdk
-Version: 0.0.5
+Version: 0.0.6
 Summary: SDK for interacting with Hamming AI platform
 Author-email: Hamming <contact@hamming.ai>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hamming_sdk-0.0.5/pyproject.toml` & `hamming_sdk-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hamming-sdk"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Hamming", email="contact@hamming.ai" },
 ]
 description = "SDK for interacting with Hamming AI platform"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `hamming_sdk-0.0.5/src/hamming/framework.py` & `hamming_sdk-0.0.6/src/hamming/framework.py`

 * *Files identical despite different names*

### Comparing `hamming_sdk-0.0.5/src/hamming/http_client.py` & `hamming_sdk-0.0.6/src/hamming/http_client.py`

 * *Files identical despite different names*

### Comparing `hamming_sdk-0.0.5/src/hamming/oai.py` & `hamming_sdk-0.0.6/src/hamming/oai.py`

 * *Files identical despite different names*

### Comparing `hamming_sdk-0.0.5/src/hamming/resources/datasets.py` & `hamming_sdk-0.0.6/src/hamming/resources/datasets.py`

 * *Files identical despite different names*

### Comparing `hamming_sdk-0.0.5/src/hamming/resources/experiments.py` & `hamming_sdk-0.0.6/src/hamming/resources/experiments.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import inspect
 from datetime import datetime
-from typing import Optional
+from typing import Optional, Dict
 
 from ..types import (
     DatasetItem,
     Experiment,
     ExperimentItem,
     ExperimentItemContext,
     ExperimentStatus,
@@ -13,17 +13,20 @@
     MetadataType,
     OutputType,
     Runner,
     RunOptions,
     RunResult,
     ScoreType,
     TracingMode,
+    Score,
+    CustomScoringConfig,
 )
-from ..utils import get_url_origin
 from .api_resource import APIResource
+from .scoring import ScoringHelper
+from ..utils import get_url_origin
 
 DEFAULT_SCORE_TYPES: list[ScoreType] = [ScoreType.STRING_DIFF]
 
 
 class ExperimentItems(APIResource):
     def start(
         self, experiment: Experiment, dataset_item: DatasetItem
@@ -33,27 +36,34 @@
             f"/experiments/{experiment.id}/items",
             json={"datasetItemId": dataset_item.id, "output": {}, "metrics": {}},
         )
         item = ExperimentItem(**resp_data["item"])
         item_context = ExperimentItemContext(item=item, startTs=datetime.now())
         return item_context
 
-    def end(self, item_context: ExperimentItemContext, output: OutputType):
+    def end(self, 
+        item_context: ExperimentItemContext, 
+        output: OutputType,
+        scores: Dict[str, Score]
+    ):
         item = item_context.item
         start_ts = item_context.startTs
         duration_sec = (datetime.now() - start_ts).total_seconds()
         duration_ms = int(duration_sec * 1000)
 
         self._client.tracing._flush(item.id)
+
         self._client.request(
             "PATCH",
             f"/experiments/{item.experimentId}/items/{item.id}",
             json={
                 "output": output,
-                "scores": {}, # TODO: Custom Scores
+                "scores": {
+                    key: value.model_dump() for key, value in scores.items()
+                },
                 "metrics": {"durationMs": duration_ms},
             },
         )
 
 
 class Experiments(APIResource):
     _items: ExperimentItems
@@ -75,51 +85,67 @@
         dataset_id = opts.dataset
         dataset = self._client.datasets.load(dataset_id)
 
         name = opts.name or Experiments.generate_name(dataset.name)
         scoring = opts.scoring or DEFAULT_SCORE_TYPES
         metadata = opts.metadata or {}
 
+        scoring_helper = ScoringHelper(self._client, scoring)
+        scoring_helper.initialize()
+
         def execute_runner(run: Runner, input: InputType) -> OutputType:
             if inspect.iscoroutinefunction(run):
                 return asyncio.run(run(input))
             else:
                 return run(input)
 
-        experiment = self._start(name, dataset_id, scoring, metadata)
+        experiment = self._start(
+            name, 
+            dataset_id, 
+            scoring_helper.get_config(), 
+            metadata
+        )
         url_origin = get_url_origin(self._client.base_url)
         experiment_url = f"{url_origin}/experiments/{experiment.id}"
 
         try:
             for dataset_item in dataset.items:
                 item_context = self._items.start(experiment, dataset_item)
                 output = execute_runner(run, dataset_item.input)
-                self._items.end(item_context, output)
+                scores = scoring_helper.score(
+                    dataset_item.input,
+                    dataset_item.output,
+                    output,
+                )
+                self._items.end(item_context, output, scores)
             self._end(experiment)
             return RunResult(url=experiment_url)
         except Exception as ex:
             self._end(experiment, status=ExperimentStatus.FAILED)
             raise ex
 
     def _start(
         self,
         name: str,
         dataset_id: str,
-        scoring: list[ScoreType],
+        scoring: list[ScoreType | CustomScoringConfig],
         metadata: MetadataType,
     ) -> Experiment:
         status = ExperimentStatus.RUNNING
+        scoring_obj = [
+            s.model_dump() if type(s) == CustomScoringConfig else s for s in scoring
+        ]
         resp_data = self._client.request(
             "POST",
             "/experiments",
             json={
                 "name": name,
                 "dataset": dataset_id,
                 "status": status,
-                "scoring": scoring,
+                "scoring": scoring_obj,
                 "metadata": metadata,
             },
         )
         return Experiment(**resp_data["experiment"])
 
     def _end(
         self,
```

### Comparing `hamming_sdk-0.0.5/src/hamming/resources/logger.py` & `hamming_sdk-0.0.6/src/hamming/resources/logger.py`

 * *Files identical despite different names*

### Comparing `hamming_sdk-0.0.5/src/hamming/resources/monitoring.py` & `hamming_sdk-0.0.6/src/hamming/resources/monitoring.py`

 * *Files identical despite different names*

### Comparing `hamming_sdk-0.0.5/src/hamming/resources/tracing.py` & `hamming_sdk-0.0.6/src/hamming/resources/tracing.py`

 * *Files identical despite different names*

### Comparing `hamming_sdk-0.0.5/src/hamming/types.py` & `hamming_sdk-0.0.6/src/hamming/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,21 +35,14 @@
 
 
 InputType: TypeAlias = Dict
 OutputType: TypeAlias = Dict
 MetadataType: TypeAlias = Dict
 
 
-class RunOptions(BaseModel):
-    dataset: str
-    name: Optional[str]
-    scoring: Optional[list[ScoreType]]
-    metadata: Optional[MetadataType]
-
-
 Runner: TypeAlias = Union[
     Callable[[InputType], OutputType], Callable[[InputType], Awaitable[OutputType]]
 ]
 
 
 class RunResult(BaseModel):
     url: str
@@ -197,13 +190,82 @@
 
 class LogMessageType(int, Enum):
     Monitoring = 1
 
 
 class LogMessage(BaseModel):
     type: LogMessageType
-    payload: Union[MonitoringTrace]
+    payload: MonitoringTrace
 
 class TracingMode(Enum):
     OFF = "off"
     MONITORING = "monitoring"
     EXPERIMENT = "experiment"
+
+class Score(BaseModel):
+    value: float
+    reason: Optional[str]
+
+class FunctionType(str, Enum):
+    NUMERIC = "numeric"
+    CLASSIFICATION = "classification"
+
+class FunctionAggregateType(str, Enum):
+    MEAN = "mean"
+    MEDIAN = "median"
+
+class LabelColor(str, Enum):
+    GRAY = "gray"
+    LIGHT_GREEN = "light-green"
+    LIGHT_BLUE = "light-blue"
+    AMBER = "amber"
+    PURPLE = "purple"
+    PINK = "pink"
+    GREEN = "green"
+    PASTEL_GREEN = "pastel-green"
+    YELLOW = "yellow"
+    BLUE = "blue"
+    RED = "red"
+
+class NumericScoreConfig(BaseModel):
+    type: FunctionType = FunctionType.NUMERIC
+    aggregate: FunctionAggregateType
+
+class ClassificationScoreConfig(BaseModel):
+    type: FunctionType = FunctionType.CLASSIFICATION
+    labels: Dict[int, str]
+    colors: Optional[Dict[int, LabelColor]]
+
+ScoreConfig = Union[NumericScoreConfig, ClassificationScoreConfig]
+
+
+class ScorerExecutionType(str, Enum):
+    LOCAL = "local"
+    REMOTE = "remote"
+
+class ScoreArgs(BaseModel):
+    input: InputType
+    output: OutputType
+    expected: OutputType
+
+class LocalScorer(BaseModel):
+    type: ScorerExecutionType = ScorerExecutionType.LOCAL
+    score_fn: Callable[[ScoreArgs], Score]
+
+Scorer = LocalScorer
+
+class ScoringFunction(BaseModel):
+    name: str
+    version: int
+    score_config: ScoreConfig
+    scorer: Scorer
+
+class CustomScoringConfig(BaseModel):
+    id: str
+    key_name: str
+
+
+class RunOptions(BaseModel):
+    dataset: str
+    name: Optional[str]
+    scoring: Optional[list[ScoreType | ScoringFunction]]
+    metadata: Optional[MetadataType]
```

### Comparing `hamming_sdk-0.0.5/src/hamming_sdk.egg-info/PKG-INFO` & `hamming_sdk-0.0.6/src/hamming_sdk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hamming-sdk
-Version: 0.0.5
+Version: 0.0.6
 Summary: SDK for interacting with Hamming AI platform
 Author-email: Hamming <contact@hamming.ai>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hamming_sdk-0.0.5/src/hamming_sdk.egg-info/SOURCES.txt` & `hamming_sdk-0.0.6/src/hamming_sdk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,13 +9,14 @@
 src/hamming/utils.py
 src/hamming/resources/__init__.py
 src/hamming/resources/api_resource.py
 src/hamming/resources/datasets.py
 src/hamming/resources/experiments.py
 src/hamming/resources/logger.py
 src/hamming/resources/monitoring.py
+src/hamming/resources/scoring.py
 src/hamming/resources/tracing.py
 src/hamming_sdk.egg-info/PKG-INFO
 src/hamming_sdk.egg-info/SOURCES.txt
 src/hamming_sdk.egg-info/dependency_links.txt
 src/hamming_sdk.egg-info/requires.txt
 src/hamming_sdk.egg-info/top_level.txt
```

