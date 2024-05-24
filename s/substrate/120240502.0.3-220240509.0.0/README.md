# Comparing `tmp/substrate-120240502.0.3.tar.gz` & `tmp/substrate-220240509.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrate-120240502.0.3.tar", max compression
+gzip compressed data, was "substrate-220240509.0.0.tar", max compression
```

## Comparing `substrate-120240502.0.3.tar` & `substrate-220240509.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1066 2024-04-01 19:52:58.550017 substrate-120240502.0.3/LICENSE
--rw-r--r--   0        0        0     2715 2024-05-07 14:55:29.245125 substrate-120240502.0.3/README.md
--rw-r--r--   0        0        0     2079 2024-05-20 15:26:28.899939 substrate-120240502.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-17 17:39:17.445476 substrate-120240502.0.3/substrate/.keep
--rw-r--r--   0        0        0       17 2024-05-07 14:55:29.246970 substrate-120240502.0.3/substrate/GEN_VERSION
--rw-r--r--   0        0        0     2188 2024-05-07 14:55:29.247076 substrate-120240502.0.3/substrate/__init__.py
--rw-r--r--   0        0        0     5885 2024-05-20 15:23:21.502856 substrate-120240502.0.3/substrate/_client.py
--rw-r--r--   0        0        0       29 2024-05-20 15:26:28.900395 substrate-120240502.0.3/substrate/_version.py
--rw-r--r--   0        0        0        1 2024-04-01 19:52:58.552158 substrate-120240502.0.3/substrate/core/__init__.py
--rw-r--r--   0        0        0       27 2024-04-01 19:52:58.552245 substrate-120240502.0.3/substrate/core/_version.py
--rw-r--r--   0        0        0     1535 2024-04-17 17:39:17.446324 substrate-120240502.0.3/substrate/core/base_future.py
--rw-r--r--   0        0        0        0 2024-04-01 19:52:58.552427 substrate-120240502.0.3/substrate/core/client/__init__.py
--rw-r--r--   0        0        0     1750 2024-04-01 19:52:58.552528 substrate-120240502.0.3/substrate/core/client/find_futures_client.py
--rw-r--r--   0        0        0     2697 2024-04-17 17:39:17.446448 substrate-120240502.0.3/substrate/core/client/future.py
--rw-r--r--   0        0        0     1212 2024-04-01 19:52:58.552701 substrate-120240502.0.3/substrate/core/client/graph.py
--rw-r--r--   0        0        0     1149 2024-04-01 19:52:58.552792 substrate-120240502.0.3/substrate/core/coregraph.py
--rw-r--r--   0        0        0     2212 2024-05-07 14:55:29.247367 substrate-120240502.0.3/substrate/core/corenode.py
--rw-r--r--   0        0        0     1587 2024-05-07 14:55:29.247795 substrate-120240502.0.3/substrate/core/future_directive.py
--rw-r--r--   0        0        0     1095 2024-05-20 15:23:21.503310 substrate-120240502.0.3/substrate/core/id_generator.py
--rw-r--r--   0        0        0    37176 2024-05-07 14:55:29.248214 substrate-120240502.0.3/substrate/core/models.py
--rw-r--r--   0        0        0     3798 2024-05-07 14:55:29.248358 substrate-120240502.0.3/substrate/core/sb.py
--rw-r--r--   0        0        0    32553 2024-04-19 22:14:10.804912 substrate-120240502.0.3/substrate/dataclass_models.py
--rw-r--r--   0        0        0    47757 2024-05-07 14:55:29.248641 substrate-120240502.0.3/substrate/future_dataclass_models.py
--rw-r--r--   0        0        0    42949 2024-05-07 14:55:29.248958 substrate-120240502.0.3/substrate/nodes.py
--rw-r--r--   0        0        0        0 2024-04-01 19:52:58.553826 substrate-120240502.0.3/substrate/py.typed
--rw-r--r--   0        0        0     2196 2024-05-20 14:53:03.816270 substrate-120240502.0.3/substrate/substrate.py
--rw-r--r--   0        0        0     1015 2024-05-07 14:55:29.249194 substrate-120240502.0.3/substrate/substrate_response.py
--rw-r--r--   0        0        0    37584 2024-05-07 14:55:29.249408 substrate-120240502.0.3/substrate/typeddict_models.py
--rw-r--r--   0        0        0     3352 1970-01-01 00:00:00.000000 substrate-120240502.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-220240509.0.0/LICENSE
+-rw-r--r--   0        0        0     2715 2024-05-01 20:59:44.017862 substrate-220240509.0.0/README.md
+-rw-r--r--   0        0        0     2079 2024-05-24 10:50:42.952002 substrate-220240509.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 19:17:25.000000 substrate-220240509.0.0/substrate/.keep
+-rw-r--r--   0        0        0       17 2024-05-24 10:31:07.000000 substrate-220240509.0.0/substrate/GEN_VERSION
+-rw-r--r--   0        0        0     2189 2024-05-24 10:31:09.000000 substrate-220240509.0.0/substrate/__init__.py
+-rw-r--r--   0        0        0     5885 2024-05-23 08:32:49.033293 substrate-220240509.0.0/substrate/_client.py
+-rw-r--r--   0        0        0       30 2024-05-24 10:56:53.972716 substrate-220240509.0.0/substrate/_version.py
+-rw-r--r--   0        0        0        1 2024-05-24 10:50:43.510765 substrate-220240509.0.0/substrate/core/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-24 10:50:43.510522 substrate-220240509.0.0/substrate/core/_version.py
+-rw-r--r--   0        0        0     1535 2024-05-24 10:50:43.511260 substrate-220240509.0.0/substrate/core/base_future.py
+-rw-r--r--   0        0        0        0 2024-05-24 10:50:43.512621 substrate-220240509.0.0/substrate/core/client/__init__.py
+-rw-r--r--   0        0        0     1750 2024-05-24 10:50:43.512882 substrate-220240509.0.0/substrate/core/client/find_futures_client.py
+-rw-r--r--   0        0        0     2697 2024-05-24 10:50:43.513384 substrate-220240509.0.0/substrate/core/client/future.py
+-rw-r--r--   0        0        0     1212 2024-05-24 10:50:43.512440 substrate-220240509.0.0/substrate/core/client/graph.py
+-rw-r--r--   0        0        0     1149 2024-05-24 10:50:43.511082 substrate-220240509.0.0/substrate/core/coregraph.py
+-rw-r--r--   0        0        0     2212 2024-05-24 10:50:43.508719 substrate-220240509.0.0/substrate/core/corenode.py
+-rw-r--r--   0        0        0     1587 2024-05-24 10:50:43.511587 substrate-220240509.0.0/substrate/core/future_directive.py
+-rw-r--r--   0        0        0     1095 2024-05-24 10:50:43.508248 substrate-220240509.0.0/substrate/core/id_generator.py
+-rw-r--r--   0        0        0    37376 2024-05-24 10:50:43.509677 substrate-220240509.0.0/substrate/core/models.py
+-rw-r--r--   0        0        0     3798 2024-05-24 10:50:43.507773 substrate-220240509.0.0/substrate/core/sb.py
+-rw-r--r--   0        0        0    32553 2024-04-19 00:53:25.000000 substrate-220240509.0.0/substrate/dataclass_models.py
+-rw-r--r--   0        0        0    50559 2024-05-24 10:31:06.000000 substrate-220240509.0.0/substrate/future_dataclass_models.py
+-rw-r--r--   0        0        0    59454 2024-05-24 10:46:13.000000 substrate-220240509.0.0/substrate/nodes.py
+-rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-220240509.0.0/substrate/py.typed
+-rw-r--r--   0        0        0     2196 2024-05-06 18:16:14.492293 substrate-220240509.0.0/substrate/substrate.py
+-rw-r--r--   0        0        0     1015 2024-04-30 17:24:23.842724 substrate-220240509.0.0/substrate/substrate_response.py
+-rw-r--r--   0        0        0    37780 2024-05-24 10:31:03.000000 substrate-220240509.0.0/substrate/typeddict_models.py
+-rw-r--r--   0        0        0     3352 1970-01-01 00:00:00.000000 substrate-220240509.0.0/PKG-INFO
```

### Comparing `substrate-120240502.0.3/LICENSE` & `substrate-220240509.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.3/README.md` & `substrate-220240509.0.0/README.md`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.3/pyproject.toml` & `substrate-220240509.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "substrate"
-version = "120240502.0.3"
+version = "220240509.0.0"
 description = "Substrate Python SDK"
 readme = "README.md"
 authors = [ "vprtwn <ben@substrate.run>", "liamgriffiths <liam@substrate.run>",]
 [[tool.poetry.packages]]
 include = "substrate"
 
 [tool.pyright]
```

