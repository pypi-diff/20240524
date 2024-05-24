# Comparing `tmp/superb_ai_curate-1.2.2.tar.gz` & `tmp/superb_ai_curate-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superb_ai_curate-1.2.2.tar", max compression
+gzip compressed data, was "superb_ai_curate-1.3.0.tar", max compression
```

## Comparing `superb_ai_curate-1.2.2.tar` & `superb_ai_curate-1.3.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1083 2023-06-15 06:27:16.156321 superb_ai_curate-1.2.2/LICENSE
--rw-r--r--   0        0        0     3309 2023-09-19 05:20:56.054403 superb_ai_curate-1.2.2/README.md
--rw-r--r--   0        0        0     3244 2024-04-12 05:01:59.826062 superb_ai_curate-1.2.2/pyproject.toml
--rw-r--r--   0        0        0      430 2024-04-11 13:01:44.645615 superb_ai_curate-1.2.2/spb_curate/__init__.py
--rw-r--r--   0        0        0      172 2023-11-14 10:01:04.037123 superb_ai_curate-1.2.2/spb_curate/abstract/__init__.py
--rw-r--r--   0        0        0      164 2023-11-14 10:01:04.037271 superb_ai_curate-1.2.2/spb_curate/abstract/api/__init__.py
--rw-r--r--   0        0        0    10126 2023-09-19 05:20:56.055153 superb_ai_curate-1.2.2/spb_curate/abstract/api/resource.py
--rw-r--r--   0        0        0     8270 2023-09-19 05:20:56.055472 superb_ai_curate-1.2.2/spb_curate/abstract/superb_ai_object.py
--rw-r--r--   0        0        0     9349 2023-06-15 06:27:16.158041 superb_ai_curate-1.2.2/spb_curate/api_requestor.py
--rw-r--r--   0        0        0     1932 2023-06-15 06:27:16.158123 superb_ai_curate-1.2.2/spb_curate/config.py
--rw-r--r--   0        0        0      139 2023-11-14 10:01:04.037385 superb_ai_curate-1.2.2/spb_curate/curate/__init__.py
--rw-r--r--   0        0        0      125 2023-11-14 10:01:04.037496 superb_ai_curate-1.2.2/spb_curate/curate/api/__init__.py
--rw-r--r--   0        0        0      378 2023-11-14 10:01:04.037568 superb_ai_curate-1.2.2/spb_curate/curate/api/abstract.py
--rw-r--r--   0        0        0   108488 2024-04-12 05:01:59.826544 superb_ai_curate-1.2.2/spb_curate/curate/api/curate.py
--rw-r--r--   0        0        0      618 2023-11-14 10:01:04.038109 superb_ai_curate-1.2.2/spb_curate/curate/api/enums.py
--rw-r--r--   0        0        0    10696 2023-11-14 10:01:04.038389 superb_ai_curate-1.2.2/spb_curate/curate/api/job.py
--rw-r--r--   0        0        0    25391 2023-11-14 10:01:04.038566 superb_ai_curate-1.2.2/spb_curate/curate/api/model_diagnosis.py
--rw-r--r--   0        0        0       70 2023-11-14 10:01:04.038647 superb_ai_curate-1.2.2/spb_curate/curate/api/settings.py
--rw-r--r--   0        0        0      300 2023-06-15 06:27:16.158508 superb_ai_curate-1.2.2/spb_curate/curate/model/__init__.py
--rw-r--r--   0        0        0    24433 2023-06-15 06:27:16.158644 superb_ai_curate-1.2.2/spb_curate/curate/model/annotation_types.py
--rw-r--r--   0        0        0     2162 2023-06-15 06:27:16.158744 superb_ai_curate-1.2.2/spb_curate/error.py
--rw-r--r--   0        0        0     4820 2024-04-03 05:52:51.356901 superb_ai_curate-1.2.2/spb_curate/http_client.py
--rw-r--r--   0        0        0      287 2023-06-15 06:27:16.158905 superb_ai_curate-1.2.2/spb_curate/object_mapping.py
--rw-r--r--   0        0        0      730 2024-04-03 05:52:51.357334 superb_ai_curate-1.2.2/spb_curate/superb_ai_response.py
--rw-r--r--   0        0        0     5347 2023-06-15 06:27:16.159080 superb_ai_curate-1.2.2/spb_curate/util.py
--rw-r--r--   0        0        0      166 2023-06-15 06:27:16.159147 superb_ai_curate-1.2.2/spb_curate/version.py
--rw-r--r--   0        0        0     5180 1970-01-01 00:00:00.000000 superb_ai_curate-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-10-25 02:33:11.990425 superb_ai_curate-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3309 2023-10-25 02:33:11.990493 superb_ai_curate-1.3.0/README.md
+-rw-r--r--   0        0        0     3247 2024-05-24 07:37:12.559355 superb_ai_curate-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      430 2023-10-31 07:38:13.527407 superb_ai_curate-1.3.0/spb_curate/__init__.py
+-rw-r--r--   0        0        0      172 2023-10-31 07:38:13.527493 superb_ai_curate-1.3.0/spb_curate/abstract/__init__.py
+-rw-r--r--   0        0        0      164 2023-10-31 07:38:13.527572 superb_ai_curate-1.3.0/spb_curate/abstract/api/__init__.py
+-rw-r--r--   0        0        0    10126 2023-10-25 02:33:11.991765 superb_ai_curate-1.3.0/spb_curate/abstract/api/resource.py
+-rw-r--r--   0        0        0     8270 2023-10-25 02:33:11.991855 superb_ai_curate-1.3.0/spb_curate/abstract/superb_ai_object.py
+-rw-r--r--   0        0        0     9349 2024-03-15 02:23:20.097160 superb_ai_curate-1.3.0/spb_curate/api_requestor.py
+-rw-r--r--   0        0        0     1932 2023-10-25 02:33:11.992010 superb_ai_curate-1.3.0/spb_curate/config.py
+-rw-r--r--   0        0        0      139 2023-10-31 07:38:13.527835 superb_ai_curate-1.3.0/spb_curate/curate/__init__.py
+-rw-r--r--   0        0        0      125 2023-10-31 07:38:13.528111 superb_ai_curate-1.3.0/spb_curate/curate/api/__init__.py
+-rw-r--r--   0        0        0      378 2023-10-31 07:38:13.528165 superb_ai_curate-1.3.0/spb_curate/curate/api/abstract.py
+-rw-r--r--   0        0        0   108488 2024-05-24 06:32:44.279060 superb_ai_curate-1.3.0/spb_curate/curate/api/curate.py
+-rw-r--r--   0        0        0      818 2024-05-24 07:37:12.559707 superb_ai_curate-1.3.0/spb_curate/curate/api/enums.py
+-rw-r--r--   0        0        0    10696 2023-10-31 07:38:13.528988 superb_ai_curate-1.3.0/spb_curate/curate/api/job.py
+-rw-r--r--   0        0        0    26137 2024-05-24 07:37:12.560155 superb_ai_curate-1.3.0/spb_curate/curate/api/model_diagnosis.py
+-rw-r--r--   0        0        0       70 2023-10-31 07:38:13.529377 superb_ai_curate-1.3.0/spb_curate/curate/api/settings.py
+-rw-r--r--   0        0        0      300 2023-10-25 02:33:11.992298 superb_ai_curate-1.3.0/spb_curate/curate/model/__init__.py
+-rw-r--r--   0        0        0    24433 2023-10-25 02:33:11.992398 superb_ai_curate-1.3.0/spb_curate/curate/model/annotation_types.py
+-rw-r--r--   0        0        0     2162 2023-10-25 02:33:11.992458 superb_ai_curate-1.3.0/spb_curate/error.py
+-rw-r--r--   0        0        0     4820 2024-05-24 06:32:44.280099 superb_ai_curate-1.3.0/spb_curate/http_client.py
+-rw-r--r--   0        0        0      287 2023-10-25 02:33:11.992561 superb_ai_curate-1.3.0/spb_curate/object_mapping.py
+-rw-r--r--   0        0        0      730 2024-05-24 06:32:44.280434 superb_ai_curate-1.3.0/spb_curate/superb_ai_response.py
+-rw-r--r--   0        0        0     5347 2023-10-25 02:33:11.992686 superb_ai_curate-1.3.0/spb_curate/util.py
+-rw-r--r--   0        0        0      166 2023-10-25 02:33:11.992735 superb_ai_curate-1.3.0/spb_curate/version.py
+-rw-r--r--   0        0        0     4505 1970-01-01 00:00:00.000000 superb_ai_curate-1.3.0/setup.py
+-rw-r--r--   0        0        0     5374 1970-01-01 00:00:00.000000 superb_ai_curate-1.3.0/PKG-INFO
```

### Comparing `superb_ai_curate-1.2.2/LICENSE` & `superb_ai_curate-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.2/README.md` & `superb_ai_curate-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.2/pyproject.toml` & `superb_ai_curate-1.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # /pyproject.toml
 [project]
 description = "The official Superb AI Curate client for Python"
 name = "superb-ai-curate"
