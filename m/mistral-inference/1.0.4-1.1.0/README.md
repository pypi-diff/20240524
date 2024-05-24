# Comparing `tmp/mistral_inference-1.0.4.tar.gz` & `tmp/mistral_inference-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistral_inference-1.0.4.tar", max compression
+gzip compressed data, was "mistral_inference-1.1.0.tar", max compression
```

## Comparing `mistral_inference-1.0.4.tar` & `mistral_inference-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    11357 2024-05-13 15:10:07.471001 mistral_inference-1.0.4/LICENSE
--rw-r--r--   0        0        0     7760 2024-05-22 14:58:05.363410 mistral_inference-1.0.4/README.md
--rw-r--r--   0        0        0     1139 2024-05-22 09:55:48.049936 mistral_inference-1.0.4/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-22 09:55:18.014799 mistral_inference-1.0.4/src/mistral_inference/__init__.py
--rw-r--r--   0        0        0     7441 2024-05-22 15:25:31.252665 mistral_inference-1.0.4/src/mistral_inference/cache.py
--rw-r--r--   0        0        0     4262 2024-05-22 15:25:31.307427 mistral_inference-1.0.4/src/mistral_inference/generate.py
--rw-r--r--   0        0        0     5358 2024-05-20 16:49:26.556866 mistral_inference-1.0.4/src/mistral_inference/main.py
--rw-r--r--   0        0        0    14527 2024-05-22 15:25:31.311908 mistral_inference-1.0.4/src/mistral_inference/model.py
--rw-r--r--   0        0        0     1147 2024-05-20 16:41:20.124394 mistral_inference-1.0.4/src/mistral_inference/moe.py
--rw-r--r--   0        0        0      851 2024-05-20 16:41:20.128114 mistral_inference-1.0.4/src/mistral_inference/rope.py
--rw-r--r--   0        0        0     8341 1970-01-01 00:00:00.000000 mistral_inference-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-22 16:20:51.708797 mistral_inference-1.1.0/LICENSE
+-rw-r--r--   0        0        0     8340 2024-05-24 17:48:19.803435 mistral_inference-1.1.0/README.md
+-rw-r--r--   0        0        0     1139 2024-05-24 17:47:03.308982 mistral_inference-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-24 17:58:28.167380 mistral_inference-1.1.0/src/mistral_inference/__init__.py
+-rw-r--r--   0        0        0     7441 2024-05-22 16:20:51.823612 mistral_inference-1.1.0/src/mistral_inference/cache.py
+-rw-r--r--   0        0        0     4262 2024-05-22 16:20:51.826933 mistral_inference-1.1.0/src/mistral_inference/generate.py
+-rw-r--r--   0        0        0     5553 2024-05-24 17:40:19.760625 mistral_inference-1.1.0/src/mistral_inference/lora.py
+-rw-r--r--   0        0        0     5630 2024-05-24 17:45:50.081985 mistral_inference-1.1.0/src/mistral_inference/main.py
+-rw-r--r--   0        0        0    15048 2024-05-24 17:45:30.836844 mistral_inference-1.1.0/src/mistral_inference/model.py
+-rw-r--r--   0        0        0     1147 2024-05-22 16:20:51.837670 mistral_inference-1.1.0/src/mistral_inference/moe.py
+-rw-r--r--   0        0        0      851 2024-05-22 16:20:51.847072 mistral_inference-1.1.0/src/mistral_inference/rope.py
+-rw-r--r--   0        0        0     8921 1970-01-01 00:00:00.000000 mistral_inference-1.1.0/PKG-INFO
```

### Comparing `mistral_inference-1.0.4/LICENSE` & `mistral_inference-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mistral_inference-1.0.4/README.md` & `mistral_inference-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: mistral_inference
+Version: 1.1.0
+Summary: 
+Author: bam4d
+Author-email: bam4d@mistral.ai
+Requires-Python: >=3.9.10,<4.0.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: fire (>=0.6.0)
+Requires-Dist: mistral_common (>=1.0.0,<2.0.0)
+Requires-Dist: safetensors (>=0.4.0)
+Requires-Dist: simple-parsing (>=0.1.5)
+Requires-Dist: xformers (>=0.0.24)
+Description-Content-Type: text/markdown
+
 # Mistral Inference
 <a target="_blank" href="https://colab.research.google.com/github/mistralai/mistral-inference/blob/main/tutorials/getting_started.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 
 This repository contains minimal code to run our 7B, 8x7B and 8x22B models.