### Comparing `substrate-120240502.0.3/substrate/__init__.py` & `substrate-220240509.0.0/substrate/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
-꩜ Substrate Python SDK
+𐃏 Substrate Python SDK
 
-20240502.20240502
+20240509.20240524
 """
 
 from .nodes import (
     CLIP,
     XTTSV2,
     JinaV2,
     RunCode,
```

### Comparing `substrate-120240502.0.3/substrate/_client.py` & `substrate-220240509.0.0/substrate/_client.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.3/substrate/core/base_future.py` & `substrate-220240509.0.0/substrate/core/base_future.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.3/substrate/core/client/find_futures_client.py` & `substrate-220240509.0.0/substrate/core/client/find_futures_client.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.3/substrate/core/client/future.py` & `substrate-220240509.0.0/substrate/core/client/future.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.3/substrate/core/client/graph.py` & `substrate-220240509.0.0/substrate/core/client/graph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.3/substrate/core/coregraph.py` & `substrate-220240509.0.0/substrate/core/coregraph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.3/substrate/core/corenode.py` & `substrate-220240509.0.0/substrate/core/corenode.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.3/substrate/core/future_directive.py` & `substrate-220240509.0.0/substrate/core/future_directive.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.3/substrate/core/id_generator.py` & `substrate-220240509.0.0/substrate/core/id_generator.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.3/substrate/core/models.py` & `substrate-220240509.0.0/substrate/core/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-꩜ Substrate
+𐃏 Substrate
 @generated file
 (using datamodel-codegen)
 """
 
 
 from __future__ import annotations
 
@@ -109,18 +109,22 @@
     node: Literal["Mistral7BInstruct", "Mixtral8x7BInstruct"] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
 class GenerateJSONOut(BaseModel):
-    json_object: Dict[str, Any]
+    json_object: Optional[Dict[str, Any]] = None
     """
     JSON response.
     """
+    text: Optional[str] = None
+    """
+    If the model output could not be parsed to JSON, this is the raw text output.
+    """
 
 
 class MultiGenerateTextIn(BaseModel):
     prompt: str
     """
     Input prompt.
     """
@@ -564,15 +568,15 @@
 
 
 class StableDiffusionXLIPAdapterIn(BaseModel):
     prompt: str
     """
     Text prompt.
     """
-    image_prompt_uri: Optional[str] = None
+    image_prompt_uri: str
     """
     Image prompt.
     """
     num_images: Annotated[int, Field(ge=1, le=8)]
     """
     Number of images to generate.
     """
@@ -1124,15 +1128,15 @@
     """
     collection_name: Optional[str] = None
     """
     Vector store name.
     """
     metadata: Optional[Dict[str, Any]] = None
     """
-    Metadata that can be used to query the vector store. Ignored if `store` is unset.
+    Metadata that can be used to query the vector store. Ignored if `collection_name` is unset.
     """
     embedded_metadata_keys: Optional[List[str]] = None
     """
     Choose keys from `metadata` to embed with text.
     """
     doc_id: Optional[str] = None
     """
@@ -1154,19 +1158,19 @@
 class EmbedTextItem(BaseModel):
     text: str
     """
     Text to embed.
     """
     metadata: Optional[Dict[str, Any]] = None
     """
-    Metadata that can be used to query the vector store. Ignored if `store` is unset.
+    Metadata that can be used to query the vector store. Ignored if `collection_name` is unset.
     """
     doc_id: Optional[str] = None
     """
-    Vector store document ID. Ignored if `store` is unset.
+    Vector store document ID. Ignored if `collection_name` is unset.
     """
 
 
 class MultiEmbedTextIn(BaseModel):
     items: List[EmbedTextItem]
     """
     Items to embed.
@@ -1221,15 +1225,15 @@
     """
     collection_name: Optional[str] = None
     """
     Vector store name.
     """
     doc_id: Optional[str] = None
     """
-    Vector store document ID. Ignored if `store` is unset.
+    Vector store document ID. Ignored if `collection_name` is unset.
     """
     model: Literal["clip"] = "clip"
     """
     Selected embedding model.
     """
 
 