-version = "1.2.2"
+version = "1.3.0"
 
 [[project.authors]]
 name = "Superb AI"
 email = "support@superb-ai.com"
 
 [tool.poetry]
 name = "superb-ai-curate"
-version = "1.2.2"
+version = "1.3.0"
 license = "MIT"
 description = "The official Superb AI Curate client for Python"
 authors = ["Superb AI <support@superb-ai.com>"]
 homepage = "https://superb-ai.com/"
 repository = "https://github.com/Superb-AI-Suite/superb-ai-curate-python"
-documentation = "https://docs.superb-ai.com/reference/introduction-curate-sdk"
+documentation = "https://docs.superb-ai.com/reference/superb-curate-sdk-overview"
 readme = "README.md"
 packages = [{ include = "spb_curate" }]
 keywords = [
   "superb ai",
   "superbapi",
   "tasks",
   "categorization",
```

### Comparing `superb_ai_curate-1.2.2/spb_curate/abstract/api/resource.py` & `superb_ai_curate-1.3.0/spb_curate/abstract/api/resource.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.2/spb_curate/abstract/superb_ai_object.py` & `superb_ai_curate-1.3.0/spb_curate/abstract/superb_ai_object.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.2/spb_curate/api_requestor.py` & `superb_ai_curate-1.3.0/spb_curate/api_requestor.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.2/spb_curate/config.py` & `superb_ai_curate-1.3.0/spb_curate/config.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.2/spb_curate/curate/api/curate.py` & `superb_ai_curate-1.3.0/spb_curate/curate/api/curate.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.2/spb_curate/curate/api/enums.py` & `superb_ai_curate-1.3.0/spb_curate/curate/api/enums.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 from enum import Enum
 
 
+class IouType(str, Enum):
+    """
+    Types of IoU.
+    """
+
+    BOX = "bbox"
+    POLYGON = "segm"
+
+
 class JobType(Enum):
     """
     Available types of a job.
     """
 
     ANNOTATION_IMPORT = "ANNOTATION_IMPORT"
     DELETE_IMAGES = "DELETE_IMAGES"
@@ -13,14 +22,23 @@
     UPDATE_SLICE = "UPDATE_SLICE"
     UPDATE_SLICE_BY_QUERY = "UPDATE_SLICE_BY_QUERY"
 
     def __str__(self):
         return self.value
 
 
+class Split(str, Enum):
+    """
+    Types of Split.
+    """
+
+    TRAIN = "TRAIN"
+    VAL = "VAL"
+
+
 class SearchFieldMappingType(str, Enum):
     ANNOTATION_CLASS = "annotations.class_count"
     ANNOTATION_METADATA = "annotations.metadata"
     IMAGE_METADATA = "images.metadata"
 
     def __str__(self):
         return self.value
```

### Comparing `superb_ai_curate-1.2.2/spb_curate/curate/api/job.py` & `superb_ai_curate-1.3.0/spb_curate/curate/api/job.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.2/spb_curate/curate/api/model_diagnosis.py` & `superb_ai_curate-1.3.0/spb_curate/curate/api/model_diagnosis.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     CreateResource,
     ModifyResource,
     PaginateResource,
 )
 from spb_curate.abstract.superb_ai_object import SuperbAIObject
 from spb_curate.curate.api import settings
 from spb_curate.curate.api.curate import Job
