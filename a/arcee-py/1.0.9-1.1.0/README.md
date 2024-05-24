# Comparing `tmp/arcee_py-1.0.9.tar.gz` & `tmp/arcee_py-1.1.0.tar.gz`

## Comparing `arcee_py-1.0.9.tar` & `arcee_py-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 arcee_py-1.0.9/.python-version
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 arcee_py-1.0.9/tasks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 arcee_py-1.0.9/.github/CODEOWNERS
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 arcee_py-1.0.9/.github/iced/test.yml
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 arcee_py-1.0.9/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 arcee_py-1.0.9/arcee/__init__.py
--rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 arcee_py-1.0.9/arcee/api.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 arcee_py-1.0.9/arcee/api_handler.py
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 arcee_py-1.0.9/arcee/cli.py
--rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 arcee_py-1.0.9/arcee/cli_handler.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 arcee_py-1.0.9/arcee/config.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 arcee_py-1.0.9/arcee/dalm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.9/arcee/schemas/__init__.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 arcee_py-1.0.9/arcee/schemas/doc.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 arcee_py-1.0.9/arcee/schemas/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.9/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.0.9/tests/conftest.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 arcee_py-1.0.9/tests/test_api_handler.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 arcee_py-1.0.9/.gitignore
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 arcee_py-1.0.9/README.md
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 arcee_py-1.0.9/pyproject.toml
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 arcee_py-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 arcee_py-1.1.0/.python-version
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 arcee_py-1.1.0/tasks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 arcee_py-1.1.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 arcee_py-1.1.0/.github/iced/test.yml
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 arcee_py-1.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 arcee_py-1.1.0/arcee/__init__.py
+-rw-r--r--   0        0        0    10164 2020-02-02 00:00:00.000000 arcee_py-1.1.0/arcee/api.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 arcee_py-1.1.0/arcee/api_handler.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 arcee_py-1.1.0/arcee/cli.py
+-rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 arcee_py-1.1.0/arcee/cli_handler.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 arcee_py-1.1.0/arcee/config.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 arcee_py-1.1.0/arcee/dalm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.1.0/arcee/schemas/__init__.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 arcee_py-1.1.0/arcee/schemas/doc.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 arcee_py-1.1.0/arcee/schemas/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcee_py-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 arcee_py-1.1.0/tests/test_api_handler.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 arcee_py-1.1.0/.gitignore
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 arcee_py-1.1.0/README.md
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 arcee_py-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 arcee_py-1.1.0/PKG-INFO
```

### Comparing `arcee_py-1.0.9/tasks.py` & `arcee_py-1.1.0/tasks.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.9/.github/iced/test.yml` & `arcee_py-1.1.0/.github/iced/test.yml`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.9/.github/workflows/publish.yml` & `arcee_py-1.1.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.9/arcee/__init__.py` & `arcee_py-1.1.0/arcee/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.9"
+__version__ = "1.1.0"
 
 import os
 
 from arcee import config
 from arcee.api import (
     upload_docs,
     upload_corpus_folder,
```

### Comparing `arcee_py-1.0.9/arcee/api.py` & `arcee_py-1.1.0/arcee/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -123,50 +123,56 @@
 
     data = {"pretraining_name": pretraining_name, "corpus_name": corpus, "base_model": base_model}
 
     return make_request("post", Route.pretraining + "/startTraining", data)
 
 def start_merging(
     merging_name: str,
-    arcee_aligned_models: Optional[List[str]],
-    arcee_merged_models: Optional[List[str]],
+    wandb_key: str = None,
+    arcee_aligned_models: Optional[List[str]] = None,
+    arcee_merged_models: Optional[List[str]] = None,
     arcee_pretrained_models: Optional[List[str]] = None,
     hf_models: Optional[List[str]] = None,
-    arcee_eval_qa_set_names: Optional[List[str]] = None,
-    general_evals: Optional[List[str]] = None,
+    arcee_eval_qa_set_names_and_weights: Optional[List[dict]] = None,
+    general_evals_and_weights: Optional[List[dict]] = None,
     base_model: Optional[str] = None,
     merge_method: Optional[str] = None,
+    instance_type str = None,
+    capacity_id: str = None,
     time_budget_secs: int = 1,
 ) -> None:
     """
     Start merging models
 
     Args:
         merging_name (str): The name of the merging job
         arcee_aligned_models (list): A list of ARCEE models to merge
         arcee_merged_models (list): A list of ARCEE models already merged
         arcee_pretrained_models (list): A list of pretrained ARCEE models
         hf_models (list): A list of Hugging Face models to merge
-        eval_qa_set_names (list): A list of QA set names to merge
-        general_evals (list): A list of general evaluations to merge
+        eval_qa_set_names_and_weights (list): A list of QA set names to merge
+        general_evals_and_weights (list): A list of general evaluations to merge
         base_model (str): The name of the base model to use
         merge_method (str): The merging method to use
         time_budget_secs (int): The time budget for the merging job (seconds)
     """
-
+    
     data = {
         "merging_name": merging_name,
+        "wandb_key": wandb_key,
         "arcee_aligned_models": arcee_aligned_models,
         "arcee_merged_models": arcee_merged_models,
         "arcee_pretrained_models": arcee_pretrained_models,
         "hf_models": hf_models,
-        "arcee_eval_qa_set_names": arcee_eval_qa_set_names,
-        "general_evals": general_evals,
+        "arcee_eval_qa_set_names_and_weights": arcee_eval_qa_set_names_and_weights,
+        "general_evals_and_weights": general_evals_and_weights,
         "base_model": base_model,
         "merge_method": merge_method,
+        "instance_type": instance_type,
+        "capacity_id": capacity_id,
         "time_budget_secs": time_budget_secs,
     }
 
     return make_request("post", Route.merging + "/startMerging", data)
 
 
 def delete_corpus(corpus: str) -> None:
```

### Comparing `arcee_py-1.0.9/arcee/api_handler.py` & `arcee_py-1.1.0/arcee/api_handler.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.9/arcee/cli.py` & `arcee_py-1.1.0/arcee/cli.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.9/arcee/cli_handler.py` & `arcee_py-1.1.0/arcee/cli_handler.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.9/arcee/config.py` & `arcee_py-1.1.0/arcee/config.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.9/arcee/dalm.py` & `arcee_py-1.1.0/arcee/dalm.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.9/tests/test_api_handler.py` & `arcee_py-1.1.0/tests/test_api_handler.py`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.9/.gitignore` & `arcee_py-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.9/README.md` & `arcee_py-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.9/pyproject.toml` & `arcee_py-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arcee_py-1.0.9/PKG-INFO` & `arcee_py-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcee-py
-Version: 1.0.9
+Version: 1.1.0
 Project-URL: Home, https://arcee.ai
 Author-email: Jacob Solowetz <jacob@arcee.ai>, Ben Epstein <ben@arcee.ai>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: pydantic<3.0,>=2.4.2
 Requires-Dist: requests
 Requires-Dist: rich
```