@@ -1243,34 +1247,34 @@
 class EmbedImageItem(BaseModel):
     image_uri: str
     """
     Image to embed.
     """
     doc_id: Optional[str] = None
     """
-    Vector store document ID. Ignored if `store` is unset.
+    Vector store document ID. Ignored if `collection_name` is unset.
     """
 
 
 class EmbedTextOrImageItem(BaseModel):
     image_uri: Optional[str] = None
     """
     Image to embed.
     """
     text: Optional[str] = None
     """
     Text to embed.
     """
     metadata: Optional[Dict[str, Any]] = None
     """
-    Metadata that can be used to query the vector store. Ignored if `store` is unset.
+    Metadata that can be used to query the vector store. Ignored if `collection_name` is unset.
     """
     doc_id: Optional[str] = None
     """
-    Vector store document ID. Ignored if `store` is unset.
+    Vector store document ID. Ignored if `collection_name` is unset.
     """
 
 
 class MultiEmbedImageIn(BaseModel):
     items: List[EmbedImageItem]
     """
     Items to embed.
```

### Comparing `substrate-120240502.0.3/substrate/core/sb.py` & `substrate-220240509.0.0/substrate/core/sb.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.3/substrate/dataclass_models.py` & `substrate-220240509.0.0/substrate/dataclass_models.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.3/substrate/future_dataclass_models.py` & `substrate-220240509.0.0/substrate/future_dataclass_models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-꩜ Substrate
+𐃏 Substrate
 @generated file
 (using datamodel-codegen)
 """
 
 
 from __future__ import annotations
 
@@ -11,15 +11,15 @@
 from dataclasses import dataclass
 from typing_extensions import Literal
 
 
 @dataclass
 class ErrorOut:
     """
-    (Future reference)
+    Future reference to ErrorOut
     """
 
     type: Literal["api_error", "invalid_request_error"]
     """
     (Future reference)
     The type of error returned.
     """
@@ -34,15 +34,15 @@
     A unique identifier for the request.
     """
 
 
 @dataclass
 class FutureRunCodeIn:
     """
-    (Future reference)
+    Future reference to FutureRunCodeIn
     """
 
     code: str
     """
     (Future reference)
     Code to execute.
     """
@@ -57,15 +57,15 @@
     Interpreter to use.
     """
 
 
 @dataclass
 class FutureRunCodeOut:
     """
-    (Future reference)
+    Future reference to FutureRunCodeOut
     """
 
     json_output: Dict[str, Any]
     """
     (Future reference)
     `output` as parsed JSON. Print serialized json to `stdout` to receive JSON.
     """
@@ -80,15 +80,15 @@
     Contents of `stderr` after executing the code.
     """
 
 
 @dataclass
 class FutureGenerateTextIn:
     """
-    (Future reference)
+    Future reference to FutureGenerateTextIn
     """
 
     prompt: str
     """
     (Future reference)
     Input prompt.
     """
@@ -113,28 +113,28 @@
     Selected node.
     """
 
 
 @dataclass
 class FutureGenerateTextOut:
     """
-    (Future reference)
+    Future reference to FutureGenerateTextOut
     """
 
     text: str
     """
     (Future reference)
     Text response.
     """
 
 
 @dataclass
 class FutureGenerateJSONIn:
     """
-    (Future reference)
+    Future reference to FutureGenerateJSONIn
     """
 
     prompt: str
     """
     (Future reference)
     Input prompt.
     """
@@ -159,28 +159,33 @@
     Selected node.
     """
 
 
 @dataclass
 class FutureGenerateJSONOut:
     """
-    (Future reference)
+    Future reference to FutureGenerateJSONOut
     """
 
-    json_object: Dict[str, Any]
+    json_object: Optional[Dict[str, Any]] = None
     """
     (Future reference)
     JSON response.
     """
+    text: Optional[str] = None
+    """
+    (Future reference)
+    If the model output could not be parsed to JSON, this is the raw text output.
+    """
 
 
 @dataclass
 class FutureMultiGenerateTextIn:
     """
-    (Future reference)
+    Future reference to FutureMultiGenerateTextIn
     """
 
     prompt: str
     """
     (Future reference)
     Input prompt.
     """
@@ -210,28 +215,28 @@
     Selected node.
     """
 
 
 @dataclass
 class FutureMultiGenerateTextOut:
     """
-    (Future reference)
+    Future reference to FutureMultiGenerateTextOut
     """
 
     choices: List[FutureGenerateTextOut]
     """
     (Future reference)
     Response choices.
     """
 
 
 @dataclass
 class FutureBatchGenerateTextIn:
     """
-    (Future reference)
+    Future reference to FutureBatchGenerateTextIn
     """
 
     prompts: List[str]
     """
     (Future reference)
     Batch input prompts.
     """
@@ -246,28 +251,28 @@
     Maximum number of tokens to generate.
     """
 
 
 @dataclass
 class FutureBatchGenerateTextOut:
     """
-    (Future reference)
+    Future reference to FutureBatchGenerateTextOut
     """
 
     outputs: List[FutureGenerateTextOut]
     """
     (Future reference)
     Batch outputs.
     """
 
 
 @dataclass
 class FutureMultiGenerateJSONIn:
     """
-    (Future reference)
+    Future reference to FutureMultiGenerateJSONIn
     """
 
     prompt: str
     """
     (Future reference)
     Input prompt.
     """
@@ -297,28 +302,28 @@
     Selected node.
     """
 
 
 @dataclass
 class FutureMultiGenerateJSONOut:
     """
-    (Future reference)
+    Future reference to FutureMultiGenerateJSONOut
     """
 
     choices: List[FutureGenerateJSONOut]
     """
     (Future reference)
     Response choices.
     """
 
 
 @dataclass
 class FutureBatchGenerateJSONIn:
     """
-    (Future reference)
+    Future reference to FutureBatchGenerateJSONIn
     """
 
     prompts: List[str]
     """
     (Future reference)
     Batch input prompts.
     """
@@ -338,28 +343,28 @@
     Maximum number of tokens to generate.
     """
 
 
 @dataclass
 class FutureBatchGenerateJSONOut:
     """
-    (Future reference)
+    Future reference to FutureBatchGenerateJSONOut
     """
 
     outputs: List[FutureGenerateJSONOut]
     """
     (Future reference)
     Batch outputs.
     """
 
 
 @dataclass
 class FutureMistral7BInstructIn:
     """
-    (Future reference)
+    Future reference to FutureMistral7BInstructIn
     """
 
     prompt: str
     """
     (Future reference)
     Input prompt.
     """
@@ -384,15 +389,15 @@
     Maximum number of tokens to generate.
     """
 
 
 @dataclass
 class Mistral7BInstructChoice:
     """
-    (Future reference)
+    Future reference to Mistral7BInstructChoice
     """
 
     text: Optional[str] = None
     """
     (Future reference)
     Text response, if `json_schema` was not provided.
     """