-from spb_curate.curate.api.enums import JobType
+from spb_curate.curate.api.enums import IouType, JobType, Split
 from spb_curate.curate.model.annotation_types import (
     AnnotationType,
     BoundingBox,
     Category,
     Cuboid2D,
     Keypoints,
     Polygon,
@@ -39,29 +39,33 @@
         cls,
         *,
         access_key: Optional[str] = None,
         team_name: Optional[str] = None,
         dataset_id: str,
         model_name: str,
         class_list: List[str],
-        metadata: Optional[dict] = None,
+        iou_type: IouType,
+        metadata: Optional[Dict[str, Union[int, float, decimal.Decimal]]] = None,
     ) -> Diagnosis:
         """
         Creates a diagnosis.
 
         Parameters
         ----------
         dataset_id
             The ID of the dataset to use for the diagnosis.
         model_name
             The name of the model to diagnose.
         class_list
             The list of class names to diagnose.
+        iou_type
+            The IoU type of the diagnosis.
         metadata
             The metadata associated with the diagnosis.
+            Supported fields: ``beta``, ``target_iou``.
         access_key
             An access key for request authentication.
             If provided, overrides the configuration.
         team_name
             A team name for request authentication.
             If provided, overrides the configuration.
 
@@ -74,14 +78,15 @@
         ConflictError
             When a diagnosis related to the dataset and model already exists.
         """
         endpoint_params = {"dataset_id": dataset_id}
         param_metadata = {
             "beta": 1.0,
             "class_list": class_list,
+            "iou_type": iou_type,
             "target_iou": 0.5,
         }
 
         if metadata:
             param_metadata["beta"] = metadata.get("beta", 1.0)
             param_metadata["target_iou"] = metadata.get("target_iou", 0.5)
 
