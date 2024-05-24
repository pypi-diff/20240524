# Comparing `tmp/automated_interpretability-0.0.3.tar.gz` & `tmp/automated_interpretability-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automated_interpretability-0.0.3.tar", max compression
+gzip compressed data, was "automated_interpretability-0.0.4.tar", max compression
```

## Comparing `automated_interpretability-0.0.3.tar` & `automated_interpretability-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0        0 2024-04-26 20:24:13.654582 automated_interpretability-0.0.3/neuron_explainer/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 20:24:13.654716 automated_interpretability-0.0.3/neuron_explainer/activations/__init__.py
--rw-r--r--   0        0        0     4751 2024-04-26 20:24:13.654851 automated_interpretability-0.0.3/neuron_explainer/activations/activation_records.py
--rw-r--r--   0        0        0    10808 2024-04-26 20:24:13.655025 automated_interpretability-0.0.3/neuron_explainer/activations/activations.py
--rw-r--r--   0        0        0     2179 2024-04-26 20:24:13.655130 automated_interpretability-0.0.3/neuron_explainer/activations/token_connections.py
--rw-r--r--   0        0        0     5455 2024-04-29 22:48:36.119355 automated_interpretability-0.0.3/neuron_explainer/api_client.py
--rw-r--r--   0        0        0      257 2024-04-26 20:24:13.655360 automated_interpretability-0.0.3/neuron_explainer/azure.py
--rw-r--r--   0        0        0        0 2024-04-26 20:24:13.655465 automated_interpretability-0.0.3/neuron_explainer/explanations/__init__.py
--rw-r--r--   0        0        0     7967 2024-04-26 20:24:13.655603 automated_interpretability-0.0.3/neuron_explainer/explanations/calibrated_simulator.py
--rw-r--r--   0        0        0    22224 2024-04-29 22:36:52.807527 automated_interpretability-0.0.3/neuron_explainer/explanations/explainer.py
--rw-r--r--   0        0        0     8867 2024-04-26 20:24:13.655965 automated_interpretability-0.0.3/neuron_explainer/explanations/explanations.py
--rw-r--r--   0        0        0    32989 2024-04-26 20:24:13.656149 automated_interpretability-0.0.3/neuron_explainer/explanations/few_shot_examples.py
--rw-r--r--   0        0        0     4698 2024-04-26 20:24:13.656293 automated_interpretability-0.0.3/neuron_explainer/explanations/prompt_builder.py
--rw-r--r--   0        0        0    52696 2024-04-26 20:24:13.656497 automated_interpretability-0.0.3/neuron_explainer/explanations/puzzles.json
--rw-r--r--   0        0        0     2178 2024-04-26 20:24:13.656717 automated_interpretability-0.0.3/neuron_explainer/explanations/puzzles.py
--rw-r--r--   0        0        0     5888 2024-04-26 20:24:13.656874 automated_interpretability-0.0.3/neuron_explainer/explanations/scoring.py
--rw-r--r--   0        0        0    45651 2024-04-27 05:42:47.856473 automated_interpretability-0.0.3/neuron_explainer/explanations/simulator.py
--rw-r--r--   0        0        0     6603 2024-04-26 20:24:13.657275 automated_interpretability-0.0.3/neuron_explainer/explanations/test_explainer.py
--rw-r--r--   0        0        0     7605 2024-04-26 20:24:13.657397 automated_interpretability-0.0.3/neuron_explainer/explanations/test_simulator.py
--rw-r--r--   0        0        0     4836 2024-04-26 20:24:13.657520 automated_interpretability-0.0.3/neuron_explainer/explanations/token_space_few_shot_examples.py
--rw-r--r--   0        0        0      147 2024-04-26 20:24:13.657701 automated_interpretability-0.0.3/neuron_explainer/fast_dataclasses/__init__.py
--rw-r--r--   0        0        0     3043 2024-04-26 20:24:13.657821 automated_interpretability-0.0.3/neuron_explainer/fast_dataclasses/fast_dataclasses.py
--rw-r--r--   0        0        0     2712 2024-04-26 20:24:13.657941 automated_interpretability-0.0.3/neuron_explainer/fast_dataclasses/test_fast_dataclasses.py
--rw-r--r--   0        0        0      467 2024-04-29 22:49:55.665812 automated_interpretability-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 automated_interpretability-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-24 20:16:50.301020 automated_interpretability-0.0.4/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-26 20:24:13.654582 automated_interpretability-0.0.4/neuron_explainer/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 20:24:13.654716 automated_interpretability-0.0.4/neuron_explainer/activations/__init__.py
+-rw-r--r--   0        0        0     4751 2024-04-26 20:24:13.654851 automated_interpretability-0.0.4/neuron_explainer/activations/activation_records.py
+-rw-r--r--   0        0        0    10808 2024-04-26 20:24:13.655025 automated_interpretability-0.0.4/neuron_explainer/activations/activations.py
+-rw-r--r--   0        0        0     2179 2024-04-26 20:24:13.655130 automated_interpretability-0.0.4/neuron_explainer/activations/token_connections.py
+-rw-r--r--   0        0        0     5455 2024-04-29 22:48:36.119355 automated_interpretability-0.0.4/neuron_explainer/api_client.py
+-rw-r--r--   0        0        0      257 2024-04-26 20:24:13.655360 automated_interpretability-0.0.4/neuron_explainer/azure.py
+-rw-r--r--   0        0        0        0 2024-04-26 20:24:13.655465 automated_interpretability-0.0.4/neuron_explainer/explanations/__init__.py
+-rw-r--r--   0        0        0     7967 2024-04-26 20:24:13.655603 automated_interpretability-0.0.4/neuron_explainer/explanations/calibrated_simulator.py
+-rw-r--r--   0        0        0    22416 2024-05-24 20:09:30.592482 automated_interpretability-0.0.4/neuron_explainer/explanations/explainer.py
+-rw-r--r--   0        0        0     8867 2024-04-26 20:24:13.655965 automated_interpretability-0.0.4/neuron_explainer/explanations/explanations.py
+-rw-r--r--   0        0        0    32989 2024-04-26 20:24:13.656149 automated_interpretability-0.0.4/neuron_explainer/explanations/few_shot_examples.py
+-rw-r--r--   0        0        0     4698 2024-04-26 20:24:13.656293 automated_interpretability-0.0.4/neuron_explainer/explanations/prompt_builder.py
+-rw-r--r--   0        0        0    52696 2024-04-26 20:24:13.656497 automated_interpretability-0.0.4/neuron_explainer/explanations/puzzles.json
+-rw-r--r--   0        0        0     2178 2024-04-26 20:24:13.656717 automated_interpretability-0.0.4/neuron_explainer/explanations/puzzles.py
+-rw-r--r--   0        0        0     5888 2024-04-26 20:24:13.656874 automated_interpretability-0.0.4/neuron_explainer/explanations/scoring.py
+-rw-r--r--   0        0        0    45651 2024-04-27 05:42:47.856473 automated_interpretability-0.0.4/neuron_explainer/explanations/simulator.py
+-rw-r--r--   0        0        0     6603 2024-04-26 20:24:13.657275 automated_interpretability-0.0.4/neuron_explainer/explanations/test_explainer.py
+-rw-r--r--   0        0        0     7605 2024-04-26 20:24:13.657397 automated_interpretability-0.0.4/neuron_explainer/explanations/test_simulator.py
+-rw-r--r--   0        0        0     4836 2024-04-26 20:24:13.657520 automated_interpretability-0.0.4/neuron_explainer/explanations/token_space_few_shot_examples.py
+-rw-r--r--   0        0        0      147 2024-04-26 20:24:13.657701 automated_interpretability-0.0.4/neuron_explainer/fast_dataclasses/__init__.py
+-rw-r--r--   0        0        0     3043 2024-04-26 20:24:13.657821 automated_interpretability-0.0.4/neuron_explainer/fast_dataclasses/fast_dataclasses.py
+-rw-r--r--   0        0        0     2712 2024-04-26 20:24:13.657941 automated_interpretability-0.0.4/neuron_explainer/fast_dataclasses/test_fast_dataclasses.py
+-rw-r--r--   0        0        0      467 2024-05-24 20:10:15.057177 automated_interpretability-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 automated_interpretability-0.0.4/PKG-INFO
```

### Comparing `automated_interpretability-0.0.3/neuron_explainer/activations/activation_records.py` & `automated_interpretability-0.0.4/neuron_explainer/activations/activation_records.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.3/neuron_explainer/activations/activations.py` & `automated_interpretability-0.0.4/neuron_explainer/activations/activations.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.3/neuron_explainer/activations/token_connections.py` & `automated_interpretability-0.0.4/neuron_explainer/activations/token_connections.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.3/neuron_explainer/api_client.py` & `automated_interpretability-0.0.4/neuron_explainer/api_client.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.3/neuron_explainer/explanations/calibrated_simulator.py` & `automated_interpretability-0.0.4/neuron_explainer/explanations/calibrated_simulator.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.3/neuron_explainer/explanations/explainer.py` & `automated_interpretability-0.0.4/neuron_explainer/explanations/explainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,31 +45,35 @@
     """Strip a final period or period-space from a string."""
     if text.endswith("."):
         return text[:-1]
     elif text.endswith(". "):
         return text[:-2]
     return text
 