@@ -402,28 +407,28 @@
     JSON response, if `json_schema` was provided.
     """
 
 
 @dataclass
 class FutureMistral7BInstructOut:
     """
-    (Future reference)
+    Future reference to FutureMistral7BInstructOut
     """
 
     choices: List[Mistral7BInstructChoice]
     """
     (Future reference)
     Response choices.
     """
 
 
 @dataclass
 class FutureMixtral8x7BInstructIn:
     """
-    (Future reference)
+    Future reference to FutureMixtral8x7BInstructIn
     """
 
     prompt: str
     """
     (Future reference)
     Input prompt.
     """
@@ -448,15 +453,15 @@
     Maximum number of tokens to generate.
     """
 
 
 @dataclass
 class Mixtral8x7BChoice:
     """
-    (Future reference)
+    Future reference to Mixtral8x7BChoice
     """
 
     text: Optional[str] = None
     """
     (Future reference)
     Text response, if `json_schema` was not provided.
     """
@@ -466,28 +471,28 @@
     JSON response, if `json_schema` was provided.
     """
 
 
 @dataclass
 class FutureMixtral8x7BInstructOut:
     """
-    (Future reference)
+    Future reference to FutureMixtral8x7BInstructOut
     """
 
     choices: List[Mixtral8x7BChoice]
     """
     (Future reference)
     Response choices.
     """
 
 
 @dataclass
 class FutureLlama3Instruct8BIn:
     """
-    (Future reference)
+    Future reference to FutureLlama3Instruct8BIn
     """
 
     prompt: str
     """
     (Future reference)
     Input prompt.
     """
@@ -507,41 +512,41 @@
     Maximum number of tokens to generate.
     """
 
 
 @dataclass
 class Llama3Instruct8BChoice:
     """
-    (Future reference)
+    Future reference to Llama3Instruct8BChoice
     """
 
     text: Optional[str] = None
     """
     (Future reference)
     Text response.
     """
 
 
 @dataclass
 class FutureLlama3Instruct8BOut:
     """
-    (Future reference)
+    Future reference to FutureLlama3Instruct8BOut
     """
 
     choices: List[Llama3Instruct8BChoice]
     """
     (Future reference)
     Response choices.
     """
 
 
 @dataclass
 class FutureLlama3Instruct70BIn:
     """
-    (Future reference)
+    Future reference to FutureLlama3Instruct70BIn
     """
 
     prompt: str
     """
     (Future reference)
     Input prompt.
     """
@@ -561,41 +566,41 @@
     Maximum number of tokens to generate.
     """
 
 
 @dataclass
 class Llama3Instruct70BChoice:
     """
-    (Future reference)
+    Future reference to Llama3Instruct70BChoice
     """
 
     text: Optional[str] = None
     """
     (Future reference)
     Text response.
     """
 
 
 @dataclass
 class FutureLlama3Instruct70BOut:
     """
-    (Future reference)
+    Future reference to FutureLlama3Instruct70BOut
     """
 
     choices: List[Llama3Instruct70BChoice]
     """
     (Future reference)
     Response choices.
     """
 
 
 @dataclass
 class FutureGenerateTextVisionIn:
     """
-    (Future reference)
+    Future reference to FutureGenerateTextVisionIn
     """
 
     prompt: str
     """
     (Future reference)
     Text prompt.
     """
@@ -610,28 +615,28 @@
     Maximum number of tokens to generate.
     """
 
 
 @dataclass
 class FutureGenerateTextVisionOut:
     """
-    (Future reference)
+    Future reference to FutureGenerateTextVisionOut
     """
 
     text: str
     """
     (Future reference)
     Text response.
     """
 
 
 @dataclass
 class FutureFirellava13BIn:
     """
-    (Future reference)
+    Future reference to FutureFirellava13BIn
     """
 
     prompt: str
     """
     (Future reference)
     Text prompt.
     """
@@ -646,28 +651,28 @@
     Maximum number of tokens to generate.
     """
 
 
 @dataclass
 class FutureFirellava13BOut:
     """
-    (Future reference)
+    Future reference to FutureFirellava13BOut
     """
 
     text: str
     """
     (Future reference)
     Text response.
     """
 
 
 @dataclass
 class FutureGenerateImageIn:
     """
-    (Future reference)
+    Future reference to FutureGenerateImageIn
     """
 
     prompt: str
     """
     (Future reference)
     Text prompt.
     """
@@ -677,28 +682,28 @@
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
 class FutureGenerateImageOut:
     """
-    (Future reference)
+    Future reference to FutureGenerateImageOut
     """
 
     image_uri: str
     """
     (Future reference)
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 @dataclass
 class FutureMultiGenerateImageIn:
     """
-    (Future reference)
+    Future reference to FutureMultiGenerateImageIn
     """
 
     prompt: str
     """
     (Future reference)
     Text prompt.
     """
@@ -713,28 +718,28 @@
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
 class FutureMultiGenerateImageOut:
     """
-    (Future reference)
+    Future reference to FutureMultiGenerateImageOut
     """
 
     outputs: List[FutureGenerateImageOut]
     """
     (Future reference)
     Generated images.
     """
 
 
 @dataclass
 class FutureStableDiffusionXLIn:
     """
-    (Future reference)
+    Future reference to FutureStableDiffusionXLIn
     """
 
     prompt: str
     """
     (Future reference)
     Text prompt.
     """
@@ -779,15 +784,15 @@
     Higher values adhere to the text prompt more strongly, typically at the expense of image quality.
     """
 
 
 @dataclass
 class StableDiffusionImage:
     """
-    (Future reference)
+    Future reference to StableDiffusionImage
     """
 
     image_uri: str
     """
     (Future reference)
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
@@ -797,28 +802,28 @@
     The random noise seed used for generation.
     """
 
 
 @dataclass
 class FutureStableDiffusionXLOut:
     """
-    (Future reference)
+    Future reference to FutureStableDiffusionXLOut
     """
 
     outputs: List[StableDiffusionImage]
     """
     (Future reference)
     Generated images.
     """
 
 
 @dataclass
 class FutureStableDiffusionXLLightningIn:
     """