@@ -314,23 +319,26 @@
 
     def add_predictions(
         self,
         *,
         access_key: Optional[str] = None,
         team_name: Optional[str] = None,
         predictions: List[Prediction],
+        split: Split = Split.VAL,
         asynchronous: bool = True,
     ) -> Job:
         """
         Creates a job that adds newly initialized predictions to the diagnosis.
 
         Parameters
         ----------
         predictions
             Newly initialized predictions to add.
+        split
+            The subset data type used for training the model.
         asynchronous
             Whether to immediately return the job after creating it.
             If set to ``False``, the function waits for the job to finish before returning.
         access_key
             An access key for request authentication.
             If provided, overrides the configuration.
         team_name
@@ -343,14 +351,15 @@
         """
         return Prediction.create_bulk(
             access_key=access_key,
             team_name=team_name,
             dataset_id=self.dataset_id,
             diagnosis_id=self.id,
             predictions=predictions,
+            split=split,
             asynchronous=asynchronous,
         )
 
     def refresh(
         self,
         *,
         access_key: Optional[str] = None,
@@ -657,17 +666,19 @@
         """
 
         super(Prediction, self).__init__(
             confidence=confidence,
             image_id=image_id,
             prediction_class=prediction_class,
             prediction_value=prediction_value,
-            prediction_type=prediction_value._object_type
-            if isinstance(prediction_value, AnnotationType)
-            else prediction_type,
+            prediction_type=(
+                prediction_value._object_type
+                if isinstance(prediction_value, AnnotationType)
+                else prediction_type
+            ),
             **params,
         )
 
     def _init_volatile_fields(
         self,
         confidence: Union[int, float, decimal.Decimal],
         image_id: str,
@@ -746,27 +757,30 @@
         cls,
         *,
         access_key: Optional[str] = None,
         team_name: Optional[str] = None,
         dataset_id: str,
         diagnosis_id: str,
         predictions: List[Prediction],
+        split: Split = Split.VAL,
         asynchronous: bool = True,
     ) -> Job:
         """
         Creates a job that adds newly initialized predictions to a diagnosis.
 
         Parameters
         ----------
         dataset_id
             The ID of the dataset to add the predictions to.
         diagnosis_id
             The ID of the diagnosis to add the predictions to.
         predictions
             Newly initialized predictions to add.
+        split
+            The subset data type used for training the model.
         asynchronous
             Whether to immediately return the job after creating it.
             If set to ``False``, the function waits for the job to finish before returning.
         access_key
             An access key for request authentication.
             If provided, overrides the configuration.
         team_name
@@ -794,14 +808,15 @@
             access_key=access_key,
             team_name=team_name,
             job_type=JobType.IMPORT_PREDICTIONS,
             param={
                 "dataset_id": dataset_id,
                 "diagnosis_id": diagnosis_id,
                 "predictions": {"param_id": uploaded_param["id"]},
+                "split": split,
             },
         )
 
         if not asynchronous:
             job.wait_until_complete()
 
         return job