@@ -37,79 +55,82 @@
 | 8x7B Instruct | https://models.mistralcdn.com/mixtral-8x7b-v0-1/Mixtral-8x7B-v0.1-Instruct.tar (**Updated model coming soon!**) | `8e2d3930145dc43d3084396f49d38a3f` |
 | 8x22 Instruct | https://models.mistralcdn.com/mixtral-8x22b-v0-3/mixtral-8x22B-Instruct-v0.3.tar | `471a02a6902706a2f1e44a693813855b` |
 | 7B Base | https://models.mistralcdn.com/mistral-7b-v0-3/mistral-7B-v0.3.tar | `0663b293810d7571dad25dae2f2a5806` |
 | 8x7B |     **Updated model coming soon!**       | - |
 | 8x22B | https://models.mistralcdn.com/mixtral-8x22b-v0-3/mixtral-8x22B-v0.3.tar | `a2fa75117174f87d1197e3a4eb50371a` |
 
 Note: 
+- **Important**:
+  - `mixtral-8x22B-Instruct-v0.3.tar` is exactly the same as [Mixtral-8x22B-Instruct-v0.1](https://huggingface.co/mistralai/Mixtral-8x22B-Instruct-v0.1), only stored in `.safetensors` format
+  - `mixtral-8x22B-v0.3.tar` is the same as [Mixtral-8x22B-v0.1](https://huggingface.co/mistralai/Mixtral-8x22B-v0.1), but has an extended vocabulary of 32768 tokens.
 - All of the listed models above supports function calling. For example, Mistral 7B Base/Instruct v3 is a minor update to Mistral 7B Base/Instruct v2,  with the addition of function calling capabilities. 
 - The "coming soon" models will include function calling as well. 
 - You can download the previous versions of our models from our [docs](https://docs.mistral.ai/getting-started/open_weight_models/#downloading).
 
 
 Create a local folder to store models
 ```sh
 export MISTRAL_MODEL=$HOME/mistral_models
 mkdir -p $MISTRAL_MODEL
 ```
 
 Download any of the above links and extract the content, *e.g.*:
 
 ```sh
-export 7B_DIR=$MISTRAL_MODEL/7B_instruct
+export M7B_DIR=$MISTRAL_MODEL/7B_instruct
 wget https://models.mistralcdn.com/mistral-7b-v0-3/mistral-7B-Instruct-v0.3.tar
-mkdir -p $7B_DIR
-tar -xf Mistral-7B-v0.2-Instruct.tar -C $7B_DIR
+mkdir -p $M7B_DIR
+tar -xf mistral-7B-Instruct-v0.3.tar -C $M7B_DIR
 ```
 
 or 
 
 ```sh
-export 8x7B_DIR=$MISTRAL_MODEL/8x7b_instruct
+export M8x7B_DIR=$MISTRAL_MODEL/8x7b_instruct
 wget https://models.mistralcdn.com/mixtral-8x7b-v0-1/Mixtral-8x7B-v0.1-Instruct.tar
-mkdir -p $8x7B_DIR
-tar -xf Mixtral-8x7B-v0.1-Instruct.tar -C $8x7B_DIR
+mkdir -p $M8x7B_DIR
+tar -xf Mixtral-8x7B-v0.1-Instruct.tar -C $M8x7B_DIR
 ```
 
 ## Usage
 
 The following sections give an overview of how to run the model from the Command-line interface or from Python.
 
 ### CLI
 
 - **Demo**
 
 To test that a model works in your setup, you can run the `mistral-demo` command.
 The 7B models can be tested on a single GPU as follows:
 
 ```sh
-mistral-demo $7B_DIR
+mistral-demo $M7B_DIR
 ```
 
 Large models, such **8x7B** and **8x22B** have to be run in a multi-GPU setup.
 For these models, you can use the following command:
 
 ```sh
-torchrun --nproc-per-node 2 --no-python mistral-demo $8x7B_DIR
+torchrun --nproc-per-node 2 --no-python mistral-demo $M8x7B_DIR
 ```
 
 *Note*: Change `--nproc-per-node` to more GPUs if available.
 
 - **Chat**
 
 To interactively chat with the models, you can make use of the `mistral-chat` command.
 
 ```sh
-mistral-chat $7B_DIR --instruct
+mistral-chat $M7B_DIR --instruct
 ```
 
 For large models, you can make use of `torchrun`.
 
 ```sh
-torchrun --nproc-per-node 2 --no-python mistral-chat $8x7B_DIR --instruct
+torchrun --nproc-per-node 2 --no-python mistral-chat $M8x7B_DIR --instruct
 ```
 
 *Note*: Change `--nproc-per-node` to more GPUs if necessary (*e.g.* for 8x22B).
 
 ### Python
 
 - *Instruction Following*:
@@ -166,26 +187,28 @@
         )
     ],
     messages=[
         UserMessage(content="What's the weather like today in Paris?"),
         ],
 )
 