-    (Future reference)
+    Future reference to FutureStableDiffusionXLLightningIn
     """
 
     prompt: str
     """
     (Future reference)
     Text prompt.
     """
@@ -853,44 +858,44 @@
     Seeds for deterministic generation. Default is a random seed.
     """
 
 
 @dataclass
 class FutureStableDiffusionXLLightningOut:
     """
-    (Future reference)
+    Future reference to FutureStableDiffusionXLLightningOut
     """
 
     outputs: List[StableDiffusionImage]
     """
     (Future reference)
     Generated images.
     """
 
 
 @dataclass
 class FutureStableDiffusionXLIPAdapterIn:
     """
-    (Future reference)
+    Future reference to FutureStableDiffusionXLIPAdapterIn
     """
 
     prompt: str
     """
     (Future reference)
     Text prompt.
     """
-    num_images: int
+    image_prompt_uri: str
     """
     (Future reference)
-    Number of images to generate.
+    Image prompt.
     """
-    image_prompt_uri: Optional[str] = None
+    num_images: int
     """
     (Future reference)
-    Image prompt.
+    Number of images to generate.
     """
     ip_adapter_scale: float = 0.5
     """
     (Future reference)
     Controls the influence of the image prompt on the generated output.
     """
     negative_prompt: Optional[str] = None
@@ -919,28 +924,28 @@
     Random noise seeds. Default is random seeds for each generation.
     """
 
 
 @dataclass
 class FutureStableDiffusionXLIPAdapterOut:
     """
-    (Future reference)
+    Future reference to FutureStableDiffusionXLIPAdapterOut
     """
 
     outputs: List[StableDiffusionImage]
     """
     (Future reference)
     Generated images.
     """
 
 
 @dataclass
 class FutureStableDiffusionXLControlNetIn:
     """
-    (Future reference)
+    Future reference to FutureStableDiffusionXLControlNetIn
     """
 
     image_uri: str
     """
     (Future reference)
     Input image.
     """
@@ -985,28 +990,28 @@
     Random noise seeds. Default is random seeds for each generation.
     """
 
 
 @dataclass
 class FutureStableDiffusionXLControlNetOut:
     """
-    (Future reference)
+    Future reference to FutureStableDiffusionXLControlNetOut
     """
 
     outputs: List[StableDiffusionImage]
     """
     (Future reference)
     Generated images.
     """
 
 
 @dataclass
 class FutureGenerativeEditImageIn:
     """
-    (Future reference)
+    Future reference to FutureGenerativeEditImageIn
     """
 
     image_uri: str
     """
     (Future reference)
     Original image.
     """
@@ -1026,28 +1031,28 @@
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
 class FutureGenerativeEditImageOut:
     """
-    (Future reference)
+    Future reference to FutureGenerativeEditImageOut
     """
 
     image_uri: str
     """
     (Future reference)
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 @dataclass
 class FutureMultiGenerativeEditImageIn:
     """
-    (Future reference)
+    Future reference to FutureMultiGenerativeEditImageIn
     """
 
     image_uri: str
     """
     (Future reference)
     Original image.
     """
@@ -1072,28 +1077,28 @@
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
 class FutureMultiGenerativeEditImageOut:
     """
-    (Future reference)
+    Future reference to FutureMultiGenerativeEditImageOut
     """
 
     outputs: List[FutureGenerativeEditImageOut]
     """
     (Future reference)
     Generated images.
     """
 
 
 @dataclass
 class FutureStableDiffusionXLInpaintIn:
     """
-    (Future reference)
+    Future reference to FutureStableDiffusionXLInpaintIn
     """
 
     image_uri: str
     """
     (Future reference)
     Original image.
     """
@@ -1138,28 +1143,28 @@
     Random noise seeds. Default is random seeds for each generation.
     """
 
 
 @dataclass
 class FutureStableDiffusionXLInpaintOut:
     """
-    (Future reference)
+    Future reference to FutureStableDiffusionXLInpaintOut
     """
 
     outputs: List[StableDiffusionImage]
     """
     (Future reference)
     Generated images.
     """
 
 
 @dataclass
 class BoundingBox:
     """
-    (Future reference)
+    Future reference to BoundingBox
     """
 
     x1: float
     """
     (Future reference)
     Top left corner x.
     """
@@ -1179,15 +1184,15 @@
     Bottom right corner y.
     """
 
 
 @dataclass
 class Point:
     """
-    (Future reference)
+    Future reference to Point
     """
 
     x: int
     """
     (Future reference)
     X position.
     """
@@ -1197,15 +1202,15 @@
     Y position.
     """
 
 
 @dataclass
 class FutureFillMaskIn:
     """
-    (Future reference)
+    Future reference to FutureFillMaskIn
     """
 
     image_uri: str
     """
     (Future reference)
     Input image.
     """
@@ -1220,28 +1225,28 @@
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
 class FutureFillMaskOut:
     """
-    (Future reference)
+    Future reference to FutureFillMaskOut
     """
 
     image_uri: str
     """
     (Future reference)
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 @dataclass
 class FutureBigLaMaIn:
     """
-    (Future reference)
+    Future reference to FutureBigLaMaIn
     """
 
     image_uri: str
     """
     (Future reference)
     Input image.
     """
@@ -1256,28 +1261,28 @@
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
 class FutureBigLaMaOut:
     """
-    (Future reference)
+    Future reference to FutureBigLaMaOut
     """
 
     image_uri: str
     """
     (Future reference)
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 @dataclass
 class FutureRemoveBackgroundIn:
     """
-    (Future reference)
+    Future reference to FutureRemoveBackgroundIn
     """
 
     image_uri: str
     """
     (Future reference)
     Input image.
     """
@@ -1297,28 +1302,28 @@
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
 class FutureRemoveBackgroundOut:
     """
-    (Future reference)
+    Future reference to FutureRemoveBackgroundOut
     """
 
     image_uri: str
     """
     (Future reference)
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 @dataclass
 class FutureDISISNetIn:
     """
-    (Future reference)
+    Future reference to FutureDISISNetIn
     """
 
     image_uri: str
     """
     (Future reference)
     Input image.
     """
@@ -1328,28 +1333,28 @@
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
 class FutureDISISNetOut:
     """
-    (Future reference)
+    Future reference to FutureDISISNetOut
     """
 
     image_uri: str
     """
     (Future reference)
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 @dataclass
 class FutureUpscaleImageIn:
     """
-    (Future reference)
+    Future reference to FutureUpscaleImageIn
     """
 
     image_uri: str
     """
     (Future reference)
     Input image.
     """
@@ -1359,28 +1364,28 @@
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
 class FutureUpscaleImageOut:
     """
-    (Future reference)
+    Future reference to FutureUpscaleImageOut
     """
 
     image_uri: str
     """
     (Future reference)
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 @dataclass
 class FutureRealESRGANIn:
     """