@@ -810,29 +825,33 @@
 def create_diagnosis(
     *,
     access_key: Optional[str] = None,
     team_name: Optional[str] = None,
     dataset_id: str,
     model_name: str,
     class_list: List[str],
-    metadata: Optional[dict] = None,
+    iou_type: IouType,
+    metadata: Optional[Dict[str, Union[int, float, decimal.Decimal]]] = None,
 ) -> Diagnosis:
     """
     Creates a diagnosis.
 
     Parameters
     ----------
     dataset_id
         The ID of the dataset to use for the diagnosis.
     model_name
         The name of the model to diagnose.
     class_list
         The list of class names to diagnose.
+    iou_type
+        The iou type of the diagnosis.
     metadata
         The metadata associated with the diagnosis.
+        Supported fields: ``beta``, ``target_iou``.
     access_key
         An access key for request authentication.
         If provided, overrides the configuration.
     team_name
         A team name for request authentication.
         If provided, overrides the configuration.
 
@@ -847,14 +866,15 @@
     """
     return Diagnosis.create(
         access_key=access_key,
         team_name=team_name,
         dataset_id=dataset_id,
         model_name=model_name,
         class_list=class_list,
+        iou_type=iou_type,
         metadata=metadata,
     )
 
 
 def fetch_available_models(
     *,
     access_key: Optional[str] = None,
```

### Comparing `superb_ai_curate-1.2.2/spb_curate/curate/model/annotation_types.py` & `superb_ai_curate-1.3.0/spb_curate/curate/model/annotation_types.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.2/spb_curate/error.py` & `superb_ai_curate-1.3.0/spb_curate/error.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.2/spb_curate/http_client.py` & `superb_ai_curate-1.3.0/spb_curate/http_client.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.2/spb_curate/superb_ai_response.py` & `superb_ai_curate-1.3.0/spb_curate/superb_ai_response.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.2/spb_curate/util.py` & `superb_ai_curate-1.3.0/spb_curate/util.py`

 * *Files identical despite different names*

### Comparing `superb_ai_curate-1.2.2/PKG-INFO` & `superb_ai_curate-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superb-ai-curate
-Version: 1.2.2
+Version: 1.3.0
 Summary: The official Superb AI Curate client for Python
 Home-page: https://superb-ai.com/
 License: MIT
 Keywords: superb ai,superbapi,tasks,categorization,annotation,labeling,dataops,mlops,curation
 Author: Superb AI
 Author-email: support@superb-ai.com
 Requires-Python: >=3.7,<4.0
@@ -16,31 +16,35 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: dev
 Provides-Extra: docs
-Requires-Dist: Sphinx ; extra == "docs"
-Requires-Dist: black ; extra == "dev"
-Requires-Dist: coveralls ; extra == "dev"
-Requires-Dist: isort ; extra == "dev"
-Requires-Dist: pytest ; extra == "dev"
-Requires-Dist: pytest-cov ; extra == "dev"
+Requires-Dist: Sphinx; extra == "docs"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: coveralls; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 Requires-Dist: requests (>=2.20.0,<3.0.0)
-Requires-Dist: sphinx-autodoc-typehints (>=1.19.4,<2.0.0) ; extra == "docs"
-Requires-Dist: sphinx-pyproject ; extra == "docs"
-Requires-Dist: sphinx-rtd-theme ; extra == "docs"
-Requires-Dist: sphinxcontrib-napoleon ; extra == "docs"
-Project-URL: Documentation, https://docs.superb-ai.com/reference/introduction-curate-sdk
+Requires-Dist: sphinx-autodoc-typehints (>=1.19.4,<2.0.0); extra == "docs"
+Requires-Dist: sphinx-pyproject; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: sphinxcontrib-napoleon; extra == "docs"
+Project-URL: Documentation, https://docs.superb-ai.com/reference/superb-curate-sdk-overview
 Project-URL: Repository, https://github.com/Superb-AI-Suite/superb-ai-curate-python
 Description-Content-Type: text/markdown
 
 # `superb-ai-curate`
 
 [![Coverage Status](https://coveralls.io/repos/github/Superb-AI-Suite/superb-ai-curate-python/badge.svg?branch=main)](https://coveralls.io/github/Superb-AI-Suite/superb-ai-curate-python?branch=main)
 [![Version](https://img.shields.io/pypi/v/superb-ai-curate)](https://pypi.org/project/superb-ai-curate/)
```