-
+# TODO: should pull from API and/or combine with the HARMONY_V4_MODELS
 class ContextSize(int, Enum):
     TWO_K = 2049
     FOUR_K = 4097
     SIXTEEN_K = 16384
+    ONETWENTYEIGHT_K = 128000
 
     @classmethod
     def from_int(cls, i: int) -> ContextSize:
         for context_size in cls:
             if context_size.value == i:
                 return context_size
         raise ValueError(f"{i} is not a valid ContextSize")
 
-
+# TODO: should pull these from API
 HARMONY_V4_MODELS = [
     "gpt-3.5-turbo",
     "gpt-4",
+    "gpt-4o",
+    "gpt-4-turbo",
+    "gpt-4o-2024-05-13",
     "gpt-4-1106-preview",
     "gpt-4-turbo-2024-04-09",
 ]
 
 
 class NeuronExplainer(ABC):
     """
```

### Comparing `automated_interpretability-0.0.3/neuron_explainer/explanations/explanations.py` & `automated_interpretability-0.0.4/neuron_explainer/explanations/explanations.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.3/neuron_explainer/explanations/few_shot_examples.py` & `automated_interpretability-0.0.4/neuron_explainer/explanations/few_shot_examples.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.3/neuron_explainer/explanations/prompt_builder.py` & `automated_interpretability-0.0.4/neuron_explainer/explanations/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.3/neuron_explainer/explanations/puzzles.json` & `automated_interpretability-0.0.4/neuron_explainer/explanations/puzzles.json`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.3/neuron_explainer/explanations/puzzles.py` & `automated_interpretability-0.0.4/neuron_explainer/explanations/puzzles.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.3/neuron_explainer/explanations/scoring.py` & `automated_interpretability-0.0.4/neuron_explainer/explanations/scoring.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.3/neuron_explainer/explanations/simulator.py` & `automated_interpretability-0.0.4/neuron_explainer/explanations/simulator.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.3/neuron_explainer/explanations/test_explainer.py` & `automated_interpretability-0.0.4/neuron_explainer/explanations/test_explainer.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.3/neuron_explainer/explanations/test_simulator.py` & `automated_interpretability-0.0.4/neuron_explainer/explanations/test_simulator.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.3/neuron_explainer/explanations/token_space_few_shot_examples.py` & `automated_interpretability-0.0.4/neuron_explainer/explanations/token_space_few_shot_examples.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.3/neuron_explainer/fast_dataclasses/fast_dataclasses.py` & `automated_interpretability-0.0.4/neuron_explainer/fast_dataclasses/fast_dataclasses.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.3/neuron_explainer/fast_dataclasses/test_fast_dataclasses.py` & `automated_interpretability-0.0.4/neuron_explainer/fast_dataclasses/test_fast_dataclasses.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.3/PKG-INFO` & `automated_interpretability-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automated-interpretability
-Version: 0.0.3
+Version: 0.0.4
 Summary: OpenAI's implementation of automated-interpretability, with some updates. Not officially affiliated with OpenAI.
 Author: OpenAI
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