-    (Future reference)
+    Future reference to FutureRealESRGANIn
     """
 
     image_uri: str
     """
     (Future reference)
     Input image.
     """
@@ -1390,28 +1395,28 @@
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
 class FutureRealESRGANOut:
     """
-    (Future reference)
+    Future reference to FutureRealESRGANOut
     """
 
     image_uri: str
     """
     (Future reference)
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 @dataclass
 class FutureSegmentUnderPointIn:
     """
-    (Future reference)
+    Future reference to FutureSegmentUnderPointIn
     """
 
     image_uri: str
     """
     (Future reference)
     Input image.
     """
@@ -1426,28 +1431,28 @@
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
 class FutureSegmentUnderPointOut:
     """
-    (Future reference)
+    Future reference to FutureSegmentUnderPointOut
     """
 
     mask_image_uri: str
     """
     (Future reference)
     Detected segments in 'mask image' format. Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 @dataclass
 class FutureSegmentAnythingIn:
     """
-    (Future reference)
+    Future reference to FutureSegmentAnythingIn
     """
 
     image_uri: str
     """
     (Future reference)
     Input image.
     """
@@ -1467,28 +1472,28 @@
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
 class FutureSegmentAnythingOut:
     """
-    (Future reference)
+    Future reference to FutureSegmentAnythingOut
     """
 
     mask_image_uri: str
     """
     (Future reference)
     Detected segments in 'mask image' format. Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 @dataclass
 class FutureTranscribeMediaIn:
     """
-    (Future reference)
+    Future reference to FutureTranscribeMediaIn
     """
 
     audio_uri: str
     """
     (Future reference)
     Input audio.
     """
@@ -1523,15 +1528,15 @@
     Suggest automatic chapter markers.
     """
 
 
 @dataclass
 class TranscribedWord:
     """
-    (Future reference)
+    Future reference to TranscribedWord
     """
 
     word: str
     """
     (Future reference)
     Text of word.
     """
@@ -1551,15 +1556,15 @@
     ID of speaker, if `diarize` is enabled.
     """
 
 
 @dataclass
 class TranscribedSegment:
     """
-    (Future reference)
+    Future reference to TranscribedSegment
     """
 
     text: str
     """
     (Future reference)
     Text of segment.
     """
@@ -1584,15 +1589,15 @@
     Aligned words, if `align` is enabled.
     """
 
 
 @dataclass
 class ChapterMarker:
     """
-    (Future reference)
+    Future reference to ChapterMarker
     """
 
     title: str
     """
     (Future reference)
     Chapter title.
     """
@@ -1602,15 +1607,15 @@
     Start time of chapter, in seconds.
     """
 
 
 @dataclass
 class FutureTranscribeMediaOut:
     """
-    (Future reference)
+    Future reference to FutureTranscribeMediaOut
     """
 
     text: str
     """
     (Future reference)
     Transcribed text.
     """
@@ -1625,15 +1630,15 @@
     Chapter markers, if `suggest_chapters` is enabled.
     """
 
 
 @dataclass
 class FutureGenerateSpeechIn:
     """
-    (Future reference)
+    Future reference to FutureGenerateSpeechIn
     """
 
     text: str
     """
     (Future reference)
     Input text.
     """
@@ -1643,28 +1648,28 @@
     Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the audio data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
 class FutureGenerateSpeechOut:
     """
-    (Future reference)
+    Future reference to FutureGenerateSpeechOut
     """
 
     audio_uri: str
     """
     (Future reference)
     Base 64-encoded WAV audio bytes, or a hosted audio url if `store` is provided.
     """
 
 
 @dataclass
 class FutureXTTSV2In:
     """
-    (Future reference)
+    Future reference to FutureXTTSV2In
     """
 
     text: str
     """
     (Future reference)
     Input text.
     """
@@ -1684,28 +1689,28 @@
     Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the audio data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
 class FutureXTTSV2Out:
     """
-    (Future reference)
+    Future reference to FutureXTTSV2Out
     """
 
     audio_uri: str
     """
     (Future reference)
     Base 64-encoded WAV audio bytes, or a hosted audio url if `store` is provided.
     """
 
 
 @dataclass
 class Embedding:
     """
-    (Future reference)
+    Future reference to Embedding
     """
 
     vector: List[float]
     """
     (Future reference)
     Embedding vector.
     """
@@ -1720,15 +1725,15 @@
     Vector store document metadata.
     """
 
 
 @dataclass
 class FutureEmbedTextIn:
     """
-    (Future reference)
+    Future reference to FutureEmbedTextIn
     """
 
     text: str
     """
     (Future reference)
     Text to embed.
     """
@@ -1736,15 +1741,15 @@
     """
     (Future reference)
     Vector store name.
     """
     metadata: Optional[Dict[str, Any]] = None
     """
     (Future reference)
-    Metadata that can be used to query the vector store. Ignored if `store` is unset.
+    Metadata that can be used to query the vector store. Ignored if `collection_name` is unset.
     """
     embedded_metadata_keys: Optional[List[str]] = None
     """
     (Future reference)
     Choose keys from `metadata` to embed with text.
     """
     doc_id: Optional[str] = None
@@ -1758,51 +1763,51 @@
     Selected embedding model.
     """
 
 
 @dataclass
 class FutureEmbedTextOut:
     """
-    (Future reference)
+    Future reference to FutureEmbedTextOut
     """
 
     embedding: Embedding
     """
     (Future reference)
     Generated embedding.
     """
 
 
 @dataclass
 class EmbedTextItem:
     """
-    (Future reference)
+    Future reference to EmbedTextItem
     """
 
     text: str
     """
     (Future reference)
     Text to embed.
     """
     metadata: Optional[Dict[str, Any]] = None
     """
     (Future reference)
-    Metadata that can be used to query the vector store. Ignored if `store` is unset.
+    Metadata that can be used to query the vector store. Ignored if `collection_name` is unset.
     """
     doc_id: Optional[str] = None
     """
     (Future reference)
-    Vector store document ID. Ignored if `store` is unset.
+    Vector store document ID. Ignored if `collection_name` is unset.
     """
 
 
 @dataclass
 class FutureMultiEmbedTextIn:
     """