+tokens = tokenizer.encode_chat_completion(completion_request).tokens
+
 out_tokens, _ = generate([tokens], model, max_tokens=64, temperature=0.0, eos_id=tokenizer.instruct_tokenizer.tokenizer.eos_id)
 result = tokenizer.instruct_tokenizer.tokenizer.decode(out_tokens[0])
 
 print(result)
 ```
 
 ### One-file-ref
 
 If you want a self-contained implementation, look at `one_file_ref.py`, or run it with 
 
 ```
-python -m one_file_ref $7B_DIR
+python -m one_file_ref $M7B_DIR
 ```
 
 which should give something along the following lines:
 
 ```
 This is a test of the emergency broadcast system. This is only a test.
 
@@ -210,21 +233,25 @@
 To run logits equivalence:
 ```
 python -m pytest tests
 ```
 
 ## Deployment
 
-The `deploy` folder contains code to build a [vLLM](https://7B_DIR.com/vllm-project/vllm) image with the required dependencies to serve the Mistral AI model. In the image, the [transformers](https://github.com/huggingface/transformers/) library is used instead of the reference implementation. To build it:
+The `deploy` folder contains code to build a [vLLM](https://M7B_DIR.com/vllm-project/vllm) image with the required dependencies to serve the Mistral AI model. In the image, the [transformers](https://github.com/huggingface/transformers/) library is used instead of the reference implementation. To build it:
 
 ```bash
 docker build deploy --build-arg MAX_JOBS=8
 ```
 
 Instructions to run the image can be found in the [official documentation](https://docs.mistral.ai/quickstart).
 
 
 ## Model platforms
 
 - Use Mistral models on [Mistral AI official API](https://console.mistral.ai/) (La Plateforme)
 - Use Mistral models via [cloud providers](https://docs.mistral.ai/deployment/cloud/overview/)
 
+## References
+
+[1]: [LoRA](https://arxiv.org/abs/2106.09685): Low-Rank Adaptation of Large Language Models, Hu et al. 2021
+
```

### Comparing `mistral_inference-1.0.4/pyproject.toml` & `mistral_inference-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mistral_inference"
-version = "v1.0.4"
+version = "v1.1.0"
 description = ""
 authors = ["bam4d <bam4d@mistral.ai>"]
 readme = "README.md"
 packages = [{ include = "mistral_inference", from = "src" }]
 
 [tool.ruff]
 lint.select = ["E", "F", "W", "Q", "I"]
@@ -20,15 +20,15 @@
 no_implicit_optional = true
 warn_return_any = true
 warn_unused_ignores = true
 exclude = ["docs", "tools", "build"]
 
 [tool.poetry.dependencies]
 python = "^3.9.10"
-xformers = ">=0.0.25"
+xformers = ">=0.0.24"
 simple-parsing = ">=0.1.5"
 fire = ">=0.6.0"
 mistral_common = "^1.0.0"
 safetensors = ">=0.4.0"
 
 [tool.poetry.group.dev.dependencies]
 types-protobuf = "4.24.0.20240129"
```

### Comparing `mistral_inference-1.0.4/src/mistral_inference/cache.py` & `mistral_inference-1.1.0/src/mistral_inference/cache.py`

 * *Files identical despite different names*

### Comparing `mistral_inference-1.0.4/src/mistral_inference/generate.py` & `mistral_inference-1.1.0/src/mistral_inference/generate.py`

 * *Files identical despite different names*

### Comparing `mistral_inference-1.0.4/src/mistral_inference/main.py` & `mistral_inference-1.1.0/src/mistral_inference/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import os
 from pathlib import Path
-from typing import List
+from typing import List, Optional
 
 import fire  # type: ignore
 import torch
 import torch.distributed as dist
 from mistral_common.protocol.instruct.messages import AssistantMessage, UserMessage
 from mistral_common.protocol.instruct.request import ChatCompletionRequest
 from mistral_common.tokens.tokenizers.base import Tokenizer
@@ -42,14 +42,15 @@
 
 def interactive(
     model_path: str,
     max_tokens: int = 35,
     temperature: float = 0.7,
     num_pipeline_ranks: int = 1,
     instruct: bool = False,
+    lora_path: Optional[str] = None,
 ) -> None:
     if is_torchrun():
         torch.distributed.init_process_group()
         torch.cuda.set_device(torch.distributed.get_rank())
         should_print = torch.distributed.get_rank() == 0
 
         num_pipeline_ranks = torch.distributed.get_world_size()
@@ -60,14 +61,18 @@
     mistral_tokenizer: MistralTokenizer = load_tokenizer(Path(model_path))
     tokenizer: Tokenizer = mistral_tokenizer.instruct_tokenizer.tokenizer
 
     transformer = Transformer.from_folder(
         Path(model_path), max_batch_size=3, num_pipeline_ranks=num_pipeline_ranks
     )
 
+    # load LoRA
+    if lora_path is not None:
+        transformer.load_lora(Path(lora_path))
+
     prompt: str = ""
     messages: List[UserMessage | AssistantMessage] = []
 
     while True:
         if should_print:
             user_input = input("Prompt: ")
 
@@ -113,28 +118,33 @@
             prompt += answer
 
 
 def demo(
     model_path: str,
     max_tokens: int = 35,
     temperature: float = 0,
+    lora_path: Optional[str] = None,
 ) -> None:
     if is_torchrun():
         torch.distributed.init_process_group()
         torch.cuda.set_device(torch.distributed.get_rank())
         should_print = torch.distributed.get_rank() == 0
 
         num_pipeline_ranks = torch.distributed.get_world_size()
     else:
         should_print = True
         num_pipeline_ranks = 1
 
     transformer = Transformer.from_folder(
         Path(model_path), max_batch_size=3, num_pipeline_ranks=num_pipeline_ranks
     )
+    # load LoRA
+    if lora_path is not None:
+        transformer.load_lora(Path(lora_path))
+
     mistral_tokenizer: MistralTokenizer = load_tokenizer(Path(model_path))
     tokenizer: Tokenizer = mistral_tokenizer.instruct_tokenizer.tokenizer
 
     prompts = [
         "This is a test",
         "This is another great test",
         "This is a third test, mistral AI is very good at testing. ",
```

### Comparing `mistral_inference-1.0.4/src/mistral_inference/model.py` & `mistral_inference-1.1.0/src/mistral_inference/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import json
 import logging
 import math
 from dataclasses import dataclass
+from functools import partial
 from pathlib import Path
 from typing import Any, List, Mapping, Optional, Tuple, Union
 
 import safetensors.torch
 import torch
 from simple_parsing.helpers import Serializable
 from torch import nn
 from xformers.ops.fmha import memory_efficient_attention  # type: ignore
 
 from mistral_inference.cache import (
     BufferCache,
     CacheInputMetadata,
     CacheView,
 )
+from mistral_inference.lora import LoraArgs, LoRALinear, LoRALoaderMixin
 from mistral_inference.moe import MoeArgs, MoeLayer
 from mistral_inference.rope import apply_rotary_emb, precompute_freqs_cis
 
 
 @dataclass
 class ModelArgs(Serializable):
     dim: int
@@ -33,14 +35,16 @@
 
     max_batch_size: int = 0
 
     # For rotary embeddings. If not set, will be infered
     rope_theta: Optional[float] = None
     # If this is set, we will use MoE layers instead of dense layers.
     moe: Optional[MoeArgs] = None
+    # If this is set, we will load LoRA linear layers instead of linear layers.
+    lora: Optional[LoraArgs] = None
 
 
 @dataclass
 class SimpleInputMetadata:
     # rope absolute positions
     positions: torch.Tensor
 
@@ -57,31 +61,39 @@
     keys: torch.Tensor, values: torch.Tensor, repeats: int, dim: int
 ) -> Tuple[torch.Tensor, torch.Tensor]:
     keys = torch.repeat_interleave(keys, repeats=repeats, dim=dim)
     values = torch.repeat_interleave(values, repeats=repeats, dim=dim)
     return keys, values
 
 
+def maybe_lora(args: ModelArgs) -> Union[nn.Linear, LoRALinear]:
+    if args.lora is None:
+        return nn.Linear
+    else:
+        return partial(LoRALinear, rank=args.lora.rank, scaling=args.lora.scaling)
+
+
 class Attention(nn.Module):
     def __init__(self, args: ModelArgs):
         super().__init__()
         self.args = args
 
         self.n_heads: int = args.n_heads
         self.head_dim: int = args.head_dim
         self.n_kv_heads: int = args.n_kv_heads
 
         self.repeats = self.n_heads // self.n_kv_heads
 
         self.scale = self.args.head_dim**-0.5
 
-        self.wq = nn.Linear(args.dim, args.n_heads * args.head_dim, bias=False)
-        self.wk = nn.Linear(args.dim, args.n_kv_heads * args.head_dim, bias=False)
-        self.wv = nn.Linear(args.dim, args.n_kv_heads * args.head_dim, bias=False)
-        self.wo = nn.Linear(args.n_heads * args.head_dim, args.dim, bias=False)
+        MaybeLora = maybe_lora(args)
+        self.wq = MaybeLora(args.dim, args.n_heads * args.head_dim, bias=False)
+        self.wk = MaybeLora(args.dim, args.n_kv_heads * args.head_dim, bias=False)
+        self.wv = MaybeLora(args.dim, args.n_kv_heads * args.head_dim, bias=False)
+        self.wo = MaybeLora(args.n_heads * args.head_dim, args.dim, bias=False)
 
     def forward(
         self,
         x: torch.Tensor,
         freqs_cis: torch.Tensor,
         cache: Optional[CacheView],
     ) -> torch.Tensor:
@@ -123,17 +135,18 @@
         return self.wo(output)  # type: ignore
 
 
 class FeedForward(nn.Module):
     def __init__(self, args: ModelArgs):
         super().__init__()
 
-        self.w1 = nn.Linear(args.dim, args.hidden_dim, bias=False)
-        self.w2 = nn.Linear(args.hidden_dim, args.dim, bias=False)
-        self.w3 = nn.Linear(args.dim, args.hidden_dim, bias=False)
+        MaybeLora = maybe_lora(args)
+        self.w1 = MaybeLora(args.dim, args.hidden_dim, bias=False)
+        self.w2 = MaybeLora(args.hidden_dim, args.dim, bias=False)
+        self.w3 = MaybeLora(args.dim, args.hidden_dim, bias=False)
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         return self.w2(nn.functional.silu(self.w1(x)) * self.w3(x))  # type: ignore
 
 
 class RMSNorm(torch.nn.Module):
     def __init__(self, dim: int, eps: float = 1e-6):
@@ -175,15 +188,15 @@
         r = self.attention.forward(self.attention_norm(x), freqs_cis, cache)
         h = x + r
         r = self.feed_forward.forward(self.ffn_norm(h))
         out = h + r
         return out
 
 
-class Transformer(nn.Module):
+class Transformer(nn.Module, LoRALoaderMixin):
     def __init__(
         self,
         args: ModelArgs,
         pipeline_rank: int = 0,
         num_pipeline_ranks: int = 1,
     ):
         super().__init__()
```

### Comparing `mistral_inference-1.0.4/src/mistral_inference/moe.py` & `mistral_inference-1.1.0/src/mistral_inference/moe.py`

 * *Files identical despite different names*

### Comparing `mistral_inference-1.0.4/src/mistral_inference/rope.py` & `mistral_inference-1.1.0/src/mistral_inference/rope.py`

 * *Files identical despite different names*

### Comparing `mistral_inference-1.0.4/PKG-INFO` & `mistral_inference-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: mistral_inference
-Version: 1.0.4
-Summary: 
-Author: bam4d
-Author-email: bam4d@mistral.ai
-Requires-Python: >=3.9.10,<4.0.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: fire (>=0.6.0)
-Requires-Dist: mistral_common (>=1.0.0,<2.0.0)
-Requires-Dist: safetensors (>=0.4.0)
-Requires-Dist: simple-parsing (>=0.1.5)
-Requires-Dist: xformers (>=0.0.25)
-Description-Content-Type: text/markdown
-
 # Mistral Inference
 <a target="_blank" href="https://colab.research.google.com/github/mistralai/mistral-inference/blob/main/tutorials/getting_started.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 
 This repository contains minimal code to run our 7B, 8x7B and 8x22B models.
@@ -55,79 +37,82 @@
 | 8x7B Instruct | https://models.mistralcdn.com/mixtral-8x7b-v0-1/Mixtral-8x7B-v0.1-Instruct.tar (**Updated model coming soon!**) | `8e2d3930145dc43d3084396f49d38a3f` |
 | 8x22 Instruct | https://models.mistralcdn.com/mixtral-8x22b-v0-3/mixtral-8x22B-Instruct-v0.3.tar | `471a02a6902706a2f1e44a693813855b` |
 | 7B Base | https://models.mistralcdn.com/mistral-7b-v0-3/mistral-7B-v0.3.tar | `0663b293810d7571dad25dae2f2a5806` |
 | 8x7B |     **Updated model coming soon!**       | - |
 | 8x22B | https://models.mistralcdn.com/mixtral-8x22b-v0-3/mixtral-8x22B-v0.3.tar | `a2fa75117174f87d1197e3a4eb50371a` |
 
 Note: 
+- **Important**:
+  - `mixtral-8x22B-Instruct-v0.3.tar` is exactly the same as [Mixtral-8x22B-Instruct-v0.1](https://huggingface.co/mistralai/Mixtral-8x22B-Instruct-v0.1), only stored in `.safetensors` format
+  - `mixtral-8x22B-v0.3.tar` is the same as [Mixtral-8x22B-v0.1](https://huggingface.co/mistralai/Mixtral-8x22B-v0.1), but has an extended vocabulary of 32768 tokens.
 - All of the listed models above supports function calling. For example, Mistral 7B Base/Instruct v3 is a minor update to Mistral 7B Base/Instruct v2,  with the addition of function calling capabilities. 
 - The "coming soon" models will include function calling as well. 
 - You can download the previous versions of our models from our [docs](https://docs.mistral.ai/getting-started/open_weight_models/#downloading).
 
 
 Create a local folder to store models
 ```sh
 export MISTRAL_MODEL=$HOME/mistral_models
 mkdir -p $MISTRAL_MODEL
 ```
 
 Download any of the above links and extract the content, *e.g.*:
 
 ```sh
-export 7B_DIR=$MISTRAL_MODEL/7B_instruct
+export M7B_DIR=$MISTRAL_MODEL/7B_instruct
 wget https://models.mistralcdn.com/mistral-7b-v0-3/mistral-7B-Instruct-v0.3.tar
-mkdir -p $7B_DIR
-tar -xf Mistral-7B-v0.2-Instruct.tar -C $7B_DIR
+mkdir -p $M7B_DIR
+tar -xf mistral-7B-Instruct-v0.3.tar -C $M7B_DIR
 ```
 
 or 
 
 ```sh
-export 8x7B_DIR=$MISTRAL_MODEL/8x7b_instruct
+export M8x7B_DIR=$MISTRAL_MODEL/8x7b_instruct
 wget https://models.mistralcdn.com/mixtral-8x7b-v0-1/Mixtral-8x7B-v0.1-Instruct.tar
-mkdir -p $8x7B_DIR
-tar -xf Mixtral-8x7B-v0.1-Instruct.tar -C $8x7B_DIR
+mkdir -p $M8x7B_DIR
+tar -xf Mixtral-8x7B-v0.1-Instruct.tar -C $M8x7B_DIR
 ```
 
 ## Usage
 
 The following sections give an overview of how to run the model from the Command-line interface or from Python.
 
 ### CLI
 
 - **Demo**
 
 To test that a model works in your setup, you can run the `mistral-demo` command.
 The 7B models can be tested on a single GPU as follows:
 
 ```sh
-mistral-demo $7B_DIR
+mistral-demo $M7B_DIR
 ```
 
 Large models, such **8x7B** and **8x22B** have to be run in a multi-GPU setup.
 For these models, you can use the following command:
 
 ```sh
-torchrun --nproc-per-node 2 --no-python mistral-demo $8x7B_DIR
+torchrun --nproc-per-node 2 --no-python mistral-demo $M8x7B_DIR
 ```
 
 *Note*: Change `--nproc-per-node` to more GPUs if available.
 
 - **Chat**
 
 To interactively chat with the models, you can make use of the `mistral-chat` command.
 
 ```sh
-mistral-chat $7B_DIR --instruct
+mistral-chat $M7B_DIR --instruct
 ```
 
 For large models, you can make use of `torchrun`.
 
 ```sh
-torchrun --nproc-per-node 2 --no-python mistral-chat $8x7B_DIR --instruct
+torchrun --nproc-per-node 2 --no-python mistral-chat $M8x7B_DIR --instruct
 ```
 
 *Note*: Change `--nproc-per-node` to more GPUs if necessary (*e.g.* for 8x22B).
 
 ### Python
 
 - *Instruction Following*:
@@ -184,26 +169,28 @@
         )
     ],
     messages=[
         UserMessage(content="What's the weather like today in Paris?"),
         ],
 )
 
+tokens = tokenizer.encode_chat_completion(completion_request).tokens
+
 out_tokens, _ = generate([tokens], model, max_tokens=64, temperature=0.0, eos_id=tokenizer.instruct_tokenizer.tokenizer.eos_id)
 result = tokenizer.instruct_tokenizer.tokenizer.decode(out_tokens[0])
 
 print(result)
 ```
 
 ### One-file-ref
 
 If you want a self-contained implementation, look at `one_file_ref.py`, or run it with 
 
 ```
-python -m one_file_ref $7B_DIR
+python -m one_file_ref $M7B_DIR
 ```
 
 which should give something along the following lines:
 
 ```
 This is a test of the emergency broadcast system. This is only a test.
 
@@ -228,22 +215,24 @@
 To run logits equivalence:
 ```
 python -m pytest tests
 ```
 
 ## Deployment
 
-The `deploy` folder contains code to build a [vLLM](https://7B_DIR.com/vllm-project/vllm) image with the required dependencies to serve the Mistral AI model. In the image, the [transformers](https://github.com/huggingface/transformers/) library is used instead of the reference implementation. To build it:
+The `deploy` folder contains code to build a [vLLM](https://M7B_DIR.com/vllm-project/vllm) image with the required dependencies to serve the Mistral AI model. In the image, the [transformers](https://github.com/huggingface/transformers/) library is used instead of the reference implementation. To build it:
 
 ```bash
 docker build deploy --build-arg MAX_JOBS=8
 ```
 
 Instructions to run the image can be found in the [official documentation](https://docs.mistral.ai/quickstart).
 
 
 ## Model platforms
 
 - Use Mistral models on [Mistral AI official API](https://console.mistral.ai/) (La Plateforme)
 - Use Mistral models via [cloud providers](https://docs.mistral.ai/deployment/cloud/overview/)
 
+## References
 
+[1]: [LoRA](https://arxiv.org/abs/2106.09685): Low-Rank Adaptation of Large Language Models, Hu et al. 2021
```