-    (Future reference)
+    Future reference to FutureMultiEmbedTextIn
     """
 
     items: List[EmbedTextItem]
     """
     (Future reference)
     Items to embed.
     """
@@ -1822,28 +1827,28 @@
     Selected embedding model.
     """
 
 
 @dataclass
 class FutureMultiEmbedTextOut:
     """
-    (Future reference)
+    Future reference to FutureMultiEmbedTextOut
     """
 
     embeddings: List[Embedding]
     """
     (Future reference)
     Generated embeddings.
     """
 
 
 @dataclass
 class FutureJinaV2In:
     """
-    (Future reference)
+    Future reference to FutureJinaV2In
     """
 
     items: List[EmbedTextItem]
     """
     (Future reference)
     Items to embed.
     """
@@ -1858,28 +1863,28 @@
     Choose keys from `metadata` to embed with text.
     """
 
 
 @dataclass
 class FutureJinaV2Out:
     """
-    (Future reference)
+    Future reference to FutureJinaV2Out
     """
 
     embeddings: List[Embedding]
     """
     (Future reference)
     Generated embeddings.
     """
 
 
 @dataclass
 class FutureEmbedImageIn:
     """
-    (Future reference)
+    Future reference to FutureEmbedImageIn
     """
 
     image_uri: str
     """
     (Future reference)
     Image to embed.
     """
@@ -1887,58 +1892,58 @@
     """
     (Future reference)
     Vector store name.
     """
     doc_id: Optional[str] = None
     """
     (Future reference)
-    Vector store document ID. Ignored if `store` is unset.
+    Vector store document ID. Ignored if `collection_name` is unset.
     """
     model: Literal["clip"] = "clip"
     """
     (Future reference)
     Selected embedding model.
     """
 
 
 @dataclass
 class FutureEmbedImageOut:
     """
-    (Future reference)
+    Future reference to FutureEmbedImageOut
     """
 
     embedding: Embedding
     """
     (Future reference)
     Generated embedding.
     """
 
 
 @dataclass
 class EmbedImageItem:
     """
-    (Future reference)
+    Future reference to EmbedImageItem
     """
 
     image_uri: str
     """
     (Future reference)
     Image to embed.
     """
     doc_id: Optional[str] = None
     """
     (Future reference)
-    Vector store document ID. Ignored if `store` is unset.
+    Vector store document ID. Ignored if `collection_name` is unset.
     """
 
 
 @dataclass
 class EmbedTextOrImageItem:
     """
-    (Future reference)
+    Future reference to EmbedTextOrImageItem
     """
 
     image_uri: Optional[str] = None
     """
     (Future reference)
     Image to embed.
     """
@@ -1946,27 +1951,27 @@
     """
     (Future reference)
     Text to embed.
     """
     metadata: Optional[Dict[str, Any]] = None
     """
     (Future reference)
-    Metadata that can be used to query the vector store. Ignored if `store` is unset.
+    Metadata that can be used to query the vector store. Ignored if `collection_name` is unset.
     """
     doc_id: Optional[str] = None
     """
     (Future reference)
-    Vector store document ID. Ignored if `store` is unset.
+    Vector store document ID. Ignored if `collection_name` is unset.
     """
 
 
 @dataclass
 class FutureMultiEmbedImageIn:
     """
-    (Future reference)
+    Future reference to FutureMultiEmbedImageIn
     """
 
     items: List[EmbedImageItem]
     """
     (Future reference)
     Items to embed.
     """
@@ -1981,28 +1986,28 @@
     Selected embedding model.
     """
 
 
 @dataclass
 class FutureMultiEmbedImageOut:
     """
-    (Future reference)
+    Future reference to FutureMultiEmbedImageOut
     """
 
     embeddings: List[Embedding]
     """
     (Future reference)
     Generated embeddings.
     """
 
 
 @dataclass
 class FutureCLIPIn:
     """
-    (Future reference)
+    Future reference to FutureCLIPIn
     """
 
     items: List[EmbedTextOrImageItem]
     """
     (Future reference)
     Items to embed.
     """
@@ -2017,28 +2022,28 @@
     Choose keys from `metadata` to embed with text. Only applies to text items.
     """
 
 
 @dataclass
 class FutureCLIPOut:
     """
-    (Future reference)
+    Future reference to FutureCLIPOut
     """
 
     embeddings: List[Embedding]
     """
     (Future reference)
     Generated embeddings.
     """
 
 
 @dataclass
 class FutureCreateVectorStoreIn:
     """
-    (Future reference)
+    Future reference to FutureCreateVectorStoreIn
     """
 
     collection_name: str
     """
     (Future reference)
     Vector store name.
     """
@@ -2063,15 +2068,15 @@
     The distance metric to construct the index with.
     """
 
 
 @dataclass
 class FutureCreateVectorStoreOut:
     """
-    (Future reference)
+    Future reference to FutureCreateVectorStoreOut
     """
 
     collection_name: str
     """
     (Future reference)
     Vector store name.
     """
@@ -2096,37 +2101,37 @@
     The distance metric to construct the index with.
     """
 
 
 @dataclass
 class FutureListVectorStoresIn:
     """
-    (Future reference)
+    Future reference to FutureListVectorStoresIn
     """
 
     pass
 
 
 @dataclass
 class FutureListVectorStoresOut:
     """
-    (Future reference)
+    Future reference to FutureListVectorStoresOut
     """
 
     items: Optional[List[FutureCreateVectorStoreOut]] = None
     """
     (Future reference)
     List of vector stores.
     """
 
 
 @dataclass
 class FutureDeleteVectorStoreIn:
     """
-    (Future reference)
+    Future reference to FutureDeleteVectorStoreIn
     """
 
     collection_name: str
     """
     (Future reference)
     Vector store name.
     """
@@ -2136,15 +2141,15 @@
     Selected embedding model.
     """
 
 
 @dataclass
 class FutureDeleteVectorStoreOut:
     """
-    (Future reference)
+    Future reference to FutureDeleteVectorStoreOut
     """
 
     collection_name: str
     """
     (Future reference)
     Vector store name.
     """
@@ -2154,16 +2159,15 @@
     Selected embedding model.
     """
 
 
 @dataclass
 class Vector:
     """
-    (Future reference)
-    Canonical representation of document with embedding vector.
+    Future reference to Vector
     """
 
     id: str
     """
     (Future reference)
     Document ID.
     """
@@ -2178,15 +2182,15 @@
     Document metadata.
     """
 
 
 @dataclass
 class FutureFetchVectorsIn:
     """
-    (Future reference)
+    Future reference to FutureFetchVectorsIn
     """
 
     collection_name: str
     """
     (Future reference)
     Vector store name.
     """
@@ -2201,54 +2205,54 @@
     Document IDs to retrieve.
     """
 
 
 @dataclass
 class FutureFetchVectorsOut:
     """
-    (Future reference)
+    Future reference to FutureFetchVectorsOut
     """
 
     vectors: List[Vector]
     """
     (Future reference)
     Retrieved vectors.
     """
 
 
 @dataclass
 class FutureUpdateVectorsOut:
     """
-    (Future reference)
+    Future reference to FutureUpdateVectorsOut
     """
 
     count: int
     """
     (Future reference)
     Number of vectors modified.
     """
 
 
 @dataclass
 class FutureDeleteVectorsOut:
     """
-    (Future reference)
+    Future reference to FutureDeleteVectorsOut
     """
 
     count: int
     """
     (Future reference)
     Number of vectors modified.
     """
 
 
 @dataclass
 class UpdateVectorParams:
     """
-    (Future reference)
+    Future reference to UpdateVectorParams
     """
 
     id: str
     """
     (Future reference)
     Document ID.
     """
@@ -2263,15 +2267,15 @@
     Document metadata.
     """
 
 
 @dataclass
 class FutureUpdateVectorsIn:
     """
-    (Future reference)
+    Future reference to FutureUpdateVectorsIn
     """
 
     collection_name: str
     """
     (Future reference)
     Vector store name.
     """
@@ -2286,15 +2290,15 @@
     Vectors to upsert.
     """
 
 
 @dataclass
 class FutureDeleteVectorsIn:
     """
-    (Future reference)
+    Future reference to FutureDeleteVectorsIn
     """
 
     collection_name: str
     """
     (Future reference)
     Vector store name.
     """
@@ -2309,15 +2313,15 @@
     Document IDs to delete.
     """
 
 
 @dataclass
 class FutureQueryVectorStoreIn:
     """
-    (Future reference)
+    Future reference to FutureQueryVectorStoreIn
     """
 
     collection_name: str
     """
     (Future reference)
     Vector store to query against.
     """
@@ -2372,15 +2376,15 @@
     Filter metadata by key-value pairs.
     """
 
 
 @dataclass
 class VectorStoreQueryResult:
     """
-    (Future reference)
+    Future reference to VectorStoreQueryResult
     """
 
     id: str
     """
     (Future reference)
     Document ID.
     """
@@ -2400,15 +2404,15 @@
     Document metadata.
     """
 
 
 @dataclass
 class FutureQueryVectorStoreOut:
     """
-    (Future reference)
+    Future reference to FutureQueryVectorStoreOut
     """
 
     results: List[List[VectorStoreQueryResult]]
     """
     (Future reference)
     Query results.
     """
```

### Comparing `substrate-120240502.0.3/substrate/substrate.py` & `substrate-220240509.0.0/substrate/substrate.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.3/substrate/substrate_response.py` & `substrate-220240509.0.0/substrate/substrate_response.py`

 * *Files identical despite different names*

### Comparing `substrate-120240502.0.3/substrate/typeddict_models.py` & `substrate-220240509.0.0/substrate/typeddict_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-꩜ Substrate
+𐃏 Substrate
 @generated file
 (using datamodel-codegen)
 """
 
 
 from __future__ import annotations
 
@@ -113,14 +113,18 @@
 
 
 class GenerateJSONOut(TypedDict):
     json_object: NotRequired[Dict[str, Any]]
     """
     JSON response.
     """
+    text: NotRequired[str]
+    """
+    If the model output could not be parsed to JSON, this is the raw text output.
+    """
 
 
 class MultiGenerateTextIn(TypedDict):
     prompt: NotRequired[str]
     """
     Input prompt.
     """
@@ -1126,15 +1130,15 @@
     """
     collection_name: NotRequired[str]
     """
     Vector store name.
     """
     metadata: NotRequired[Dict[str, Any]]
     """
-    Metadata that can be used to query the vector store. Ignored if `store` is unset.
+    Metadata that can be used to query the vector store. Ignored if `collection_name` is unset.
     """
     embedded_metadata_keys: NotRequired[List[str]]
     """
     Choose keys from `metadata` to embed with text.
     """
     doc_id: NotRequired[str]
     """
@@ -1156,19 +1160,19 @@
 class EmbedTextItem(TypedDict):
     text: NotRequired[str]
     """
     Text to embed.
     """
     metadata: NotRequired[Dict[str, Any]]
     """
-    Metadata that can be used to query the vector store. Ignored if `store` is unset.
+    Metadata that can be used to query the vector store. Ignored if `collection_name` is unset.
     """
     doc_id: NotRequired[str]
     """
-    Vector store document ID. Ignored if `store` is unset.
+    Vector store document ID. Ignored if `collection_name` is unset.
     """
 
 
 class MultiEmbedTextIn(TypedDict):
     items: NotRequired[List[EmbedTextItem]]
     """
     Items to embed.
@@ -1223,15 +1227,15 @@
     """
     collection_name: NotRequired[str]
     """
     Vector store name.
     """
     doc_id: NotRequired[str]
     """
-    Vector store document ID. Ignored if `store` is unset.
+    Vector store document ID. Ignored if `collection_name` is unset.
     """
     model: NotRequired[Literal["clip"]]
     """
     Selected embedding model.
     """
 
 
@@ -1245,34 +1249,34 @@
 class EmbedImageItem(TypedDict):
     image_uri: NotRequired[str]
     """
     Image to embed.
     """
     doc_id: NotRequired[str]
     """
-    Vector store document ID. Ignored if `store` is unset.
+    Vector store document ID. Ignored if `collection_name` is unset.
     """
 
 
 class EmbedTextOrImageItem(TypedDict):
     image_uri: NotRequired[str]
     """
     Image to embed.
     """
     text: NotRequired[str]
     """
     Text to embed.
     """
     metadata: NotRequired[Dict[str, Any]]
     """
-    Metadata that can be used to query the vector store. Ignored if `store` is unset.
+    Metadata that can be used to query the vector store. Ignored if `collection_name` is unset.
     """
     doc_id: NotRequired[str]
     """
-    Vector store document ID. Ignored if `store` is unset.
+    Vector store document ID. Ignored if `collection_name` is unset.
     """
 
 
 class MultiEmbedImageIn(TypedDict):
     items: NotRequired[List[EmbedImageItem]]
     """
     Items to embed.
```

### Comparing `substrate-120240502.0.3/PKG-INFO` & `substrate-220240509.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrate
-Version: 120240502.0.3
+Version: 220240509.0.0
 Summary: Substrate Python SDK
 Author: vprtwn
 Author-email: ben@substrate.run
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

