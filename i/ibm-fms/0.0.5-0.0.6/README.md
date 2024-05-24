# Comparing `tmp/ibm_fms-0.0.5-py3-none-any.whl.zip` & `tmp/ibm_fms-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,58 +1,65 @@
-Zip file size: 98901 bytes, number of entries: 56
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-09 13:04 fms/__init__.py
--rw-r--r--  2.0 unx     1786 b- defN 24-Apr-09 13:04 fms/datasets/__init__.py
--rw-r--r--  2.0 unx     5384 b- defN 24-Apr-09 13:04 fms/datasets/arrow.py
--rw-r--r--  2.0 unx     3055 b- defN 24-Apr-09 13:04 fms/datasets/instructions.py
--rw-r--r--  2.0 unx     2968 b- defN 24-Apr-09 13:04 fms/datasets/text.py
--rw-r--r--  2.0 unx     5159 b- defN 24-Apr-09 13:04 fms/datasets/util.py
--rw-r--r--  2.0 unx      590 b- defN 24-Apr-09 13:04 fms/distributed/__init__.py
--rw-r--r--  2.0 unx     4006 b- defN 24-Apr-09 13:04 fms/distributed/strategy.py
--rw-r--r--  2.0 unx     7423 b- defN 24-Apr-09 13:04 fms/distributed/tensorparallel.py
--rw-r--r--  2.0 unx    10549 b- defN 24-Apr-09 13:04 fms/models/__init__.py
--rw-r--r--  2.0 unx    15081 b- defN 24-Apr-22 18:19 fms/models/gpt_bigcode.py
--rw-r--r--  2.0 unx    18367 b- defN 24-Apr-09 13:04 fms/models/llama.py
--rw-r--r--  2.0 unx    10683 b- defN 24-Apr-09 13:04 fms/models/roberta.py
--rw-r--r--  2.0 unx     1426 b- defN 24-Apr-09 13:04 fms/models/hf/__init__.py
--rw-r--r--  2.0 unx    14675 b- defN 24-Apr-09 13:04 fms/models/hf/lm_head_mixins.py
--rw-r--r--  2.0 unx    84324 b- defN 24-Apr-09 13:04 fms/models/hf/modeling_hf_adapter.py
--rw-r--r--  2.0 unx     4775 b- defN 24-Apr-09 13:04 fms/models/hf/utils.py
--rw-r--r--  2.0 unx     3488 b- defN 24-Apr-09 13:04 fms/models/hf/gpt_bigcode/__init__.py
--rw-r--r--  2.0 unx     2659 b- defN 24-Apr-09 13:04 fms/models/hf/gpt_bigcode/configuration_gpt_bigcode_hf.py
--rw-r--r--  2.0 unx     3420 b- defN 24-Apr-09 13:04 fms/models/hf/gpt_bigcode/modeling_gpt_bigcode_hf.py
--rw-r--r--  2.0 unx     1498 b- defN 24-Apr-09 13:04 fms/models/hf/llama/__init__.py
--rw-r--r--  2.0 unx     2509 b- defN 24-Apr-09 13:04 fms/models/hf/llama/configuration_llama_hf.py
--rw-r--r--  2.0 unx     4822 b- defN 24-Apr-09 13:04 fms/models/hf/llama/modeling_llama_hf.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-09 13:04 fms/models/hf/roberta/__init__.py
--rw-r--r--  2.0 unx     6187 b- defN 24-Apr-09 13:04 fms/models/hf/roberta/modeling_roberta_hf.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-09 13:04 fms/modules/__init__.py
--rw-r--r--  2.0 unx    12229 b- defN 24-Apr-09 13:04 fms/modules/attention.py
--rw-r--r--  2.0 unx     8306 b- defN 24-Apr-09 13:04 fms/modules/embedding.py
--rw-r--r--  2.0 unx     8944 b- defN 24-Apr-09 13:04 fms/modules/feedforward.py
--rw-r--r--  2.0 unx     2467 b- defN 24-Apr-09 13:04 fms/modules/head.py
--rw-r--r--  2.0 unx     2488 b- defN 24-Apr-09 13:04 fms/modules/layernorm.py
--rw-r--r--  2.0 unx     9492 b- defN 24-Apr-09 13:04 fms/modules/positions.py
--rw-r--r--  2.0 unx     2661 b- defN 24-Apr-09 13:04 fms/modules/tp.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-09 13:04 fms/testing/__init__.py
--rw-r--r--  2.0 unx     5596 b- defN 24-Apr-09 13:04 fms/testing/comparison.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-09 13:04 fms/testing/_internal/__init__.py
--rw-r--r--  2.0 unx     9461 b- defN 24-Apr-09 13:04 fms/testing/_internal/model_test_suite.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-09 13:04 fms/testing/_internal/hf/__init__.py
--rw-r--r--  2.0 unx    14836 b- defN 24-Apr-09 13:04 fms/testing/_internal/hf/model_test_suite.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-09 13:04 fms/training/__init__.py
--rw-r--r--  2.0 unx    12732 b- defN 24-Apr-17 13:44 fms/training/plugins.py
--rw-r--r--  2.0 unx     3086 b- defN 24-Apr-17 13:44 fms/training/trainer.py
--rw-r--r--  2.0 unx      650 b- defN 24-Apr-09 13:04 fms/utils/__init__.py
--rw-r--r--  2.0 unx     2020 b- defN 24-Apr-09 13:04 fms/utils/activation.py
--rw-r--r--  2.0 unx     1872 b- defN 24-Apr-09 13:04 fms/utils/config.py
--rw-r--r--  2.0 unx     2626 b- defN 24-Apr-09 13:04 fms/utils/evaluation.py
--rw-r--r--  2.0 unx     4377 b- defN 24-Apr-09 13:04 fms/utils/generation.py
--rw-r--r--  2.0 unx    18133 b- defN 24-Apr-22 18:19 fms/utils/serialization.py
--rw-r--r--  2.0 unx     4982 b- defN 24-Apr-09 13:04 fms/utils/tensors.py
--rw-r--r--  2.0 unx     5337 b- defN 24-Apr-09 13:04 fms/utils/tokenizers.py
--rw-r--r--  2.0 unx     1596 b- defN 24-Apr-09 13:04 fms/utils/tp_wrapping.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Apr-22 18:19 ibm_fms-0.0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx      683 b- defN 24-Apr-22 18:19 ibm_fms-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 18:19 ibm_fms-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 24-Apr-22 18:19 ibm_fms-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4689 b- defN 24-Apr-22 18:19 ibm_fms-0.0.5.dist-info/RECORD
-56 files, 365550 bytes uncompressed, 91485 bytes compressed:  75.0%
+Zip file size: 117767 bytes, number of entries: 63
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-06 15:32 fms/__init__.py
+-rw-rw-r--  2.0 unx      152 b- defN 24-Mar-21 20:02 fms/py.typed
+-rw-rw-r--  2.0 unx     1786 b- defN 24-Apr-16 13:19 fms/datasets/__init__.py
+-rw-rw-r--  2.0 unx     5384 b- defN 24-Apr-16 13:19 fms/datasets/arrow.py
+-rw-rw-r--  2.0 unx     3055 b- defN 24-Apr-16 13:19 fms/datasets/instructions.py
+-rw-rw-r--  2.0 unx     2968 b- defN 24-Apr-16 13:19 fms/datasets/text.py
+-rw-rw-r--  2.0 unx     5159 b- defN 24-Apr-16 13:19 fms/datasets/util.py
+-rw-rw-r--  2.0 unx      590 b- defN 24-Apr-16 13:19 fms/distributed/__init__.py
+-rw-rw-r--  2.0 unx     4006 b- defN 24-Feb-06 15:32 fms/distributed/strategy.py
+-rw-rw-r--  2.0 unx     5642 b- defN 24-May-16 14:10 fms/distributed/tensorparallel.py
+-rw-rw-r--  2.0 unx    10567 b- defN 24-May-24 18:29 fms/models/__init__.py
+-rw-rw-r--  2.0 unx    13972 b- defN 24-May-17 14:42 fms/models/gpt_bigcode.py
+-rw-rw-r--  2.0 unx    18777 b- defN 24-May-24 18:29 fms/models/llama.py
+-rw-rw-r--  2.0 unx    14397 b- defN 24-May-17 14:42 fms/models/mixtral.py
+-rw-rw-r--  2.0 unx    10861 b- defN 24-May-17 14:42 fms/models/roberta.py
+-rw-rw-r--  2.0 unx     1766 b- defN 24-May-16 14:10 fms/models/hf/__init__.py
+-rw-rw-r--  2.0 unx    14684 b- defN 24-May-16 14:10 fms/models/hf/lm_head_mixins.py
+-rw-rw-r--  2.0 unx    84324 b- defN 24-Mar-21 20:02 fms/models/hf/modeling_hf_adapter.py
+-rw-rw-r--  2.0 unx     4775 b- defN 24-Feb-06 15:32 fms/models/hf/utils.py
+-rw-rw-r--  2.0 unx     3014 b- defN 24-May-17 14:42 fms/models/hf/gpt_bigcode/__init__.py
+-rw-rw-r--  2.0 unx     2659 b- defN 24-Apr-16 13:19 fms/models/hf/gpt_bigcode/configuration_gpt_bigcode_hf.py
+-rw-rw-r--  2.0 unx     3420 b- defN 24-Mar-21 20:02 fms/models/hf/gpt_bigcode/modeling_gpt_bigcode_hf.py
+-rw-rw-r--  2.0 unx     1498 b- defN 24-Feb-06 15:32 fms/models/hf/llama/__init__.py
+-rw-rw-r--  2.0 unx     2509 b- defN 24-Feb-06 15:32 fms/models/hf/llama/configuration_llama_hf.py
+-rw-rw-r--  2.0 unx     4822 b- defN 24-Mar-21 20:02 fms/models/hf/llama/modeling_llama_hf.py
+-rw-rw-r--  2.0 unx     3754 b- defN 24-May-17 14:42 fms/models/hf/mixtral/__init__.py
+-rw-rw-r--  2.0 unx     2697 b- defN 24-May-16 14:10 fms/models/hf/mixtral/configuration_mixtral_hf.py
+-rw-rw-r--  2.0 unx     4607 b- defN 24-May-16 14:10 fms/models/hf/mixtral/modeling_mixtral_hf.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-06 15:32 fms/models/hf/roberta/__init__.py
+-rw-rw-r--  2.0 unx     6319 b- defN 24-May-16 14:10 fms/models/hf/roberta/modeling_roberta_hf.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-06 15:32 fms/modules/__init__.py
+-rw-rw-r--  2.0 unx    21990 b- defN 24-May-17 14:42 fms/modules/attention.py
+-rw-rw-r--  2.0 unx    12304 b- defN 24-May-16 14:10 fms/modules/embedding.py
+-rw-rw-r--  2.0 unx    18900 b- defN 24-May-24 18:29 fms/modules/feedforward.py
+-rw-rw-r--  2.0 unx     5777 b- defN 24-May-16 14:10 fms/modules/head.py
+-rw-rw-r--  2.0 unx     2488 b- defN 24-Apr-16 13:19 fms/modules/layernorm.py
+-rw-rw-r--  2.0 unx     9529 b- defN 24-May-16 14:10 fms/modules/positions.py
+-rw-rw-r--  2.0 unx     7727 b- defN 24-May-17 14:42 fms/modules/tp.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-06 15:32 fms/testing/__init__.py
+-rw-rw-r--  2.0 unx     5596 b- defN 24-Feb-06 15:32 fms/testing/comparison.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-06 15:32 fms/testing/_internal/__init__.py
+-rw-rw-r--  2.0 unx     9461 b- defN 24-Feb-21 19:05 fms/testing/_internal/model_test_suite.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-06 15:32 fms/testing/_internal/hf/__init__.py
+-rw-rw-r--  2.0 unx    14836 b- defN 24-Feb-06 15:32 fms/testing/_internal/hf/model_test_suite.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Feb-06 15:32 fms/training/__init__.py
+-rw-rw-r--  2.0 unx    12732 b- defN 24-May-02 15:13 fms/training/plugins.py
+-rw-rw-r--  2.0 unx     3086 b- defN 24-May-02 15:13 fms/training/trainer.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-16 14:10 fms/triton/__init__.py
+-rw-rw-r--  2.0 unx    15441 b- defN 24-May-16 14:10 fms/triton/moe_kernel.py
+-rw-rw-r--  2.0 unx      650 b- defN 24-Apr-16 13:19 fms/utils/__init__.py
+-rw-rw-r--  2.0 unx     2020 b- defN 24-Feb-06 15:32 fms/utils/activation.py
+-rw-rw-r--  2.0 unx     1872 b- defN 24-Feb-06 15:32 fms/utils/config.py
+-rw-rw-r--  2.0 unx     2626 b- defN 24-Mar-21 20:02 fms/utils/evaluation.py
+-rw-rw-r--  2.0 unx     4793 b- defN 24-May-24 18:29 fms/utils/generation.py
+-rw-rw-r--  2.0 unx    17672 b- defN 24-May-24 18:29 fms/utils/serialization.py
+-rw-rw-r--  2.0 unx     4982 b- defN 24-Mar-21 20:02 fms/utils/tensors.py
+-rw-rw-r--  2.0 unx     5337 b- defN 24-Feb-06 15:32 fms/utils/tokenizers.py
+-rw-rw-r--  2.0 unx     1113 b- defN 24-May-16 14:10 fms/utils/tp_wrapping.py
+-rw-rw-r--  2.0 unx    11357 b- defN 24-May-24 18:42 ibm_fms-0.0.6.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      679 b- defN 24-May-24 18:42 ibm_fms-0.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-24 18:42 ibm_fms-0.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        4 b- defN 24-May-24 18:42 ibm_fms-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     5293 b- defN 24-May-24 18:42 ibm_fms-0.0.6.dist-info/RECORD
+63 files, 436521 bytes uncompressed, 109409 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: fms/__init__.py
 Comment: 
 
+Filename: fms/py.typed
+Comment: 
+
 Filename: fms/datasets/__init__.py
 Comment: 
 
 Filename: fms/datasets/arrow.py
 Comment: 
 
 Filename: fms/datasets/instructions.py
@@ -30,14 +33,17 @@
 
 Filename: fms/models/gpt_bigcode.py
 Comment: 
 
 Filename: fms/models/llama.py
 Comment: 
 
+Filename: fms/models/mixtral.py
+Comment: 
+
 Filename: fms/models/roberta.py
 Comment: 
 
 Filename: fms/models/hf/__init__.py
 Comment: 
 
 Filename: fms/models/hf/lm_head_mixins.py
@@ -63,14 +69,23 @@
 
 Filename: fms/models/hf/llama/configuration_llama_hf.py
 Comment: 
 
 Filename: fms/models/hf/llama/modeling_llama_hf.py
 Comment: 
 
+Filename: fms/models/hf/mixtral/__init__.py
+Comment: 
+
+Filename: fms/models/hf/mixtral/configuration_mixtral_hf.py
+Comment: 
+
+Filename: fms/models/hf/mixtral/modeling_mixtral_hf.py
+Comment: 
+
 Filename: fms/models/hf/roberta/__init__.py
 Comment: 
 
 Filename: fms/models/hf/roberta/modeling_roberta_hf.py
 Comment: 
 
 Filename: fms/modules/__init__.py
@@ -120,14 +135,20 @@
 
 Filename: fms/training/plugins.py
 Comment: 
 
 Filename: fms/training/trainer.py
 Comment: 
 
+Filename: fms/triton/__init__.py
+Comment: 
+
+Filename: fms/triton/moe_kernel.py
+Comment: 
+
 Filename: fms/utils/__init__.py
 Comment: 
 
 Filename: fms/utils/activation.py
 Comment: 
 
 Filename: fms/utils/config.py
@@ -147,23 +168,23 @@
 
 Filename: fms/utils/tokenizers.py
 Comment: 
 
 Filename: fms/utils/tp_wrapping.py
 Comment: 
 
-Filename: ibm_fms-0.0.5.dist-info/LICENSE
+Filename: ibm_fms-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: ibm_fms-0.0.5.dist-info/METADATA
+Filename: ibm_fms-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: ibm_fms-0.0.5.dist-info/WHEEL
+Filename: ibm_fms-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: ibm_fms-0.0.5.dist-info/top_level.txt
+Filename: ibm_fms-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: ibm_fms-0.0.5.dist-info/RECORD
+Filename: ibm_fms-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fms/distributed/tensorparallel.py

```diff
@@ -4,51 +4,14 @@
 import torch._inductor.ir as ir
 import torch._inductor.lowering as lowering
 import torch.distributed as dist
 import torch.distributed._functional_collectives as funcol
 from torch import nn
 
 
-def apply_colwise_tp(par_mod: nn.Linear, mod: nn.Linear, world_size, rank):
-    # Divide the weight matrix along the last dimension.
-    output_size_per_partition = mod.out_features // world_size
-    with torch.no_grad():
-        par_mod.weight.copy_(
-            torch.split(mod.weight, output_size_per_partition, dim=0)[rank]
-        )
-        if par_mod.bias is not None:
-            par_mod.bias.copy_(torch.split(mod.bias, output_size_per_partition)[rank])
-    # print(f"For rank {rank}, we have the following weights: Base weight {mod.weight} bias {mod.bias}; Par weight {par_mod.weight}, bias {par_mod.bias}")
-
-
-def apply_rowwise_tp(par_mod: nn.Linear, mod: nn.Linear, world_size, rank):
-    # Divide the weight matrix along the last dimension.
-    output_size_per_partition = mod.in_features // world_size
-    with torch.no_grad():
-        par_mod.weight.copy_(
-            torch.split(mod.weight, output_size_per_partition, dim=1)[rank]
-        )
-        if par_mod.bias is not None:
-            if rank == 0:
-                par_mod.bias.copy_(mod.bias)
-            else:
-                par_mod.bias.zero_()
-    # print(f"For rank {rank}, we have the following weights: Base weight {mod.weight}, bias {mod.bias}; Par weight {par_mod.weight}, bias {par_mod.bias}")
-
-
-def apply_embedding_tp(par_mod: nn.Embedding, mod: nn.Embedding, world_size, rank):
-    # Divide the weight matrix along the last dimension.
-    output_size_per_partition = mod.embedding_dim // world_size
-    with torch.no_grad():
-        par_mod.weight.copy_(
-            torch.split(mod.weight, output_size_per_partition, dim=1)[rank]
-        )
-    # print(f"For rank {rank}, we have the following weights: Base weight {mod.weight} bias {mod.bias}; Par weight {par_mod.weight}, bias {par_mod.bias}")
-
-
 ## Fixes for PT 2.2 collectives until PT 2.3 is released
 
 
 # Fix 1: https://github.com/pytorch/pytorch/issues/121311
 def get_volatile_reads_fixed(self):
     inp = self.inputs[0]
     if isinstance(inp, ir._CollectiveKernel):
```

## fms/models/__init__.py

```diff
@@ -111,15 +111,15 @@
         )
 
     layers = set()
     import re
 
     for key in state_dict.keys():
         # when there's a list of layers, layers have numeric IDs in the key
-        layerid = re.sub("[^.]*\.([0-9]+)\..*", "\\1", key)
+        layerid = re.sub("[^.]*\\.([0-9]+)\\..*", "\\1", key)
         if layerid != key:
             layers.add(layerid)
     return len(layers)
 
 
 def _class_hierarchy(clz):
     if clz == object:
@@ -247,16 +247,19 @@
         device = torch.device(device_type, local_rank)
     else:
         device = torch.device(device_type)
 
     hsdp = distributed_strategy == "hsdp"
     fsdp = distributed_strategy == "fsdp"
     ddp = distributed_strategy == "ddp"
-    if (hsdp and local_rank != 0) or ((fsdp or ddp) and rank != 0):
-        initial_device = torch.device("meta")
+    if hsdp or fsdp or ddp:
+        if (hsdp and local_rank != 0) or ((fsdp or ddp) and rank != 0):
+            initial_device = torch.device("meta")
+        else:
+            initial_device = torch.device("cpu")
     elif distributed_strategy == "mp":
         initial_device = torch.device("cpu")
     else:
         initial_device = device
 
     lazy_sd: MutableMapping[str, Any] = {}
     if model_path is not None:
@@ -306,20 +309,18 @@
             fms_model,
             lazy_sd,
             architecture,
             source if source is not None else "fms",
             distributed_strategy,
             checkpoint_sharding,
             initial_device,
-            local_rank if distributed_strategy == "hsdp" else rank,
-            world_size,
         )
     elif hasattr(fms_model, "reset_parameters"):
         fms_model.reset_parameters()
 
     if pre_load:
         fms_model = model_wrap(fms_model)
 
     return fms_model
 
 
-from fms.models import gpt_bigcode, llama, roberta
+from fms.models import gpt_bigcode, llama, mixtral, roberta
```

## fms/models/gpt_bigcode.py

```diff
@@ -76,16 +76,14 @@
 
         # first we do MHA and Add&Norm
         residual = x
         x = self.ln(x)
         # self attention
         x = self.attn(
             q=x,
-            k=x,
-            v=x,
             mask=mask,
             position_ids=position_ids,
             attn_algorithm=attn_algorithm,
             past_key_value_state=self_attn_past_key_value,
             use_cache=use_cache,
             is_self=True,
             is_causal_mask=is_causal_mask,
@@ -347,14 +345,27 @@
     nlayers=24,
     pad_id=-1,
     max_expected_seq_len=2048,
     p_dropout=0.1,
     emb_dropout=0.1,
 )
 
+_3b_config = GPTBigCodeConfig(
+    src_vocab_size=49152,
+    emb_dim=3072,
+    nheads=32,
+    nlayers=32,
+    pad_id=0,
+    max_expected_seq_len=2048,
+    hidden_grow_factor=4.0,
+    activation_fn="gelu",
+    multiquery_attn=True,
+    ln_eps=1e-5,
+)
+
 # https://www.ibm.com/docs/en/cloud-paks/cp-data/4.8.x?topic=models-granite-13b-instruct-v2-model-card
 _13b_config = GPTBigCodeConfig(
     src_vocab_size=50304,
     emb_dim=5632,
     nheads=44,
     nlayers=40,
     pad_id=50280,
@@ -389,82 +400,53 @@
     return factory
 
 
 models.register_model(
     _architecture_name, "santacoder", _gpt_bigcode_factory_factory(_santacoder_config)
 )
 models.register_model(
+    _architecture_name, "ibm.3b", _gpt_bigcode_factory_factory(_3b_config)
+)
+
+models.register_model(
     _architecture_name, "ibm.13b", _gpt_bigcode_factory_factory(_13b_config)
 )
 models.register_model(
     _architecture_name, "ibm.20b", _gpt_bigcode_factory_factory(_20b_config)
 )
 
+_convert_to_fused_qkv = serialization._legacy_attn_unfused_to_fused_adapter
+
 
 def _hf_sd_to_fms_sd(hf_sd: Mapping) -> Mapping:
     import re
 
     replacements = [
         ("lm_head.weight", "head.weight"),
         (r"^transformer.wte.weight", "base_model.embedding.weight"),
         (r"^transformer.wpe.weight", "base_model.position_embedding.weight"),
         (r"^transformer.ln_f", "base_model.dec_norm"),
         (r"^transformer.h", "base_model.layers"),
         # need to do kqv manually
+        (r"attn\.c_attn", "attn.in_proj.qkv_fused"),
         (r"attn\.c_proj", "attn.dense"),
         (r"mlp\.c_fc", "ff_sub_layer.w1"),
         (r"mlp\.c_proj", "ff_sub_layer.w2"),
         (r"ln_1", "ln"),
         (r"ln_2", "ff_ln"),
     ]
-    qkv_weight_pattern = re.compile("transformer.h.[0-9]+.attn.c_attn.weight")
-    qkv_bias_pattern = re.compile("transformer.h.[0-9]+.attn.c_attn.bias")
 
     new_sd = {}
     for name, param in hf_sd.items():
         new_name = name
         for pattern, repl in replacements:
             new_name = re.sub(pattern, repl, new_name)
 
         new_sd[new_name] = param
 
-        # qkv fused
-        if bool(qkv_weight_pattern.match(name)):
-            emb_dim = param.size(1)
-            num_heads = emb_dim // 128
-            num_key_value_heads = (param.size(0) // 128 - num_heads) // 2
-            attn_splits = [
-                (num_heads * 128) // num_key_value_heads,
-                (num_key_value_heads * 128) // num_key_value_heads,
-                (num_key_value_heads * 128) // num_key_value_heads,
-            ]
-
-            prefix = new_name.replace("c_attn.weight", "")
-            q, k, v = param.split(attn_splits, dim=0)
-
-            new_sd[f"{prefix}query.weight"] = q
-            new_sd[f"{prefix}key.weight"] = k
-            new_sd[f"{prefix}value.weight"] = v
-        elif bool(qkv_bias_pattern.match(name)):
-            weight_name = name.replace("bias", "weight")
-            new_sd.pop(new_name)
-
-            emb_dim = hf_sd[weight_name].size(1)
-            num_heads = emb_dim // 128
-            num_key_value_heads = (param.size(0) // 128 - num_heads) // 2
-            attn_splits = [
-                (num_heads * 128) // num_key_value_heads,
-                (num_key_value_heads * 128) // num_key_value_heads,
-                (num_key_value_heads * 128) // num_key_value_heads,
-            ]
-
-            prefix = new_name.replace("c_attn.bias", "")
-            q, k, v = param.split(attn_splits, dim=0)
-
-            new_sd[f"{prefix}query.bias"] = q
-            new_sd[f"{prefix}key.bias"] = k
-            new_sd[f"{prefix}value.bias"] = v
-
     return new_sd
 
 
 serialization.register_adapter(_architecture_name, "hf", _hf_sd_to_fms_sd)
+serialization.register_adapter(
+    _architecture_name, "fms.pre0.0.6", _convert_to_fused_qkv
+)
```

## fms/models/llama.py

```diff
@@ -46,14 +46,17 @@
     pad_id: int = -1
     hidden_grow_factor: float = 8 / 3
     multiple_of: int = 256
     activation_fn: str = "swish"
     p_dropout: float = 0.0
     max_expected_seq_len: int = 4096
     ntk_scaling: bool = False
+    attn_bias: bool = False
+    mlp_bias: bool = False
+    tie_heads: bool = False
 
 
 class LLaMABlock(nn.Module):
     def __init__(self, config: LLaMAConfig, rotary_emb: RotaryEmbedding):
         super(LLaMABlock, self).__init__()
         self.config = config
         emb_kq = self.config.emb_dim // self.config.nheads
@@ -85,24 +88,24 @@
         self.attn = MultiHeadAttention(
             self.config.emb_dim,
             emb_kq,
             emb_v,
             self.config.nheads,
             kvheads,
             p_dropout=self.config.p_dropout,
-            use_bias=False,
+            use_bias=self.config.attn_bias,
             position_encoder=rotary_emb,
         )
         self.ff_sub_layer = GatedLinearUnit(
             self.config.emb_dim,
             hidden_grow_factor=self.config.hidden_grow_factor,
             multiple_of=self.config.multiple_of,
             activation_fn=str_to_activation(self.config.activation_fn),
             p_dropout=self.config.p_dropout,
-            use_bias=False,
+            use_bias=self.config.mlp_bias,
         )
 
         if self.config.p_dropout != 0:
             self.dropout = nn.Dropout(self.config.p_dropout)
 
     def forward(
         self,
@@ -123,16 +126,14 @@
         #     self_attn_past_key_value = None
 
         # first we do MHA and Add&Norm
         residual = x
         x = self.ln(x)
         x = self.attn(
             q=x,
-            k=x,
-            v=x,
             mask=mask,
             position_ids=position_ids,
             attn_algorithm=attn_algorithm,
             past_key_value_state=self_attn_past_key_value,
             use_cache=use_cache,
             is_self=True,
             is_causal_mask=is_causal_mask,
@@ -181,15 +182,15 @@
 
         shared = WordEmbedding(
             self.config.src_vocab_size,
             self.config.emb_dim,
             padding_idx=self.config.pad_id,
             abs_pos=False,
             reversible=True,
-            tie_weights=False,
+            tie_weights=self.config.tie_heads,
             bias=False,
         )
         self.shared = self.distributed_strategy.distribute_module(shared)
 
         self.rot_emb = RotaryEmbedding(
             dim=self.config.emb_dim // self.config.nheads,
             ntk_scaling=self.config.ntk_scaling,
@@ -402,14 +403,19 @@
     _architecture_name, "micro", _llama_factory_factory(_micro_char_config)
 )
 models.register_model(_architecture_name, "7b", _llama_factory_factory(_7b_config))
 models.register_model(_architecture_name, "13b", _llama_factory_factory(_13b_config))
 models.register_model(_architecture_name, "70b", _llama_factory_factory(_70b_config))
 
 
+_convert_to_fused = lambda sd: serialization._legacy_mlp_glu_unfused_to_fused_adapter(
+    serialization._legacy_attn_unfused_to_fused_adapter(sd)
+)
+
+
 def _rename_weights_to_fms(orig_sd):
     replacements = [
         (r"^tok_embeddings", "shared.emb"),
         (r"^norm", "dec_norm"),
         (r"^output", "shared.head"),
         (r"^layers", "layers"),
         (r"\.attention\.", ".attn."),
@@ -426,15 +432,17 @@
     new_sd = {}
     for name, param in orig_sd.items():
         new_name = name
         for pattern, repl in replacements:
             new_name = re.sub(pattern, repl, new_name)
         new_sd[new_name] = param
 
-    return new_sd
+    fused_sd = _convert_to_fused(new_sd)
+
+    return fused_sd
 
 
 def _hf_sd_to_fms_sd(hf_sd: Mapping) -> Mapping:
     replacements = [
         (r"^lm_head.weight", "shared.head.weight"),
         (r"^model.embed_tokens.weight", "shared.emb.weight"),
         (r"^model.norm", "dec_norm"),
@@ -470,19 +478,22 @@
                 temp.view(nheads, 2, -1, temp.size(1))
                 .transpose(1, 2)
                 .reshape(*temp.size())
             )
 
             new_sd[new_name] = temp
 
-    return new_sd
+    fused_sd = _convert_to_fused(new_sd)
+
+    return fused_sd
 
 
 serialization.register_adapter("llama", "meta", _rename_weights_to_fms)
 serialization.register_adapter("llama", "hf", _hf_sd_to_fms_sd)
+serialization.register_adapter("llama", "fms.pre0.0.6", _convert_to_fused)
 
 
 def convert_hf_llama(hf_model: "LlamaForCausalLM") -> LLaMA:  # type: ignore
     """
     Convert a Llama huggingface model to an fms model
 
     Parameters
```

## fms/models/roberta.py

```diff
@@ -6,15 +6,15 @@
 import torch
 import torch.nn as nn
 
 from fms import models
 from fms.distributed.strategy import DistributedStrategy, NoOpStrategy
 from fms.modules.attention import MultiHeadAttention
 from fms.modules.feedforward import FeedForwardBlock
-from fms.modules.head import ClassificationHead
+from fms.modules.head import MLPClassificationHead
 from fms.utils import serialization
 from fms.utils.activation import str_to_activation
 from fms.utils.config import ModelConfig
 
 
 @dataclass
 class RoBERTaConfig(ModelConfig):
@@ -70,16 +70,14 @@
         attn_algorithm: Optional[str] = None,
     ):
         # first we do MHA
         residual = x
         # self attention
         x = self.attn(
             q=x,
-            k=x,
-            v=x,
             mask=mask,
             attn_algorithm=attn_algorithm,
             is_self=True,
             is_causal_mask=False,
         )
 
         if self.config.p_dropout != 0:
@@ -216,15 +214,15 @@
         self.config = self.config.updated(**kwargs)
         self.distributed_strategy = distributed_strategy
 
         self.base_model = RoBERTaHeadless(self.config, self.distributed_strategy)
 
         # The head does not get TP-Wrapped as in many cases the vocab_size will not be divisible by the world size
         self.classification_head = self.distributed_strategy.distribute_module(
-            ClassificationHead(
+            MLPClassificationHead(
                 self.config.emb_dim,
                 # number of classes is vocab size as this is predicting a masked token
                 num_classes=self.config.src_vocab_size,
                 activation_fn=str_to_activation(self.config.activation_fn),
                 layer_norm=nn.LayerNorm(self.config.emb_dim, self.config.norm_eps),
                 dropout=self.config.p_dropout,
             ),
@@ -292,14 +290,16 @@
 models.register_model(
     _architecture_name, "micro", _roberta_factory_factory(_micro_char_config)
 )
 models.register_model(
     _architecture_name, "base", _roberta_factory_factory(_base_config)
 )
 
+_convert_to_fused_qkv = serialization._legacy_attn_unfused_to_fused_adapter
+
 
 def _hf_sd_to_fms_sd(hf_sd: Mapping[Any, Any]) -> Mapping[Any, Any]:
     replacements = [
         (r"^roberta.embeddings.word_embeddings.weight", "base_model.embedding.weight"),
         (
             r"^roberta.embeddings.position_embeddings.weight",
             "base_model.position_embedding.weight",
@@ -325,11 +325,14 @@
             new_name = re.sub(pattern, repl, new_name)
         new_sd[new_name] = param
 
         # hf always has the first 2 spots set, we need to remove them as they are not used
         if name == "roberta.embeddings.position_embeddings.weight":
             new_sd[new_name] = new_sd[new_name][2:]
 
-    return new_sd
+    fused_sd = _convert_to_fused_qkv(new_sd)
+
+    return fused_sd
 
 
 serialization.register_adapter("roberta", "hf", _hf_sd_to_fms_sd)
+serialization.register_adapter("roberta", "fms.pre0.0.6", _convert_to_fused_qkv)
```

## fms/models/hf/__init__.py

```diff
@@ -1,45 +1,57 @@
 from fms.models.gpt_bigcode import GPTBigCode, GPTBigCodeHeadless
 from fms.models.hf.gpt_bigcode import HFAdaptedGPTBigCodeForCausalLM
 from fms.models.hf.gpt_bigcode.modeling_gpt_bigcode_hf import (
     HFAdaptedGPTBigCodeHeadless,
 )
 from fms.models.hf.llama import HFAdaptedLLaMAForCausalLM
 from fms.models.hf.llama.modeling_llama_hf import HFAdaptedLLaMAHeadless
+from fms.models.hf.mixtral.modeling_mixtral_hf import (
+    HFAdaptedMixtralForCausalLM,
+    HFAdaptedMixtralHeadless,
+)
 from fms.models.hf.roberta.modeling_roberta_hf import (
     HFAdaptedRoBERTaForMaskedLM,
     HFAdaptedRoBERTaHeadless,
 )
 from fms.models.hf.utils import register_fms_models, to_hf_api
 from fms.models.llama import LLaMA
+from fms.models.mixtral import Mixtral, MixtralHeadless
 from fms.models.roberta import RoBERTa, RoBERTaHeadless
 
 
 """
 mapping from an FMS model to its equivalent HF-Adapted model
 """
 _fms_to_hf_adapt_map = {
     LLaMA: HFAdaptedLLaMAForCausalLM,
     GPTBigCode: HFAdaptedGPTBigCodeForCausalLM,
     GPTBigCodeHeadless: HFAdaptedGPTBigCodeHeadless,
     RoBERTa: HFAdaptedRoBERTaForMaskedLM,
     RoBERTaHeadless: HFAdaptedRoBERTaHeadless,
+    Mixtral: HFAdaptedMixtralForCausalLM,
+    MixtralHeadless: HFAdaptedMixtralHeadless,
 }
 
 """
 list of all headless base HF-Adapted models used in registration 
 """
 _headless_models = [
     HFAdaptedGPTBigCodeHeadless,
     HFAdaptedLLaMAHeadless,
     HFAdaptedRoBERTaHeadless,
+    HFAdaptedMixtralHeadless,
 ]
 
 """
 list of all causal-lm HF-Adapted models used in registration 
 """
-_causal_lm_models = [HFAdaptedGPTBigCodeForCausalLM, HFAdaptedLLaMAForCausalLM]
+_causal_lm_models = [
+    HFAdaptedGPTBigCodeForCausalLM,
+    HFAdaptedLLaMAForCausalLM,
+    HFAdaptedMixtralForCausalLM,
+]
 
 """
 list of all masked-lm HF-Adapted models used in registration
 """
 _masked_lm_models = [HFAdaptedRoBERTaForMaskedLM]
```

## fms/models/hf/lm_head_mixins.py

```diff
@@ -10,15 +10,15 @@
     CausalLMOutputWithCrossAttentions,
     MaskedLMOutput,
     Seq2SeqLMOutput,
     SequenceClassifierOutput,
 )
 from transformers.utils import ModelOutput
 
-from fms.modules.head import ClassificationHead
+from fms.modules.head import MLPClassificationHead
 from fms.utils.activation import str_to_activation
 
 
 class LMHeadMixin:
     """
     Base class to represent enabled a model architecture to include the lm_head. An lm_head can either be given by the
     child class, or created by the LMHeadMixin. In either case, both lm_head should be the same type resulting in the
@@ -312,15 +312,15 @@
         )
 
     def _get_empty_lm_head(
         self,
         classifier_activation_fn: str,
         classifier_dropout: float,
     ) -> nn.Module:
-        return ClassificationHead(
+        return MLPClassificationHead(
             self.config.hidden_size,
             self.config.num_labels,
             str_to_activation(classifier_activation_fn),
             dropout=classifier_dropout,
             apply_pooling_fn=True,
         )
 
@@ -409,15 +409,15 @@
             **kwargs,
         )
 
     def get_output_embeddings(self):
         return self.lm_head.head
 
     def _get_empty_lm_head(self, activation_fn: str, norm_eps: float) -> nn.Module:
-        return ClassificationHead(
+        return MLPClassificationHead(
             self.config.hidden_size,
             self.config.vocab_size,
             activation_fn=str_to_activation(activation_fn),
             layer_norm=nn.LayerNorm(self.config.hidden_size, norm_eps),
         )
 
     def _compute_loss(self, prediction: torch.Tensor, labels: torch.Tensor) -> _Loss:
```

## fms/models/hf/gpt_bigcode/__init__.py

```diff
@@ -50,32 +50,18 @@
             fms_hf_model.decoder.model.position_embedding.weight
         )
         for i, oss_hf_layer in enumerate(oss_hf_model.transformer.h):
             fms_hf_layer = fms_hf_model.decoder.model.layers[i]
 
             # self attn
             oss_hf_layer.attn.c_attn.weight.copy_(
-                torch.cat(
-                    [
-                        fms_hf_layer.attn.query.weight.data,
-                        fms_hf_layer.attn.key.weight.data,
-                        fms_hf_layer.attn.value.weight.data,
-                    ],
-                    dim=0,
-                )
+                fms_hf_layer.attn.in_proj.qkv_fused.weight
             )
             oss_hf_layer.attn.c_attn.bias.copy_(
-                torch.cat(
-                    [
-                        fms_hf_layer.attn.query.bias.data,
-                        fms_hf_layer.attn.key.bias.data,
-                        fms_hf_layer.attn.value.bias.data,
-                    ],
-                    dim=0,
-                )
+                fms_hf_layer.attn.in_proj.qkv_fused.bias
             )
             oss_hf_layer.attn.c_proj.weight.copy_(fms_hf_layer.attn.dense.weight)
             oss_hf_layer.attn.c_proj.bias.copy_(fms_hf_layer.attn.dense.bias)
 
             # mlp
             oss_hf_layer.mlp.c_fc.weight.copy_(fms_hf_layer.ff_sub_layer.w1.weight)
             oss_hf_layer.mlp.c_fc.bias.copy_(fms_hf_layer.ff_sub_layer.w1.bias)
```

## fms/models/hf/roberta/modeling_roberta_hf.py

```diff
@@ -110,14 +110,17 @@
 
 
 class HFAdaptedRoBERTaHeadless(HFEncoderModelArchitecture):
     # attributes required by HF
     config_class = HFAdaptedRoBERTaConfig
     base_model_prefix = "hf_adapted_roberta"
 
+    _tied_weights_keys = ["encoder.model.embedding.weight", "embedding.weight"]
+    _keys_to_ignore_on_save = ["embedding.weight"]
+
     def __init__(
         self,
         config: PretrainedConfig,
         encoder: Optional[RoBERTaHeadless] = None,
         embedding: Optional[nn.Module] = None,
         *args,
         **kwargs,
```

## fms/modules/attention.py

```diff
@@ -1,8 +1,9 @@
-from typing import List, Optional, Tuple
+import abc
+from typing import Dict, List, Optional, Set, Tuple
 
 import torch
 import torch.distributed
 from torch import Tensor, nn
 from torch.distributed.distributed_c10d import ProcessGroup
 from torch.nn import functional as F
 
@@ -11,14 +12,181 @@
     copy_to_tensor_model_parallel_region,
     reduce_from_tensor_model_parallel_region,
 )
 from fms.modules.positions import PositionEncoder
 from fms.modules.tp import TPModule
 
 
+class QKV(nn.Module, metaclass=abc.ABCMeta):
+    """Simple module for applying qkv in attention"""
+
+    def __init__(
+        self,
+        emb_dim: int,
+        nheads: int,
+        kvheads: int,
+        emb_kq_per_head: int,
+        emb_v_per_head: int,
+        use_bias: bool,
+        *args,
+        **kwargs,
+    ):
+        super().__init__(*args, **kwargs)
+        self.emb_dim = emb_dim
+        self.nheads = nheads
+        self.kvheads = kvheads
+        self.emb_kq_per_head = emb_kq_per_head
+        self.emb_v_per_head = emb_v_per_head
+        self.use_bias = use_bias
+
+    @abc.abstractmethod
+    def forward(
+        self, q: torch.Tensor, k: Optional[torch.Tensor], v: Optional[torch.Tensor]
+    ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+        """applies query/key/value transformations on q, k, v inputs respectively and returns the resulting values
+
+        Args:
+            q: torch.Tensor
+                the query tensor
+            k: Optional[torch.Tensor]
+                the optional key tensor
+            v: Optional[torch.Tensor]
+                the optional value tensor
+
+        Returns:
+        Tuple[torch.Tensor, torch.Tensor, torch.Tensor]
+            the query, key, and value computed
+        """
+        pass
+
+    @abc.abstractmethod
+    def reset_parameters(self):
+        """resets the query, key, and value weights for training
+
+        Args:
+            gain: int
+                gain for std in norm (default is 1)
+        """
+        pass
+
+
+class UnfusedQKV(QKV):
+    """
+    Unfused Weights implementation of QKV
+    """
+
+    def __init__(
+        self,
+        emb_dim: int,
+        nheads: int,
+        kvheads: int,
+        emb_kq_per_head: int,
+        emb_v_per_head: int,
+        use_bias: bool,
+        *args,
+        **kwargs,
+    ):
+        super().__init__(
+            emb_dim,
+            nheads,
+            kvheads,
+            emb_kq_per_head,
+            emb_v_per_head,
+            use_bias,
+            *args,
+            **kwargs,
+        )
+        self.query = nn.Linear(
+            self.emb_dim, self.nheads * self.emb_kq_per_head, bias=use_bias
+        )
+        self.key = nn.Linear(
+            self.emb_dim, self.kvheads * self.emb_kq_per_head, bias=use_bias
+        )
+        self.value = nn.Linear(
+            self.emb_dim, self.kvheads * self.emb_v_per_head, bias=use_bias
+        )
+
+    def reset_parameters(self):
+        for m in self.modules():
+            if isinstance(m, nn.Linear):
+                nn.init.trunc_normal_(m.weight, mean=0.0, std=0.02)
+                if self.use_bias:
+                    m.bias.data.zero_()
+
+    def forward(
+        self, q: torch.Tensor, k: Optional[torch.Tensor], v: Optional[torch.Tensor]
+    ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+        if k is None and v is None:
+            k = q
+            v = q
+        elif k is None or v is None:
+            raise ValueError(
+                "both k and v must either be given as tensors or both None"
+            )
+
+        # b x h x qlen x ds
+        queries = self.query(q)
+        keys = self.key(k)
+        values = self.value(v)
+        return queries, keys, values
+
+
+class FusedQKV(QKV):
+    """
+    Fused Weights implementation of QKV
+    """
+
+    def __init__(
+        self,
+        emb_dim: int,
+        nheads: int,
+        kvheads: int,
+        emb_kq_per_head: int,
+        emb_v_per_head: int,
+        use_bias: bool,
+        *args,
+        **kwargs,
+    ):
+        super().__init__(
+            emb_dim,
+            nheads,
+            kvheads,
+            emb_kq_per_head,
+            emb_v_per_head,
+            use_bias,
+            *args,
+            **kwargs,
+        )
+        self.splits = [
+            self.nheads * self.emb_kq_per_head,
+            self.kvheads * self.emb_kq_per_head,
+            self.kvheads * self.emb_v_per_head,
+        ]
+
+        self.qkv_fused = nn.Linear(
+            self.emb_dim,
+            sum(self.splits),
+            bias=self.use_bias,
+        )
+
+    def reset_parameters(self):
+        nn.init.trunc_normal_(self.qkv_fused.weight, mean=0.0, std=0.02)
+        if self.use_bias:
+            self.qkv_fused.bias.data.zero_()
+
+    def forward(
+        self, q: torch.Tensor, k: Optional[torch.Tensor], v: Optional[torch.Tensor]
+    ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+        if (k is None and v is None) or (k is q and v is q):
+            qkv = q
+        else:
+            raise ValueError("q, k, and v must be the same or k and v must be None")
+        return self.qkv_fused(qkv).split(self.splits, dim=-1)
+
+
 class MultiHeadAttention(nn.Module):
     """
     Performs multi-headed self- or cross-attention, with optional attention masking.
     ...
     Args
     ----
     emb_dim : int
@@ -29,47 +197,49 @@
         Latent dimensionality of each head in value projection (mixing dimension).
     nheads : int
         Number of attention heads.
     p_dropout : float|None
         Dropout probability. Must be in range [0,1]. If 0 or None, dropout will not be used.
     use_bias : bool
         Include bias terms in fully-connected sublayers?
-    factorable_emb: Optional[Callable]
-        Function that computes factorable embeddings (like RoPE). It is mutually exclusive with
-        additive biases on forward() passed as rel_pos_bias
+    fused: bool
+        if True, qkv weights will be fused, otherwise qkv weights will be unfused
     """
 
     def __init__(
         self,
         emb_dim,
         emb_kq,
         emb_v,
         nheads,
         kvheads,
         p_dropout=None,
         use_bias=False,
         position_encoder: Optional[PositionEncoder] = None,
+        fused: bool = True,
     ):
         super(MultiHeadAttention, self).__init__()
         self.nheads = nheads
         self.kvheads = kvheads
         self.emb_dim = emb_dim
         self.emb_kq_per_head = emb_kq
         self.emb_v_per_head = emb_v
         self.p_dropout = p_dropout if p_dropout is not None else 0.0
         self.use_bias = use_bias
-        self.query = nn.Linear(
-            self.emb_dim, self.nheads * self.emb_kq_per_head, bias=use_bias
-        )
-        self.key = nn.Linear(
-            self.emb_dim, self.kvheads * self.emb_kq_per_head, bias=use_bias
-        )
-        self.value = nn.Linear(
-            self.emb_dim, self.kvheads * self.emb_v_per_head, bias=use_bias
+        self.fused = fused
+
+        self.in_proj: QKV = (FusedQKV if self.fused else UnfusedQKV)(
+            self.emb_dim,
+            self.nheads,
+            self.kvheads,
+            self.emb_kq_per_head,
+            self.emb_v_per_head,
+            self.use_bias,
         )
+
         self.dense = nn.Linear(
             self.nheads * self.emb_v_per_head, self.emb_dim, bias=use_bias
         )
         if self.p_dropout:
             self.attn_dropout = nn.Dropout(self.p_dropout)
         self.position_encoder = position_encoder
         # Avoiding graph breaks
@@ -81,20 +251,25 @@
 
     def reset_parameters(self):
         for m in self.modules():
             if isinstance(m, nn.Linear):
                 nn.init.trunc_normal_(m.weight, mean=0.0, std=0.02)
                 if self.use_bias:
                     m.bias.data.zero_()
+            elif isinstance(m, QKV):
+                m.reset_parameters()
+
+    def to_tp(self, group: ProcessGroup) -> "TPMultiHeadAttention":
+        return TPMultiHeadAttention.import_module(self, group)
 
     def forward(
         self,
-        q,
-        k,
-        v,
+        q: torch.Tensor,
+        k: Optional[torch.Tensor] = None,
+        v: Optional[torch.Tensor] = None,
         mask: Optional[Tensor] = None,
         position_ids=None,
         attn_algorithm=None,
         past_key_value_state: Optional[Tuple[Tensor, Tensor]] = None,
         use_cache=False,
         is_self=True,
         is_causal_mask=False,
@@ -113,54 +288,50 @@
         Returns
         -------
         tensor or tuple
             If use_cache=False, only the hidden state will be returned as a tensor. If use_cache=True, a tuple will be
             returned in the form (hidden_state, cache) where hidden_state is a tensor and cache is of the form specified
             in past_key_value_state
         """
-
         # q, k, v: batch_size x seq_len x emb_dim
         # mask: batch_size x seq_len x seq_len
         batch_size, q_len, _ = q.size()
-        kv_len = k.size(1)
-
-        # split emb_dim as nheads*emb_dim_per_head
-        # b x h x qlen x ds
-        queries = self.query(q).view(
-            batch_size, q_len, self.nheads, self.emb_kq_per_head
-        )
 
         # if this is self attention, we always recompute
         # cross attention only gets computed when a cache does not exist
         # if we dont have the cache yet, we need to compute
         # d x (h x ds)
         # b x kvlen x d
         # b x kvlen x h x ds
         # b x h x kvlen x ds
+        # todo: Cross attention (This always is true for now)
         if is_self or past_key_value_state is None:
-            keys = self.key(k).view(
-                batch_size, kv_len, self.kvheads, self.emb_kq_per_head
-            )
+            q_out, k_out, v_out = self.in_proj(q, k, v)
 
-            values = self.value(v).view(
-                batch_size, kv_len, self.kvheads, self.emb_v_per_head
-            )
+            # note: transposes will be moved in a later PR to fix dis-contiguous tensor issues
+            queries = q_out.view(batch_size, q_len, self.nheads, self.emb_kq_per_head)
+            keys = k_out.view(batch_size, q_len, self.kvheads, self.emb_kq_per_head)
+            values = v_out.view(batch_size, q_len, self.kvheads, self.emb_v_per_head)
 
             # You want to apply rotary embeddings pre-cache
             if self.position_encoder is not None:
                 queries, keys = self.position_encoder.adjusted_qk(
                     queries, keys, position_ids, past_key_value_state, use_cache
                 )
 
         queries = queries.transpose(2, 1)  # / (self.emb_kq_per_head**(1/4))
         keys = keys.transpose(2, 1)  # / (self.emb_kq_per_head**(1/4))
         values = values.transpose(2, 1)  # compatible with QK.T
 
         # if you want to use caching and past_key_value_state is not None meaning you have values in your cache
-        if use_cache and past_key_value_state is not None:
+        if (
+            use_cache
+            and past_key_value_state is not None
+            and past_key_value_state[0].numel() > 0
+        ):
             if is_self:
                 keys = torch.cat((past_key_value_state[0], keys), dim=2)
                 values = torch.cat((past_key_value_state[1], values), dim=2)
             else:
                 keys = past_key_value_state[0]
                 values = past_key_value_state[1]
 
@@ -253,45 +424,146 @@
         emb_kq,
         emb_v,
         nheads,
         kvheads,
         p_dropout=None,
         use_bias=False,
         position_encoder: Optional[PositionEncoder] = None,
+        fused: bool = True,
         group: Optional[ProcessGroup] = None,
     ):
         assert torch.distributed.is_initialized()
 
         rank, world_size = distributed.rank_and_world(group)
         assert (
             nheads % world_size == 0
         ), "The number of heads must be divisible by world size"
+        assert (kvheads >= world_size and kvheads % world_size == 0) or (
+            kvheads < world_size and world_size % kvheads == 0
+        ), "the kv heads must be divisible by the world size or the world size must be divisible by kv heads"
         MultiHeadAttention.__init__(
             self,
             emb_dim,
             emb_kq,
             emb_v,
             nheads // world_size,
-            (kvheads // world_size) if kvheads > 1 else kvheads,
+            (kvheads // world_size) if kvheads >= world_size else 1,
             p_dropout,
             use_bias,
             position_encoder,
+            fused,
         )
+        self.pre_tp_nheads = nheads
         self.pre_tp_kvheads = kvheads
         self.setup_tp(rank, world_size)
 
-    def colwise_param_names(self) -> List[str]:
-        colwise_weights = ["query"]
-        if self.pre_tp_kvheads != 1:
-            colwise_weights.append("key")
-            colwise_weights.append("value")
-        return colwise_weights
+    def load_weights(
+        self,
+        tensor_values: Dict[str, torch.Tensor],
+    ):
+        used_keys: Set[str] = set()
+        dense_weight = self._get_sd_weight(
+            tensor_values, used_keys, ["dense", "weight"]
+        )
+        if self.use_bias:
+            dense_bias = self._get_sd_weight(
+                tensor_values, used_keys, ["dense", "bias"]
+            )
 
-    def rowwise_param_names(self) -> List[str]:
-        return ["dense"]
+        # 1. Grab the weights from tensor_values
+        if self.fused:
+            qkv_weight = self._get_sd_weight(
+                tensor_values, used_keys, ["qkv_fused", "weight"]
+            )
+            if self.use_bias:
+                qkv_bias = self._get_sd_weight(
+                    tensor_values, used_keys, ["qkv_fused", "bias"]
+                )
+
+            # 2. Raise exceptions
+            if len(tensor_values) > (4 if self.use_bias else 2):
+                unused_keys = set(tensor_values.keys()).difference(used_keys)
+                raise AttributeError(f"Unused weight(s): {', '.join(unused_keys)}")
+
+            # 3. Load and shard the weights
+            # The number in max_partition_sizes will signify the largest world size
+            # til we need to duplicate.  For instance if we have nheads=16 and
+            # world_size=32, then first 2 ranks will get first 1/16th of query
+            self.sharded_copy(
+                self.in_proj.qkv_fused.weight,
+                qkv_weight,
+                0,
+                [self.pre_tp_nheads, self.pre_tp_kvheads, self.pre_tp_kvheads],
+            )
+            self.sharded_copy(self.dense.weight, dense_weight, 1, [self.world_size])
+            if self.use_bias:
+                self.sharded_copy(
+                    self.in_proj.qkv_fused.bias,
+                    qkv_bias,
+                    0,
+                    [self.pre_tp_nheads, self.pre_tp_kvheads, self.pre_tp_kvheads],
+                )
+                self.sharded_copy(
+                    self.dense.bias, dense_bias, 1, [self.world_size], False
+                )
+
+        else:
+            query_weight = self._get_sd_weight(
+                tensor_values, used_keys, ["query", "weight"]
+            )
+            key_weight = self._get_sd_weight(
+                tensor_values, used_keys, ["key", "weight"]
+            )
+            value_weight = self._get_sd_weight(
+                tensor_values, used_keys, ["value", "weight"]
+            )
+
+            if self.use_bias:
+                query_bias = self._get_sd_weight(
+                    tensor_values, used_keys, ["query", "bias"]
+                )
+                key_bias = self._get_sd_weight(
+                    tensor_values, used_keys, ["key", "bias"]
+                )
+                value_bias = self._get_sd_weight(
+                    tensor_values, used_keys, ["value", "bias"]
+                )
+
+            # 2. Raise exceptions
+            if len(tensor_values) > (8 if self.use_bias else 4):
+                unused_keys = set(tensor_values.keys()).difference(used_keys)
+                raise AttributeError(f"Unused weight(s): {', '.join(unused_keys)}")
+
+            # 3. Load and shard the weights
+            # The number in max_partition_sizes will signify the largest world size
+            # til we need to duplicate.  For instance if we have nheads=16 and
+            # world_size=32, then first 2 ranks will get first 1/16th of query
+            self.sharded_copy(
+                self.in_proj.query.weight, query_weight, 0, [self.pre_tp_nheads]
+            )
+            self.sharded_copy(
+                self.in_proj.key.weight, key_weight, 0, [self.pre_tp_kvheads]
+            )
+            self.sharded_copy(
+                self.in_proj.value.weight, value_weight, 0, [self.pre_tp_kvheads]
+            )
+            self.sharded_copy(self.dense.weight, dense_weight, 1, [self.world_size])
+            if self.use_bias:
+                self.sharded_copy(
+                    self.in_proj.query.bias, query_bias, 0, [self.pre_tp_nheads]
+                )
+                self.sharded_copy(
+                    self.in_proj.key.bias, key_bias, 0, [self.pre_tp_kvheads]
+                )
+                self.sharded_copy(
+                    self.in_proj.value.bias, value_bias, 0, [self.pre_tp_kvheads]
+                )
+                self.sharded_copy(
+                    self.dense.bias, dense_bias, 1, [self.world_size], False
+                )
 
     @staticmethod
     def import_module(
         mha: MultiHeadAttention, group: ProcessGroup
     ) -> "TPMultiHeadAttention":
         tp_mha = TPMultiHeadAttention(
             emb_dim=mha.emb_dim,
@@ -299,38 +571,57 @@
             emb_v=mha.emb_v_per_head,
             nheads=mha.nheads,
             kvheads=mha.kvheads,
             p_dropout=mha.p_dropout,
             use_bias=mha.use_bias,
             position_encoder=mha.position_encoder,
             group=group,
+            fused=mha.fused,
         )
         return tp_mha
 
+    def _copy_to_tp_region(
+        self,
+        q: torch.Tensor,
+        k: Optional[torch.Tensor] = None,
+        v: Optional[torch.Tensor] = None,
+    ):
+        if (k is None and v is None) or (k is q and v is q):
+            q_par = copy_to_tensor_model_parallel_region(q)
+            if self.fused:
+                k_par = None
+                v_par = None
+            else:
+                k_par = copy_to_tensor_model_parallel_region(k)
+                v_par = copy_to_tensor_model_parallel_region(v)
+        else:
+            raise ValueError(
+                "both k and v must either be given as tensors or both None"
+            )
+
+        return q_par, k_par, v_par
+
     def forward(
         self,
         q,
-        k,
-        v,
+        k=None,
+        v=None,
         mask=None,
         position_ids=None,
         attn_algorithm=None,
         past_key_value_state=None,
         use_cache=False,
         is_self=True,
         is_causal_mask=False,
     ):
         """
         Check MultiHeadAttention for up-to-date arguments and docs
         """
 
-        q_par = copy_to_tensor_model_parallel_region(q)
-        k_par = copy_to_tensor_model_parallel_region(k)
-        v_par = copy_to_tensor_model_parallel_region(v)
-        # rel_pos_bias_par = copy_to_tensor_model_parallel_region(rel_pos_bias)
+        q_par, k_par, v_par = self._copy_to_tp_region(q, k, v)
 
         out_par = MultiHeadAttention.forward(
             self,
             q_par,
             k_par,
             v_par,
             mask,
```

## fms/modules/embedding.py

```diff
@@ -1,21 +1,19 @@
 import math
-from typing import List, Optional, Tuple, Union
+from typing import Dict, List, Optional, Set, Tuple, Union
 
 import torch
 import torch.distributed
 import torch.nn as nn
 from numpy import sign
 from torch.distributed.distributed_c10d import ProcessGroup
 
 from fms import distributed
 from fms.distributed.tensorparallel import (
     all_gather_from_tensor_model_parallel_region,
-    apply_colwise_tp,
-    apply_embedding_tp,
     copy_to_tensor_model_parallel_region,
 )
 from fms.modules.tp import TPModule
 
 
 class WordEmbedding(nn.Module):
     """
@@ -95,14 +93,17 @@
             nn.init.trunc_normal_(getattr(self, layer).weight, mean=0.0, std=0.02)
         if self.reversible and self.bias:
             self.head.bias.data.zero_()
         # Preserve pad index dummy-hood
         if self.padding_idx is not None:
             self.emb.weight.data[self.padding_idx].zero_()
 
+    def to_tp(self, group: ProcessGroup) -> "TPWordEmbedding":
+        return TPWordEmbedding.import_module(self, group)
+
     def forward(self, inp, reverse=False):
         # If reverse is False, compute input embeddings. If reverse is True, compute output logits.
         # vocab_idx: b n d if reverse, else b n
         if not reverse:
             if self.debug:
                 assert (
                     inp.min().item() >= 0
@@ -211,27 +212,129 @@
             tie_weights=we.tie_weights,
             bias=we.bias,
             debug=we.debug,
             group=group,
         )
         return tp_we
 
-    def colwise_param_names(self) -> List[str]:
+    def load_weights(
+        self,
+        tensor_values: Dict[str, torch.Tensor],
+    ):
+        # 1. Grab the weights from tensor_values
+        used_keys: Set[str] = set()
+        weight_count = 1
+        emb_weight = self._get_sd_weight(tensor_values, used_keys, ["emb"])
+        if self.abs_pos:
+            pos_emb_weight = self._get_sd_weight(tensor_values, used_keys, ["pos_emb"])
+            weight_count += 1
         if self.reversible and not self.tie_weights:
-            return ["head"]
-        return []
+            head_weight = self._get_sd_weight(
+                tensor_values, used_keys, ["head", "weight"]
+            )
+            weight_count += 1
+            if self.bias:
+                head_bias = self._get_sd_weight(
+                    tensor_values, used_keys, ["head", "bias"]
+                )
+                weight_count += 1
+
+        # 2. Raise exceptions
+        if len(tensor_values) > weight_count:
+            unused_keys = set(tensor_values.keys()).difference(used_keys)
+            raise AttributeError(f"Unused weight(s): {', '.join(unused_keys)}")
 
-    def embedding_param_names(self) -> List[str]:
-        emb_weights = ["emb"]
+        # 3. Load and shard the weights
+        self.sharded_copy(self.emb.weight, emb_weight, 1, [self.world_size])
         if self.abs_pos:
-            emb_weights.append("pos_emb")
-        return emb_weights
+            self.sharded_copy(self.pos_emb.weight, pos_emb_weight, 1, [self.world_size])
+        if self.reversible and not self.tie_weights:
+            self.sharded_copy(self.head.weight, head_weight, 0, [self.world_size])
+            if self.bias:
+                self.sharded_copy(self.head.bias, head_bias, 0, [self.world_size])
 
     def forward(self, inp, reverse=False):
         # If reverse is False, compute input embeddings. If reverse is True, compute output logits.
         # vocab_idx: b n d if reverse, else b n
         inp_par = copy_to_tensor_model_parallel_region(inp)
         out_par = WordEmbedding.forward(self, inp_par, reverse=reverse)
         # with ints this wasn't `torch.compile`ing
         rank = torch.tensor(self.rank)
         world_size = torch.tensor(self.world_size)
         return all_gather_from_tensor_model_parallel_region(out_par, rank, world_size)
+
+
+class TPEmbedding(nn.Embedding, TPModule):
+    """
+    Input embedding layer for sequence models. Not to be confused with TPWordEmbedding.
+    (TP)WordEmbedding supports fusing together the LM Head and the input Embedding, while
+    this is a class for when you want them separate, like in headless models.
+
+    Args
+    ----
+    Check nn.Embedding for up-to-date docs
+
+    world_size: int
+        the number of processes running this model in TP
+    rank: int
+        the index of this process wrt to the rest running the model in TP
+    """
+
+    def __init__(
+        self,
+        num_embeddings: int,
+        embedding_dim: int,
+        *,
+        group: Optional[ProcessGroup] = None,
+        **kwargs,
+    ):
+        assert torch.distributed.is_initialized()
+        rank, world_size = distributed.rank_and_world(group)
+        assert (
+            embedding_dim % world_size == 0
+        ), "The embedding dimensions must be divisible by world size"
+        nn.Embedding.__init__(
+            self, num_embeddings, embedding_dim // world_size, **kwargs
+        )
+        self.setup_tp(rank, world_size)
+
+    @staticmethod
+    def import_module(e: nn.Embedding, group: ProcessGroup) -> "TPEmbedding":
+        tp_e = TPEmbedding(
+            num_embeddings=e.num_embeddings,
+            embedding_dim=e.embedding_dim,
+            padding_idx=e.padding_idx,
+            max_norm=e.max_norm,
+            norm_type=e.norm_type,
+            scale_grad_by_freq=e.scale_grad_by_freq,
+            sparse=e.sparse,
+            _freeze=not e.weight.requires_grad,
+            device=e.weight.device,
+            dtype=e.weight.dtype,
+            group=group,
+        )
+        return tp_e
+
+    def load_weights(
+        self,
+        tensor_values: Dict[str, torch.Tensor],
+    ):
+        # 1. Grab the weights from tensor_values
+        used_keys: Set[str] = set()
+        emb_weight = self._get_sd_weight(tensor_values, used_keys, ["weight"])
+
+        # 2. Raise exceptions
+        if len(tensor_values) > 1:
+            unused_keys = set(tensor_values.keys()).difference(used_keys)
+            raise AttributeError(f"Unused weight(s): {', '.join(unused_keys)}")
+
+        # 3. Load and shard the weights
+        self.sharded_copy(self.weight, emb_weight, 1, [self.world_size])
+
+    def forward(self, inp: torch.Tensor):
+        # vocab_idx: b n d if reverse, else b n
+        inp_par = copy_to_tensor_model_parallel_region(inp)
+        out_par = nn.Embedding.forward(self, inp_par)
+        # with ints this wasn't `torch.compile`ing
+        rank = torch.tensor(self.rank)
+        world_size = torch.tensor(self.world_size)
+        return all_gather_from_tensor_model_parallel_region(out_par, rank, world_size)
```

## fms/modules/feedforward.py

```diff
@@ -1,14 +1,16 @@
-from typing import List, Optional
+from typing import Dict, Optional, Set
 
 import torch
 import torch.distributed
 import torch.nn as nn
+import torch.nn.functional as F
 from torch.distributed.distributed_c10d import ProcessGroup
 
+import fms.triton.moe_kernel as moe_kernel  # registers the PT custom ops
 from fms import distributed
 from fms.distributed.tensorparallel import (
     copy_to_tensor_model_parallel_region,
     reduce_from_tensor_model_parallel_region,
 )
 from fms.modules.tp import TPModule
 
@@ -63,14 +65,17 @@
                 getattr(self, layer).weight,
                 mean=0.0,
                 std=0.02,
             )
             if self.use_bias:
                 getattr(self, layer).bias.data.zero_()
 
+    def to_tp(self, group: ProcessGroup) -> "TPFeedForwardBlock":
+        return TPFeedForwardBlock.import_module(self, group)
+
     def forward(self, x):
         out = self.a(self.w1(x))
         if self.p_dropout:
             out = self.d(out)
         out = self.w2(out)
         return out
 
@@ -114,19 +119,37 @@
             multiple_of,
             activation_fn,
             p_dropout,
             use_bias,
         )
         self.setup_tp(rank, world_size)
 
-    def colwise_param_names(self) -> List[str]:
-        return ["w1"]
-
-    def rowwise_param_names(self) -> List[str]:
-        return ["w2"]
+    def load_weights(
+        self,
+        tensor_values: Dict[str, torch.Tensor],
+    ):
+        # 1. Grab the weights from tensor_values
+        used_keys: Set[str] = set()
+        w1_weight = self._get_sd_weight(tensor_values, used_keys, ["w1", "weight"])
+        w2_weight = self._get_sd_weight(tensor_values, used_keys, ["w2", "weight"])
+        if self.use_bias:
+            w1_bias = self._get_sd_weight(tensor_values, used_keys, ["w1", "bias"])
+            w2_bias = self._get_sd_weight(tensor_values, used_keys, ["w2", "bias"])
+
+        # 2. Raise exceptions for extra weights in tensor_values
+        if len(tensor_values) > (4 if self.use_bias else 2):
+            unused_keys = set(tensor_values.keys()).difference(used_keys)
+            raise AttributeError(f"Unused weight(s): {', '.join(unused_keys)}")
+
+        # 3. Load and shard the weights
+        self.sharded_copy(self.w1.weight, w1_weight, 0, [self.world_size])
+        self.sharded_copy(self.w2.weight, w2_weight, 1, [self.world_size])
+        if self.use_bias:
+            self.sharded_copy(self.w1.bias, w1_bias, 0, [self.world_size])
+            self.sharded_copy(self.w2.bias, w2_bias, 1, [self.world_size], False)
 
     @staticmethod
     def import_module(
         ffb: FeedForwardBlock, group: ProcessGroup
     ) -> "TPFeedForwardBlock":
         tp_ffb = TPFeedForwardBlock(
             emb_dim=ffb.w1.in_features,
@@ -178,37 +201,41 @@
     ):
         super(GatedLinearUnit, self).__init__()
         self.hidden_dim = int(hidden_grow_factor * emb_dim)
         if multiple_of:
             self.hidden_dim = multiple_of * (
                 (self.hidden_dim + multiple_of - 1) // multiple_of
             )
-        self.w1 = nn.Linear(emb_dim, self.hidden_dim, bias=use_bias)
-        self.wg = nn.Linear(emb_dim, self.hidden_dim, bias=use_bias)
+        self.wg1_fused = nn.Linear(emb_dim, 2 * self.hidden_dim, bias=use_bias)
         self.a = activation_fn
         self.p_dropout = p_dropout
         if p_dropout:
             self.d = nn.Dropout(p_dropout)
         self.w2 = nn.Linear(self.hidden_dim, emb_dim, bias=use_bias)
         self.use_bias = use_bias
         self.width = emb_dim
         self.grow_factor = hidden_grow_factor
 
     def reset_parameters(self):
-        for layer in ["w1", "w2", "wg"]:
+        for layer in ["wg1_fused", "w2"]:
             nn.init.trunc_normal_(
                 getattr(self, layer).weight,
                 mean=0.0,
                 std=0.02,
             )
             if self.use_bias:
                 getattr(self, layer).bias.data.zero_()
 
+    def to_tp(self, group: ProcessGroup) -> "TPGatedLinearUnit":
+        return TPGatedLinearUnit.import_module(self, group)
+
     def forward(self, x):
-        out = self.a(self.wg(x)) * self.w1(x)
+        out_fused = self.wg1_fused(x)
+        wg, w1 = torch.split(out_fused, [self.hidden_dim, self.hidden_dim], dim=2)
+        out = self.a(wg) * w1
         if self.p_dropout:
             out = self.d(out)
         return self.w2(out)
 
 
 class TPGatedLinearUnit(GatedLinearUnit, TPModule):
     """
@@ -252,19 +279,45 @@
             multiple_of,
             activation_fn,
             p_dropout,
             use_bias,
         )
         self.setup_tp(rank, world_size)
 
-    def colwise_param_names(self) -> List[str]:
-        return ["w1", "wg"]
+    def load_weights(
+        self,
+        tensor_values: Dict[str, torch.Tensor],
+    ):
+        # 1. Grab the weights from tensor_values
+        used_keys: Set[str] = set()
+        wg_weight = self._get_sd_weight(
+            tensor_values, used_keys, ["wg1_fused", "weight"]
+        )
+        w2_weight = self._get_sd_weight(tensor_values, used_keys, ["w2", "weight"])
+        if self.use_bias:
+            wg_bias = self._get_sd_weight(
+                tensor_values, used_keys, ["wg1_fused", "bias"]
+            )
+            w2_bias = self._get_sd_weight(tensor_values, used_keys, ["w2", "bias"])
 
-    def rowwise_param_names(self) -> List[str]:
-        return ["w2"]
+        # 2. Raise exceptions
+        if len(tensor_values) > (4 if self.use_bias else 2):
+            unused_keys = set(tensor_values.keys()).difference(used_keys)
+            raise AttributeError(f"Unused weight(s): {', '.join(unused_keys)}")
+
+        # 3. Load and shard the weights
+        self.sharded_copy(
+            self.wg1_fused.weight, wg_weight, 0, [self.world_size, self.world_size]
+        )
+        self.sharded_copy(self.w2.weight, w2_weight, 1, [self.world_size])
+        if self.use_bias:
+            self.sharded_copy(
+                self.wg1_fused.bias, wg_bias, 0, [self.world_size, self.world_size]
+            )
+            self.sharded_copy(self.w2.bias, w2_bias, 1, [self.world_size], False)
 
     @staticmethod
     def import_module(glu: GatedLinearUnit, group: ProcessGroup) -> "TPGatedLinearUnit":
         tp_glu = TPGatedLinearUnit(
             emb_dim=glu.width,
             hidden_grow_factor=glu.hidden_dim / glu.width,
             multiple_of=None,
@@ -276,7 +329,226 @@
 
         return tp_glu
 
     def forward(self, x):
         x_par = copy_to_tensor_model_parallel_region(x)
         out_par = GatedLinearUnit.forward(self, x_par)
         return reduce_from_tensor_model_parallel_region(out_par)
+
+
+class ConditionalFeedForward(nn.Module):
+    """
+    This class represents the expert feed forward networks of an MoE FF layer.
+
+    For more information, see the review paper in https://arxiv.org/pdf/2209.01667.pdf
+
+    Args
+    ----
+    num_experts : int
+        The number of expert feed forward networks.
+    dim : int
+        The embedding dimension for the transformer model.
+    intermediate_size : int
+        The intermediate size for the expert networks.
+    """
+
+    def __init__(self, num_experts: int, dim: int, intermediate_size: int):
+        super().__init__()
+        self.num_experts = num_experts
+        self.dim = dim
+        self.intermediate_size = intermediate_size
+        self.w13 = nn.Parameter(torch.empty(num_experts, 2 * intermediate_size, dim))
+        self.w2 = nn.Parameter(torch.empty(num_experts, dim, intermediate_size))
+
+    def reset_parameters(self):
+        for param in ["w13", "w2"]:
+            nn.init.trunc_normal_(
+                getattr(self, param),
+                mean=0.0,
+                std=0.02,
+            )
+
+    def to_tp(self, group: ProcessGroup) -> "TPConditionalFeedForward":
+        return TPConditionalFeedForward.import_module(self, group)
+
+    def forward(self, x: torch.Tensor, expert_indices: torch.Tensor) -> torch.Tensor:
+        # Check constraints.
+        assert x.shape[1] == self.w13.shape[2], "Hidden size mismatch"
+        assert x.is_contiguous(), "Hidden_states must be contiguous"
+        assert self.w13.is_contiguous(), "Expert weights 1 must be contiguous"
+        assert self.w2.is_contiguous(), "Expert weights 2 must be contiguous"
+
+        M, D = x.shape
+        E, N, _ = self.w13.shape
+        _, A = expert_indices.shape
+
+        #  if x.device.type == "cuda":
+        ## Triton path
+
+        if expert_indices.numel() <= E:
+            padding_size = 16
+        else:
+            padding_size = 64
+
+        (
+            padded_token_ids_per_block,
+            expert_block_mapping,
+            total_padded_tokens,
+        ) = moe_kernel.moe_align_block_size(expert_indices, padding_size, E)
+
+        x1, x3 = (
+            torch.ops.moe.moe_mm(
+                x,
+                self.w13,
+                expert_indices,
+                padded_token_ids_per_block,
+                expert_block_mapping,
+                total_padded_tokens,
+                expert_indices.shape[1],
+                padding_size,
+            )
+            .view(-1, N)
+            .chunk(2, dim=1)
+        )
+        return torch.ops.moe.moe_mm(
+            F.silu(x1) * x3,
+            self.w2,
+            expert_indices,
+            padded_token_ids_per_block,
+            expert_block_mapping,
+            total_padded_tokens,
+            1,
+            padding_size,
+        )
+
+
+class TPConditionalFeedForward(ConditionalFeedForward, TPModule):
+    """
+    This class represents the expert feed forward networks of an MoE FF layer.
+    This subclass adds TP support.
+
+    Args
+    ----
+    num_experts : int
+        The number of expert feed forward networks.
+    dim : int
+        The embedding dimension for the transformer model.
+    intermediate_size : int
+        The intermediate size for the expert networks.
+    """
+
+    def __init__(
+        self,
+        num_experts: int,
+        dim: int,
+        intermediate_size: int,
+        group: Optional[ProcessGroup] = None,
+    ):
+        assert torch.distributed.is_initialized()
+        rank, world_size = distributed.rank_and_world(group)
+
+        assert (
+            intermediate_size % world_size == 0
+        ), "Intermediate size must be divisible by world size"
+        ConditionalFeedForward.__init__(
+            self,
+            num_experts,
+            dim,
+            intermediate_size // world_size,
+        )
+        self.setup_tp(rank, world_size)
+
+    def load_weights(
+        self,
+        tensor_values: Dict[str, torch.Tensor],
+    ):
+        # 1. Grab the weights from tensor_values
+        used_keys: Set[str] = set()
+        w13_weight = self._get_sd_weight(tensor_values, used_keys, ["w13"])
+        w2_weight = self._get_sd_weight(tensor_values, used_keys, ["w2"])
+
+        # 2. Raise exceptions
+        if len(tensor_values) > 2:
+            unused_keys = set(tensor_values.keys()).difference(used_keys)
+            raise AttributeError(f"Unused weight(s): {', '.join(unused_keys)}")
+
+        # 3. Load and shard the weights
+        self.sharded_copy(self.w13, w13_weight, 1, [self.world_size, self.world_size])
+        self.sharded_copy(self.w2, w2_weight, 2, [self.world_size])
+
+    @staticmethod
+    def import_module(
+        cff: ConditionalFeedForward, group: ProcessGroup
+    ) -> "TPConditionalFeedForward":
+        tp_cff = TPConditionalFeedForward(
+            num_experts=cff.num_experts,
+            dim=cff.dim,
+            intermediate_size=cff.intermediate_size,
+            group=group,
+        )
+
+        return tp_cff
+
+    def forward(self, x, expert_indices):
+        x_par = copy_to_tensor_model_parallel_region(x)
+        out_par = ConditionalFeedForward.forward(self, x_par, expert_indices)
+        return reduce_from_tensor_model_parallel_region(out_par)
+
+
+class MOEFeedForward(nn.Module):
+    """
+    A Sparse Mixture Of Experts (MoE) Feed Forward layer. The output of this layer for a
+    given input is determined by the weighted sum of the outputs of a subset of size
+    `num_activated_experts` of the `num_experts` expert networks. The weights are given
+    by the gating network, then passed through a topK and a softmax filter to make it _sparse_.
+
+    For more information, see the review paper in https://arxiv.org/pdf/2209.01667.pdf
+
+    Args
+    ----
+    num_experts : int
+        The number of expert feed forward networks.
+    num_activated_experts : int
+        How many experts can be activated at any single time.
+    dim : int
+        The embedding dimension for the transformer model.
+    intermediate_size : int
+        The intermediate size for the expert networks.
+    """
+
+    def __init__(
+        self,
+        num_experts: int,
+        num_activated_experts: int,
+        dim: int,
+        intermediate_size: int,
+    ) -> None:
+        super().__init__()
+        self.gate = nn.Linear(dim, num_experts, bias=False)
+        self.cond_ffn = ConditionalFeedForward(num_experts, dim, intermediate_size)
+        self.dim = dim
+        self.num_activated_experts = num_activated_experts
+
+    def reset_parameters(self):
+        nn.init.trunc_normal_(
+            self.gate.weight,
+            mean=0.0,
+            std=0.02,
+        )
+
+        self.cond_ffn.reset_parameters()
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        B, S = x.shape[:2]
+        x = x.view(-1, self.dim)
+        # T = num_tokens, E = num_experts, D = hidden dim, A = activated experts
+        # x: [T, D]
+        scores = self.gate(x)  # [T, E]
+        expert_weights = F.softmax(scores, dim=-1)
+        expert_weights, expert_indices = torch.topk(
+            expert_weights, self.num_activated_experts, dim=-1
+        )  # [T, A], [T, A]
+        expert_weights /= expert_weights.sum(dim=-1, keepdim=True)  # [T, A]
+        expert_outs = self.cond_ffn(x, expert_indices)
+        int_v1 = torch.einsum("tai,ta -> ti", expert_outs, expert_weights)
+        int_v2 = int_v1.view(B, S, self.dim)
+        return int_v2
```

## fms/modules/head.py

```diff
@@ -1,14 +1,23 @@
-from typing import Optional
+from typing import Dict, List, Optional, Set
 
 import torch
+import torch.distributed
 import torch.nn as nn
+from torch.distributed.distributed_c10d import ProcessGroup
 
+from fms import distributed
+from fms.distributed.tensorparallel import (
+    all_gather_from_tensor_model_parallel_region,
+    copy_to_tensor_model_parallel_region,
+)
+from fms.modules.tp import TPModule
 
-class ClassificationHead(nn.Module):
+
+class MLPClassificationHead(nn.Module):
     """
     A general purpose Classification Head. When applied on the output of a
     Headless model, will project from the embedding space to a space equal to
     the number of classes provided.
     """
 
     def __init__(
@@ -19,15 +28,15 @@
         layer_norm: Optional[nn.Module] = None,
         dense_bias: bool = True,
         head_bias: bool = True,
         dropout: float = 0.0,
         apply_pooling_fn: bool = False,
     ):
         """
-        Initialize a ClassificationHead
+        Initialize a MLPClassificationHead
 
         Parameters
         ----------
         emb_dim: int
             the embedding dimension
         num_classes: int
             the output number of classes
@@ -71,7 +80,98 @@
         x = self.dense(x)
         x = self.act(x)
         x = self.dropout(x)
         if self.ln is not None:
             x = self.ln(x)
         x = self.head(x)
         return x
+
+
+class LinearClassificationHead(nn.Linear):
+    # To differentiate for TP
+    def forward(self, x):
+        return super().forward(x)
+
+    def to_tp(self, group: ProcessGroup) -> "TPLinearClassificationHead":
+        return TPLinearClassificationHead.import_module(self, group)
+
+
+class TPLinearClassificationHead(LinearClassificationHead, TPModule):
+    """
+    Output embedding layer for language models.
+
+    Args
+    ----
+    Check nn.Linear for up-to-date docs
+
+    world_size: int
+        the number of processes running this model in TP
+    rank: int
+        the index of this process wrt to the rest running the model in TP
+    """
+
+    def __init__(
+        self,
+        vocab_size,
+        emb_dim,
+        bias=False,
+        device=None,
+        dtype=None,
+        group: Optional[ProcessGroup] = None,
+    ):
+        assert torch.distributed.is_initialized()
+        rank, world_size = distributed.rank_and_world(group)
+        assert (
+            vocab_size % world_size == 0
+        ), "The number of tokens must be divisible by world size"
+        LinearClassificationHead.__init__(
+            self,
+            emb_dim,
+            vocab_size // world_size,
+            bias=bias,
+            device=device,
+            dtype=dtype,
+        )
+        self.setup_tp(rank, world_size)
+
+    @staticmethod
+    def import_module(
+        head: LinearClassificationHead, group: ProcessGroup
+    ) -> "TPLinearClassificationHead":
+        tp_lmh = TPLinearClassificationHead(
+            vocab_size=head.out_features,
+            emb_dim=head.in_features,
+            bias=head.bias,
+            device=head.weight.device,
+            dtype=head.weight.dtype,
+            group=group,
+        )
+        return tp_lmh
+
+    def load_weights(
+        self,
+        tensor_values: Dict[str, torch.Tensor],
+    ):
+        # 1. Grab the weights from tensor_values
+        used_keys: Set[str] = set()
+        head_weight = self._get_sd_weight(tensor_values, used_keys, ["weight"])
+        if self.bias != None:
+            head_bias = self._get_sd_weight(tensor_values, used_keys, ["bias"])
+
+        # 2. Raise exceptions
+        if len(tensor_values) > (2 if self.bias != None else 1):
+            unused_keys = set(tensor_values.keys()).difference(used_keys)
+            raise AttributeError(f"Unused weight(s): {', '.join(unused_keys)}")
+
+        # 3. Load and shard the weights
+        self.sharded_copy(self.weight, head_weight, 0, [self.world_size])
+        if self.bias != None:
+            self.sharded_copy(self.bias, head_bias, 0, [self.world_size])
+
+    def forward(self, inp):
+        # vocab_idx: b n d if reverse, else b n
+        inp_par = copy_to_tensor_model_parallel_region(inp)
+        out_par = LinearClassificationHead.forward(self, inp_par)
+        # with ints this wasn't `torch.compile`ing
+        rank = torch.tensor(self.rank)
+        world_size = torch.tensor(self.world_size)
+        return all_gather_from_tensor_model_parallel_region(out_par, rank, world_size)
```

## fms/modules/positions.py

```diff
@@ -97,15 +97,15 @@
             attn_mask = attn_mask.masked_fill(mask == 0, float("-inf"))
 
         return attn_mask
 
 
 class RotaryEmbedding(PositionEncoder):
     def __init__(
-        self, dim: int, ratio: int = 10_000, max_seq_len=2048, ntk_scaling=False
+        self, dim: int, ratio: float = 10_000.0, max_seq_len=2048, ntk_scaling=False
     ):
         """
         This implementation of Rotary Position Embeddings (RoPE) avoids
         complex numbers, and so can be used with torch.compile.
 
         https://arxiv.org/abs/2104.09864
 
@@ -236,15 +236,15 @@
 
         seq_len = max(k.size(1), q.size(1))
         if position_ids is None:
             # Compute position_ids based on cache config
             position_ids = torch.arange(
                 0, seq_len, dtype=torch.long, device=q.device
             ).repeat(k.size(0), 1)
-            if use_cache and past_kv_state is not None:
+            if use_cache and past_kv_state is not None and past_kv_state[0].numel() > 0:
                 position_ids += past_kv_state[0].size(2)
 
         q_ = q.float().view(*q.size()[:-1], -1, 2)  # B L H D/2 2
         k_ = k.float().view(*k.size()[:-1], -1, 2)  # B L H D/2 2
 
         # the max start position should be based on the max first position of each sequence
         max_start_pos = torch.max(position_ids[:, 0])
```

## fms/modules/tp.py

```diff
@@ -1,20 +1,20 @@
 import itertools
 from abc import ABCMeta, abstractmethod
-from typing import List, Type
+from typing import Dict, List, Set, Type, Union
 
 import torch
 import torch.nn as nn
 from torch.distributed.distributed_c10d import ProcessGroup
 
-from fms.distributed.tensorparallel import (
-    apply_colwise_tp,
-    apply_embedding_tp,
-    apply_rowwise_tp,
-)
+
+def _get_tpd_module(module: nn.Module, attr_name: str):
+    if attr_name == "self":
+        return module
+    return getattr(module, attr_name)
 
 
 class TPModule(nn.Module, metaclass=ABCMeta):
     """
     This is an abstract class that any nn.Module can implement to enable
     Tensor Parallel. On top of inheriting from this class, the TP module
     will have to implement list_colwise_weights, list_rowwise_weights,
@@ -27,58 +27,170 @@
     rank: int
     world_size: int
 
     def setup_tp(self, rank: int, world_size: int) -> None:
         self.rank = rank
         self.world_size = world_size
 
-    def colwise_param_names(self) -> List[str]:
-        return []
+    def __get_tp_slices(
+        self,
+        input_size,
+        output_size_per_partition,
+        max_partition_sizes,
+    ):
+        cusum_max_partition_sizes = [0]
+        min_partition_size = min(max_partition_sizes)
+        for m in max_partition_sizes:
+            cusum_max_partition_sizes.append(
+                cusum_max_partition_sizes[-1] + (m // min_partition_size)
+            )
+
+        for weight_i, replication in enumerate(max_partition_sizes):
+            # The shard to copy based on the process rank and the replication threshold
+            sharding_rank = self.rank // max(1, self.world_size // replication)
+            # The number of elements to shard out of the tensor
+            tensor_shard_size = output_size_per_partition * (
+                max(self.world_size, replication)
+                // max(self.world_size, min_partition_size)
+            )
+            # For fused weights, where to start extracting the shard
+            tensor_shard_offset = (
+                cusum_max_partition_sizes[weight_i]
+                * input_size
+                // cusum_max_partition_sizes[-1]
+            )
+            yield slice(
+                sharding_rank * tensor_shard_size + tensor_shard_offset,
+                (sharding_rank + 1) * tensor_shard_size + tensor_shard_offset,
+            )
 
-    def rowwise_param_names(self) -> List[str]:
-        return []
+    def sharded_copy(
+        self,
+        param: Union[torch.nn.Parameter, torch.Tensor],
+        tensor_value: torch.Tensor,
+        dim: int,
+        max_partition_sizes: List[int],
+        is_sharded: bool = True,
+    ):
+        """
+        This function copies the correct shard of the weights for a rowwise-TP'd module
+        according to the rank of the process and the world_size.
+
+        Args
+        ====
+        param: torch.nn.Parameter
+            Parameter that has had TP applied
+        tensor_value: torch.Tensor
+            tensor that needs sharding
+        dim: int
+            Dimension on which to shard. colwise sharding is usually dim 0, rowwise is usually dim 1
+        is_sharded: bool
+            For additive terms (like bias), is_sharded might be False. Otherwise True.
+        max_partition_sizes: List[int]
+            for each number in the list, if world_size is smaller than or equal to that number, the tensor will get
+            partitioned in worldsize parts, else if world size is larger than the number then you will get world size parts
+            replicated in worldsize / number
+
+            world_size = 4, max_partition_sizes = [8], tensor = [0 1 2 3 4 5 6 7]
+            [0 1] [2 3] [4 5] [6 7]
+
+            world_size = 8, max_partition_sizes = [4], tensor = [0 1 2 3 4 5 6 7]
+            [0 1] [0 1] [2 3] [2 3] [4 5] [4 5] [6 7] [6 7]
+
+            If there are multiple numbers in the max_partition_sizes list, then the param gets filled with non-contiguous
+            slices of the tensor_value. This is useful for fused weight cases (qkv, mlp, moe, etc.)
+
+            world_size = 4, max_partition_sizes = [4, 4], tensor = [0 1 2 3 4 5 6 7]
+            [0 4] [1 5] [2 6] [3 7]
+
+            world_size = 4, max_partition_sizes = [4, 1], tensor = [0 1 2 3 4 5 6 7 8 9]
+            [0 1 8 9] [2 3 8 9] [4 5 8 9] [6 7 8 9]
+        """
+        if is_sharded:
+            # In the case where world size is larger than any of the partition sizes, we must add replication up til the
+            # world size per partition
+            max_partition_sizes_replicated = [
+                max(self.world_size, m) for m in max_partition_sizes
+            ]
+            # Divide the weight matrix along the second dimension.
+            output_size_per_partition = param.shape[dim] // (
+                sum(max_partition_sizes_replicated)
+                // min(max_partition_sizes_replicated)
+            )
+            tp_slices = self.__get_tp_slices(
+                tensor_value.shape[dim], output_size_per_partition, max_partition_sizes
+            )
+            tp_shard_indices = [
+                tuple([slice(None) for _ in range(dim)] + [tp_slice])
+                for tp_slice in tp_slices
+            ]
+            tensors_to_cat = [
+                tensor_value[tp_shard_index] for tp_shard_index in tp_shard_indices
+            ]
+            tensor = torch.cat(tensors_to_cat, dim=dim)
+            param.copy_(tensor, non_blocking=True)
+        else:
+            if self.rank == 0:
+                param.copy_(tensor_value, non_blocking=True)
+            else:
+                param.zero_()
+
+    def _get_sd_weight(
+        self,
+        state_dict: Dict[str, torch.Tensor],
+        used_keys: Set[str],
+        substr_matches: List[str],
+    ):
+        results = []
+        for k in state_dict:
+            all_matches = True
+            for substr_match in substr_matches:
+                if substr_match not in k.split("."):
+                    all_matches = False
+            if all_matches:
+                used_keys.add(k)
+                results.append(state_dict[k])
+        if len(results) == 1:
+            return results[0]
+        elif len(results) > 1:
+            raise ValueError(
+                f"Conditions not stringent enough: keys are {', '.join(state_dict.keys())}"
+            )
+        else:
+            raise ValueError(
+                f"Weight not found, weights names are {', '.join(state_dict.keys())}"
+            )
 
-    def embedding_param_names(self) -> List[str]:
-        return []
+    def load_weights(
+        self,
+        tensor_values: Dict[str, torch.Tensor],
+    ):
+        """Load all tensor values into a TP module.
+
+        Override this method to load weights into a TP module. You can see
+        examples for all TP modules in FMS, but the functions will generally
+        have the following structure:
+
+        1. Grab the necessary weights from tensor_values. Which weights
+            these are depend on each module.
+        2. Raise exceptions for missing required weights in tensor_values
+            (ValueError) or for unused weights in tensor_values
+            (AttributeError)
+        3. Use the sharded_copy method to load and shard each weight correctly
+            into the TP module. Pay special attention to the max_partition_sizes
+            parameter for supporting fused weights and MQA/GQA among others.
+
+        PSA: Each weight has a List[int] (max_partition_sizes) associated
+        with it where if the list is larger than size 1, this implies the
+        weight is fused (where the length of the list is the number of fused
+        weights in a single parameter).
+
+        Args:
+            tensor_values: Dict[str, torch.Tensor]
+                a state dict containing all the weights for a TP module
+        """
+        pass
 
     @staticmethod
     @abstractmethod
     def import_module(module, group: ProcessGroup):
         pass
-
-    def import_weights(self, module: nn.Module):
-        for weight in self.colwise_param_names():
-            apply_colwise_tp(
-                getattr(self, weight),
-                getattr(module, weight),
-                self.world_size,
-                self.rank,
-            )
-        for weight in self.rowwise_param_names():
-            apply_rowwise_tp(
-                getattr(self, weight),
-                getattr(module, weight),
-                self.world_size,
-                self.rank,
-            )
-        for weight in self.embedding_param_names():
-            apply_embedding_tp(
-                getattr(self, weight),
-                getattr(module, weight),
-                self.world_size,
-                self.rank,
-            )
-        tp_sharded_modules = list(
-            itertools.chain(
-                self.colwise_param_names(),
-                self.rowwise_param_names(),
-                self.embedding_param_names(),
-            )
-        )
-        with torch.no_grad():
-            for mod_name, module in self.named_children():
-                if not mod_name in tp_sharded_modules:
-                    for param_name, param in module.named_parameters(recurse=False):
-                        param.copy_(
-                            getattr(getattr(module, mod_name), param_name),
-                            non_blocking=True,
-                        )
```

## fms/utils/generation.py

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, List, MutableMapping, Union
+from typing import Any, Callable, List, MutableMapping, Optional, Union
 
 import torch
 import torch.nn.functional as F
 
 
 def _make_cache_contiguous(past_key_value_states):
     # kv updates are required for torch.compile with
@@ -19,22 +19,23 @@
             # torch._dynamo.mark_dynamic(n_kv_s[layer_idx][tensor_idx], 2)
     return n_kv_s
 
 
 def generate(
     model: Union[Callable, torch.nn.Module],
     input_ids: torch.Tensor,
-    max_seq_len: int = 2048,
+    max_seq_len: int = 4096,
     max_new_tokens: int = 256,
     temperature: float = 1.0,
     top_k: int = 10,
     do_sample: bool = True,
     num_beams: int = 1,
     use_cache: bool = False,
     contiguous_cache: bool = False,
+    eos_token_id: Optional[int] = None,
 ):
     """
     A trivial generate function that can be used for validation/testing in
     cases where HF is not available.
     We could add implementations for other types of generation, but this is
     enough for making sure a model is working.
     Does not implement batching nor beam search, but those could be added.
@@ -60,14 +61,18 @@
             batched = True
     else:
         raise RuntimeError("generate() requires a tensor of token ids as the prefix")
 
     if not batched:
         input_ids = input_ids.unsqueeze(0)
 
+    eos_found = torch.zeros(
+        input_ids.shape[0], dtype=torch.bool, device=input_ids.device
+    )
+
     result = input_ids
     next_input = input_ids
     kwargs: MutableMapping[str, Any] = dict()
     kwargs["past_key_value_states"] = None
     kwargs["use_cache"] = use_cache
 
     for _ in range(max_new_tokens):
@@ -97,14 +102,20 @@
             probs = F.softmax(logits, dim=-1)
             next_val = torch.multinomial(probs, num_samples=1)
         else:
             next_val = torch.argmax(logits, dim=-1).unsqueeze(0).t()
 
         result = torch.cat((result, next_val), dim=-1)
 
+        # avoid continuing to generate if all have reached EOS
+        if eos_token_id is not None:
+            eos_found = torch.logical_or(eos_found, next_val == eos_token_id)
+            if torch.sum(eos_found) == input_ids.shape[0]:
+                break
+
         if use_cache:
             next_input = next_val
         else:
             next_input = result
 
     if not batched:
         result = result[0]
```

## fms/utils/serialization.py

```diff
@@ -1,13 +1,25 @@
 import collections
 import os
+import re
 from collections import ChainMap
 from collections.abc import Iterable
 from pathlib import Path
-from typing import Any, Callable, List, Mapping, MutableMapping, Optional, Set, Union
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Mapping,
+    MutableMapping,
+    Optional,
+    Set,
+    Tuple,
+    Union,
+)
 
 import torch
 
 from fms.modules.tp import TPModule
 
 
 __adapters: MutableMapping[str, MutableMapping[str, Callable[[Mapping], Mapping]]] = {}
@@ -51,14 +63,104 @@
                     `models.list_models()`.
     """
     if architecture not in __adapters:
         return []
     return list(__adapters[architecture].keys())
 
 
+def _legacy_attn_unfused_to_fused_adapter(orig_sd):
+    """
+    Legacy adapter for converting pre 0.0.6 unfused attn weights to fused attn weights
+    """
+    new_sd = {}
+    removed_params = set()
+    orig_keys = set(orig_sd.keys())
+    for name in orig_keys:
+        # if the name is part of removed_params, we no longer want to process it
+        if name in removed_params:
+            continue
+
+        if "attn.query" in name or "attn.key" in name or "attn.value" in name:
+            # weight_type denotes weight or bias
+            weight_type = name.split(".")[-1]
+
+            unfused_weights = [
+                re.sub(
+                    rf"attn.(query|key|value).{weight_type}",
+                    f"attn.query.{weight_type}",
+                    name,
+                ),
+                re.sub(
+                    rf"attn.(query|key|value).{weight_type}",
+                    f"attn.key.{weight_type}",
+                    name,
+                ),
+                re.sub(
+                    rf"attn.(query|key|value).{weight_type}",
+                    f"attn.value.{weight_type}",
+                    name,
+                ),
+            ]
+            removed_params.update(unfused_weights)
+            new_name = re.sub(
+                rf"attn.(query|key|value).{weight_type}",
+                f"attn.in_proj.qkv_fused.{weight_type}",
+                name,
+            )
+            new_sd[new_name] = torch.cat(
+                [orig_sd.pop(w) for w in unfused_weights], dim=0
+            )
+        else:
+            new_sd[name] = orig_sd.pop(name)
+    return new_sd
+
+
+def _legacy_mlp_glu_unfused_to_fused_adapter(orig_sd):
+    """
+    Legacy adapter for converting pre 0.0.6 unfused mlp glu weights to fused mlp glu weights
+    """
+    new_sd = {}
+    removed_params = set()
+    orig_keys = set(orig_sd.keys())
+    for name in orig_keys:
+        # if the name is part of removed_params, we no longer want to process it
+        if name in removed_params:
+            continue
+
+        if "ff_sub_layer.wg1_fused" not in name and (
+            "ff_sub_layer.wg" in name or "ff_sub_layer.w1" in name
+        ):
+            weight_type = name.split(".")[-1]
+
+            unfused_weights = [
+                re.sub(
+                    rf"ff_sub_layer.(wg|w1).{weight_type}",
+                    f"ff_sub_layer.wg.{weight_type}",
+                    name,
+                ),
+                re.sub(
+                    rf"ff_sub_layer.(wg|w1).{weight_type}",
+                    f"ff_sub_layer.w1.{weight_type}",
+                    name,
+                ),
+            ]
+            removed_params.update(unfused_weights)
+            new_name = re.sub(
+                rf"ff_sub_layer.(w1|wg).{weight_type}",
+                f"ff_sub_layer.wg1_fused.{weight_type}",
+                name,
+            )
+            new_sd[new_name] = torch.cat(
+                [orig_sd.pop(w) for w in unfused_weights], dim=0
+            )
+        else:
+            new_sd[name] = orig_sd.pop(name)
+    return new_sd
+
+
 def _get_adapter(
     architecture: str, source: Optional[str]
 ) -> Callable[[Mapping[str, Any]], Mapping[str, Any]]:
     if (
         source is None
         or architecture not in __adapters
         or source not in __adapters[architecture]
@@ -198,17 +300,15 @@
         ), f"Loading a {checkpoint_sharding}-sharded checkpoint with len={len(checkpoints)} but world size is {world_size}"
 
         checkpoints = [checkpoints[rank]]
 
     # if there's only one checkpoint for fsdp/hsdp, load it only into rank zero
     # and it will be distributed by the FSDP `sync_module_states` parameter
     if checkpoint_sharding is None and distributed_strategy in {"hsdp", "fsdp"}:
-        if rank == 0:
-            checkpoints = [checkpoints[0]]
-        else:
+        if rank != 0:
             return {}
 
     checkpoint_sds = []
     if checkpoints[0].suffix == ".safetensors":
         for ckp in checkpoints:
             checkpoint_sds.append(
                 _load_safetensors_state_dict(
@@ -238,41 +338,47 @@
             sd.set_lazy_tensor(key, checkpoint, device)
     return sd
 
 
 def _find_key_neighbors(key: str, sd_keys: Set[str]):
     # For loading most models that concern us, a good partition is the
     # one used for FSDP units: everything that is in a layer can
-    # go together and memory usage will be keep in control
+    # go together, everything else can also go together and memory usage
+    # will be keep in control.
     key_steps = key.split(".")
     prefix = ""
     # Navigate the model tree to find a layer index. If not found,
-    # grab that weight alone
+    # grab everything that is not numerical
+    has_number = False
     for idx, step in enumerate(key_steps):
         prefix = ".".join(key_steps[: idx + 1])
         if step.isnumeric():
             prefix += "."
+            has_number = True
             break
     prefix_neighbors = set()
-    for key_in_sd in sd_keys:
-        if prefix in key_in_sd:
-            prefix_neighbors.add(key_in_sd)
+    if has_number:
+        for key_in_sd in sd_keys:
+            if prefix in key_in_sd:
+                prefix_neighbors.add(key_in_sd)
+    else:
+        for key_in_sd in sd_keys:
+            if not bool(re.search(r"\.\d+\.", key_in_sd)):
+                prefix_neighbors.add(key_in_sd)
     return list(prefix_neighbors)
 
 
 def load_state_dict_into_model(
     model: torch.nn.Module,
     state_dict: MutableMapping[str, Any],
     architecture: str,
     source: str,
     distributed_strategy: Optional[str] = None,
     checkpoint_sharding: Optional[str] = None,
     initial_device: torch.device = torch.device("cpu"),
-    rank: int = 0,
-    world_size: int = 0,
 ) -> None:
     """
     This function loads state_dict into model in the most efficient way possible,
     and it removes all weights that have been used in model from state_dict
     in order to conserve memory.
 
     Args:
@@ -306,152 +412,55 @@
         for key in sd_keys:
             if key in used_keys:
                 continue
             used_keys.add(key)
 
             partial_sd = {key: state_dict[key]}
             # Find neighbors to the key. If the adapter requires a neighbor and
-            # this function doesn't find it, it will crash. This is useful when
-            # adapters merge multiple weights into one, e.g. if the source state
-            # dict has unfused q,k,v projections and your model has fused qkv, you
-            # want your partial_sd to have the three weights available at a time
+            # this function doesn't find it, it will crash.
             remaining_keys = sd_keys.difference(used_keys)
             neighbors = _find_key_neighbors(key, remaining_keys)
             for neighbor in neighbors:
                 partial_sd[neighbor] = state_dict[neighbor]
                 used_keys.add(neighbor)
             for psd_key in partial_sd.keys():
                 if partial_sd[psd_key].device != initial_device:
                     partial_sd[psd_key] = partial_sd[psd_key].to(device=initial_device)
             fms_partial_sd = adapter(partial_sd)
-            _load_partial_state_dict(
-                model, fms_partial_sd, needs_tp_sharding, rank, world_size
-            )
+            _load_partial_state_dict(model, fms_partial_sd, needs_tp_sharding)
             # Be aggressive in removing weights to save as much memory as possible
             for p_key in partial_sd.keys():
                 if isinstance(state_dict, ChainMap):
                     for child_sd in state_dict.maps:
                         child_sd.pop(p_key, None)
                 else:
                     state_dict.pop(p_key)
             del partial_sd
             del fms_partial_sd
 
 
-def _copy_colwise(param: torch.nn.Parameter, tensor_value, is_bias, rank, world_size):
-    """
-    This function copies the correct shard of the weights for a colwise-TP'd module
-    according to the rank of the process and the world_size.
-
-    Args
-    ====
-    param: torch.nn.Parameter
-        Parameter that has had TP applied
-    tensor_value: torch.Tensor
-        tensor that needs sharding
-    rank: int
-        Rank of the current process
-    world_size: int
-        Total number of TP processes
-    """
-    # Divide the weight matrix along the first dimension.
-    output_size_per_partition = param.shape[0]
-    if not is_bias:
-        tensor = tensor_value[
-            (rank * output_size_per_partition) : (
-                (rank + 1) * output_size_per_partition
-            ),
-            :,
-        ]
-    else:
-        tensor = tensor_value[
-            (rank * output_size_per_partition) : (
-                (rank + 1) * output_size_per_partition
-            )
-        ]
-    param.copy_(tensor, non_blocking=True)
-
-
-def _copy_rowwise(param: torch.nn.Parameter, tensor_value, is_bias, rank, world_size):
-    """
-    This function copies the correct shard of the weights for a rowwise-TP'd module
-    according to the rank of the process and the world_size.
-
-    Args
-    ====
-    param: torch.nn.Parameter
-        Parameter that has had TP applied
-    tensor_value: torch.Tensor
-        tensor that needs sharding
-    rank: int
-        Rank of the current process
-    world_size: int
-        Total number of TP processes
-    """
-    # Divide the weight matrix along the last dimension.
-    if not is_bias:
-        output_size_per_partition = param.shape[1]
-        tensor = tensor_value[
-            :,
-            (rank * output_size_per_partition) : (
-                (rank + 1) * output_size_per_partition
-            ),
-        ]
-        param.copy_(tensor, non_blocking=True)
-    else:
-        if rank == 0:
-            _copy_if_present(param, tensor_value)
-        else:
-            param.zero_()
-
-
-def _copy_embedding(param: torch.nn.Parameter, tensor_value, rank, world_size):
-    """
-    This function copies the correct shard of the weights for a TP'd embedding module
-    according to the rank of the process and the world_size.
-
-    Args
-    ====
-    param: torch.nn.Parameter
-        Parameter that has had TP applied
-    tensor_value: torch.Tensor
-        tensor that needs sharding
-    rank: int
-        Rank of the current process
-    world_size: int
-        Total number of TP processes
-    """
-    # Divide the weight matrix along the last dimension.
-    output_size_per_partition = param.shape[1]
-    tensor = tensor_value[
-        :,
-        (rank * output_size_per_partition) : ((rank + 1) * output_size_per_partition),
-    ]
-    param.copy_(tensor, non_blocking=True)
-
-
 def _copy_if_present(parameter, tensor_value):
     parameter.copy_(tensor_value, non_blocking=True)
 
 
 def _load_partial_state_dict(
     model: torch.nn.Module,
     state_dict,
     needs_tp_sharding: bool,
-    rank=0,
-    world_size=1,
 ):
     unused_params = []
+    seen_tp_modules = set()
     for key, tensor_value in state_dict.items():
         target_module = model
         # Find where to put the weight and decide whether it needs TP'ing
         key_steps = key.split(".")
         prefix = ""
         key_step = 0
         tp_module = None
+        tp_prefix = ""
         # Navigate the model tree to find the module where the parameter is
         # located and whether there is a TPModule in the way in case the
         # parameter requires sharding
         while key_step < len(key_steps) - 1:
             try:
                 target_module = getattr(target_module, key_steps[key_step])
                 if key_step > 0:
@@ -460,46 +469,25 @@
                 key_step += 1
                 if isinstance(target_module, Iterable):
                     target_module = target_module[int(key_steps[key_step])]  # type: ignore[index]
                     prefix += "." + key_steps[key_step]
                     key_step += 1
                 if isinstance(target_module, TPModule):
                     tp_module = target_module
+                    tp_prefix = prefix
             except AttributeError:
                 unused_params.append(key)
                 break
 
         # Check if target_module has the Parameter/buffer
         try:
-            param = getattr(target_module, key_steps[-1])
-
             # If TP sharding is not needed, copy the parameter
             # into the model
             if not needs_tp_sharding or tp_module is None:
-                _copy_if_present(param, tensor_value)
-            elif tp_module is not None:
-                # Handle TP sharding
-                if key_steps[-2] in tp_module.colwise_param_names():
-                    _copy_colwise(
-                        param,
-                        tensor_value,
-                        key_steps[-1] == "bias",
-                        rank,
-                        world_size,
-                    )
-                if key_steps[-2] in tp_module.rowwise_param_names():
-                    _copy_rowwise(
-                        param,
-                        tensor_value,
-                        key_steps[-1] == "bias",
-                        rank,
-                        world_size,
-                    )
-                if key_steps[-2] in tp_module.embedding_param_names():
-                    _copy_embedding(
-                        param,
-                        tensor_value,
-                        rank,
-                        world_size,
-                    )
+                param = getattr(target_module, key_steps[-1])
+                param.copy_(tensor_value, non_blocking=True)
+            elif tp_module is not None and tp_module not in seen_tp_modules:
+                seen_tp_modules.add(tp_module)
+                tensor_values = {k: v for k, v in state_dict.items() if tp_prefix in k}
+                tp_module.load_weights(tensor_values)
         except AttributeError:
             unused_params.append(key)
```

## fms/utils/tp_wrapping.py

```diff
@@ -1,38 +1,26 @@
 from torch import nn
 from torch.distributed.distributed_c10d import ProcessGroup
 
-from fms.modules.attention import MultiHeadAttention, TPMultiHeadAttention
-from fms.modules.embedding import TPWordEmbedding, WordEmbedding
-from fms.modules.feedforward import (
-    FeedForwardBlock,
-    GatedLinearUnit,
-    TPFeedForwardBlock,
-    TPGatedLinearUnit,
-)
+from fms.modules.embedding import TPEmbedding
 from fms.modules.positions import Alibi
 
 
 # this probably belongs somewhere else but can't go in fms.distribtued b/c
 # circular dependency.
 def _tp_wrapped(module: nn.Module, group: ProcessGroup):
     if hasattr(module, "to_tp"):
         return module.to_tp(group)
-    elif isinstance(module, FeedForwardBlock):
-        return TPFeedForwardBlock.import_module(module, group)
-    elif isinstance(module, GatedLinearUnit):
-        return TPGatedLinearUnit.import_module(module, group)
-    elif isinstance(module, MultiHeadAttention):
-        return TPMultiHeadAttention.import_module(module, group)
     elif isinstance(module, Alibi):
         raise NotImplementedError("TODO: implement TP for Alibi")
         # tp_layer = TPAlibi.import_module(layer, world_size, rank, dtype)
         # setattr(model, name, tp_layer)
-    elif isinstance(module, WordEmbedding):
-        return TPWordEmbedding.import_module(module, group)
+    elif isinstance(module, nn.Embedding):
+        # We can't directly modify torch.nn modules to add the to_tp function
+        return TPEmbedding.import_module(module, group)
     else:
         return module
 
 
 def apply_tp(model: nn.Module, group: ProcessGroup):
     wrapped = _tp_wrapped(model, group)
     if wrapped is not model:
```

## Comparing `ibm_fms-0.0.5.dist-info/LICENSE` & `ibm_fms-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ibm_fms-0.0.5.dist-info/METADATA` & `ibm_fms-0.0.6.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ibm-fms
-Version: 0.0.5
+Version: 0.0.6
 Summary: IBM Foundation Model Stack
 Home-page: https://github.com/foundation-model-stack/foundation-model-stack
 Author: Brian Vaughan, Joshua Rosenkranz, Antoni Viros i Martin, Davis Wertheimer, Supriyo Chakraborty, Raghu Kiran Ganti
 Author-email: bvaughan@ibm.com, jmrosenk@us.ibm.com, aviros@ibm.com, Davis.Wertheimer@ibm.com, supriyo@us.ibm.com, rganti@us.ibm.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 License-File: LICENSE
-Requires-Dist: torch (>=2.1)
+Requires-Dist: torch >=2.2
 Provides-Extra: hf
-Requires-Dist: transformers (>=4.35.0) ; extra == 'hf'
+Requires-Dist: transformers >=4.40.2 ; extra == 'hf'
```

## Comparing `ibm_fms-0.0.5.dist-info/RECORD` & `ibm_fms-0.0.6.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,63 @@
 fms/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+fms/py.typed,sha256=SVy5SbzGZMwIrHje2DAU-o0KvzrQdIJDmp2Og_0M4ws,152
 fms/datasets/__init__.py,sha256=R8JlXkBSNJ6Nt1M5gsTOf2o5H8iBQu_2gEUiq04B7sw,1786
 fms/datasets/arrow.py,sha256=BCm5Dv-MjJ04dPGAR2CMWvMbtO56_rMmpN1Su3_R35A,5384
 fms/datasets/instructions.py,sha256=Ltnd-rWPrwCLwTDfnrbUoh6e5MGeB26Oclsl4nrh8Bk,3055
 fms/datasets/text.py,sha256=eoXfUzFw8jCz23YhjLZNEHMFEqJREZcuD0wkAkQHnqY,2968
 fms/datasets/util.py,sha256=ehat5sRTqwuLQB3DFD7L5o3Y720x21O1jehN_Sjlqlc,5159
 fms/distributed/__init__.py,sha256=uKysiqWCseHUck_fql2ceCLVpOINfg8TANJVIO3HEcI,590
 fms/distributed/strategy.py,sha256=77atjbmP-3zpKo10tc_SezY0qg5xCa8SVZFldcH9ol0,4006
-fms/distributed/tensorparallel.py,sha256=paxYexSysK5cgaajFt_pzlHqA1UyVSXTOaPAzwq7Avs,7423
-fms/models/__init__.py,sha256=d73XqdD0p4znNv-gjQEqm5MLJW56DDsUmOoh6YFK1VU,10549
-fms/models/gpt_bigcode.py,sha256=bkk8HfbClGC29Yju415ezE1ILbUMGnrsr59JIymZ8c0,15081
-fms/models/llama.py,sha256=pDaOgU8495YRMiJ3SpuHpruiGpto8Aw-PsVhAs9f6pM,18367
-fms/models/roberta.py,sha256=V0j5dLc7CYYbgREbsYi8SL8bfsurnI_gyANqG4ReTwo,10683
-fms/models/hf/__init__.py,sha256=JkuqV77T_K4pn6KSoaBbsVTyGo0r_XyZ_UE62wP6NMc,1426
-fms/models/hf/lm_head_mixins.py,sha256=zW_qansMMm9pGKM3IEKzmxXJfR_6Q4llK5wMAa_Z1Rw,14675
+fms/distributed/tensorparallel.py,sha256=aUQt1VoIfzlX66iLykN7AapY5DEpnSKlhDs0v8hf7Os,5642
+fms/models/__init__.py,sha256=lGgGEZP9NsCkNGJU2krPi3qYPcevZ3Db9E4ym1xeIF0,10567
+fms/models/gpt_bigcode.py,sha256=o6L8WklqyfR2s8ZUZ1N2ngeHH5ThIRBUZe9dj73BbZQ,13972
+fms/models/llama.py,sha256=Lw3BmURY3XPyVtWiazdKPbe261wwCM-M19WOfPFhgKw,18777
+fms/models/mixtral.py,sha256=nPivHHoJbZD7IblAOaMA0WakpVrydUkrSE4dL01i9MA,14397
+fms/models/roberta.py,sha256=pQeyjMBNQjRMi2kQHHWG_0oMJTILCQP5V2WkXRfzP_I,10861
+fms/models/hf/__init__.py,sha256=L2quEdWWQVUIu3GaFIhmCmLmnmVCqc5NuLlUrNo_zcg,1766
+fms/models/hf/lm_head_mixins.py,sha256=Y0qGXlNdpg2-4RqEArHPuegHQVeMx9C6zJDHs_mA7ss,14684
 fms/models/hf/modeling_hf_adapter.py,sha256=JE_IN79AQniQxgW92rP9WKtW8oumSHh5LmaKnagpXn0,84324
 fms/models/hf/utils.py,sha256=lL-gOGbBMpefTAOPUBISn-n3jvRt-cGYCMMsR2-ajWM,4775
-fms/models/hf/gpt_bigcode/__init__.py,sha256=jKiTvB6iC7UXEHafLea9nw5Cle7rmuOr2Gdjd4FMoZc,3488
+fms/models/hf/gpt_bigcode/__init__.py,sha256=dNDf4G7CCleJdctxM-BmXPlYtxHaY509RnW1A33sMO8,3014
 fms/models/hf/gpt_bigcode/configuration_gpt_bigcode_hf.py,sha256=v8dhpmpUT69iOW_CJPiW3DapnRgYTST_Hr77rFC9ZoM,2659
 fms/models/hf/gpt_bigcode/modeling_gpt_bigcode_hf.py,sha256=cy6oEyc2kBbahjo3s1B1RK5RyrMgOn78dkbmeMfzG5Y,3420
 fms/models/hf/llama/__init__.py,sha256=cYzKdD7_H1_DGagC-Ylw2RBLc8LMQvnP7T7cF5zBZl8,1498
 fms/models/hf/llama/configuration_llama_hf.py,sha256=iwDCXWIcjE3ChfmhcvN36s6bfPCo9ls4JP-fGjHmEws,2509
 fms/models/hf/llama/modeling_llama_hf.py,sha256=dVy461_TUGNgx3mChvj5egrVa866MHqLW-Rm41L-hzY,4822
+fms/models/hf/mixtral/__init__.py,sha256=kzxKG5Bv-yNtHN9t6R5jS7Ptu9vs5oJHFA8cBdaF3Ko,3754
+fms/models/hf/mixtral/configuration_mixtral_hf.py,sha256=hxgpS8L3UUnD0HyfYvdWl-OSWr-nsuDhpm2rp9_kqIU,2697
+fms/models/hf/mixtral/modeling_mixtral_hf.py,sha256=yUITmWyO16L4gYhF19GAqwQZGkUJlTsYZn_M5Qvg-RY,4607
 fms/models/hf/roberta/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fms/models/hf/roberta/modeling_roberta_hf.py,sha256=AkVycY88b5KfFVSucup4Ixft-Xm77ztSY3kYoNhFBY0,6187
+fms/models/hf/roberta/modeling_roberta_hf.py,sha256=JB5nwxsMiePtqgxGNZhy2jWzYDbvnu-wUazg-4a_2-0,6319
 fms/modules/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fms/modules/attention.py,sha256=6AmKrFWuWom6kq0X68vw5cBlirIagRdNbbrCv7wpo3A,12229
-fms/modules/embedding.py,sha256=Ab7WG1CByrhFCopabUAtVufcok3wnLWbGzDPZEwYYm4,8306
-fms/modules/feedforward.py,sha256=qJ0F5mSMIcpdGaTIS7r4oWUNZbIrnclkCIExvgNiDZo,8944
-fms/modules/head.py,sha256=l5H6hAtX4Dp9D9zMcvtlyEHAxyKSMlvV_upjdJzinYs,2467
+fms/modules/attention.py,sha256=nYWtiTovOWdUUcaFkfx0uCYDSzpR9tolyI0sKGWRjkg,21990
+fms/modules/embedding.py,sha256=gKYWaS6IR2AvCe_hbRnkLwCX--YhD65z5g5bUCLXFl8,12304
+fms/modules/feedforward.py,sha256=Yb7W19PVsN0ETLXjLwhEMM-7FOP-KrTGOfvRxYtrhns,18900
+fms/modules/head.py,sha256=i7alm8IdnML9XrlhKgaWcw_daAteatGL8dRFkL68ldU,5777
 fms/modules/layernorm.py,sha256=Wiu6ulrr0LGYAucv-4RVyAGPZaWpVEUqlCW_69G5lMo,2488
-fms/modules/positions.py,sha256=sCUoJ9xIN7VqL_tlyI-G-w0DF_SISzN_yI0YC3cI9hA,9492
-fms/modules/tp.py,sha256=Aa55yHChChjQYyPFxcrmKEn39zDWkBDzksi36Y6MT3Q,2661
+fms/modules/positions.py,sha256=GWsIdRJdYiSEFJ8EOvjnyr39zFnPgYCY133Sz1MKFHs,9529
+fms/modules/tp.py,sha256=PJHMp-799Dku5OQ6cO82fqOlQT3GFslYxpWaEYkZdig,7727
 fms/testing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fms/testing/comparison.py,sha256=fX-sUW_sz8hhzIRTZjbkaD5Qr5JXsuERq94oKxmXPlU,5596
 fms/testing/_internal/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fms/testing/_internal/model_test_suite.py,sha256=IzEZQEJg5fl1LCslqINz_7sr_uVYr555_ox3hW0ytmE,9461
 fms/testing/_internal/hf/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fms/testing/_internal/hf/model_test_suite.py,sha256=PM3cK7WdAQYX60oIz7Yy6b-tIq9fAeRwV2CIb0ouGj0,14836
 fms/training/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fms/training/plugins.py,sha256=46ryjAkHnXJykUw-tklRzgPiaQahLo2U-Y3b1CCUVWs,12732
 fms/training/trainer.py,sha256=CZgRI0cetXAkR1xqCKaaICEKFTKFLjFK8QSiN89ytnA,3086
+fms/triton/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+fms/triton/moe_kernel.py,sha256=FHch0Ak_sqEOrlBuYc7fdZ_NPkw5CUjkdD16KO5Jchs,15441
 fms/utils/__init__.py,sha256=D_byaw4RQk-IKnYyxSPUJSwroK_TyA609Ff2yM3j20o,650
 fms/utils/activation.py,sha256=8WQA2DFjtymHuvqamZvb1zbRkDJGUEZtRNqRXJ3U1LQ,2020
 fms/utils/config.py,sha256=x2kL9NBWZH2yJ0Qre_rgeAS7-kTOhDyi_D45bj3w-0M,1872
 fms/utils/evaluation.py,sha256=XOe5jLlzogssZ_oInVG7ls3fR05DXT-69XplrW7kQhE,2626
-fms/utils/generation.py,sha256=vjCh6sEZNwLFT15VHExCCKbm50zl3kUqjUlskvU8UMg,4377
-fms/utils/serialization.py,sha256=zbOnliQfhFW-WKWECLaMtKv8aLdPIAFVC7uiv9u6Rx0,18133
+fms/utils/generation.py,sha256=HFVLuP1MlOMzDvl5XZNU3RPPWJTq0YXCIj1tRGu10Lo,4793
+fms/utils/serialization.py,sha256=lV2M6Es6c-p76n1cJ7k0xZlWBVQtH_50cNZfVNz9q70,17672
 fms/utils/tensors.py,sha256=0tsR9o3ov_v1wWxByKTbHBq6xDAoydyoqnWd_fMUo7E,4982
 fms/utils/tokenizers.py,sha256=TovD2WsigU8ErMTBAIHBABEf0mAqLIrgonj6T_5xLNk,5337
-fms/utils/tp_wrapping.py,sha256=g2k5ayIaqJeo-hRKT74NGHaO7qNKnREp1eXGkpCmdtk,1596
-ibm_fms-0.0.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-ibm_fms-0.0.5.dist-info/METADATA,sha256=4peRnd6WsMtMFpKX2PSFxKDTEfngr15ZKc3YTcUvRoQ,683
-ibm_fms-0.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-ibm_fms-0.0.5.dist-info/top_level.txt,sha256=4q4zprUhYB424UwinVFiS1FPsd3KHv1_Y1qvef7MtPw,4
-ibm_fms-0.0.5.dist-info/RECORD,,
+fms/utils/tp_wrapping.py,sha256=GpQhTY_np0pxjJefSTKgifHsf3Gqes-pORvwIkSvAws,1113
+ibm_fms-0.0.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+ibm_fms-0.0.6.dist-info/METADATA,sha256=mXp2elGJCK3iu_xxg24-oUATKbaEbfRiflkTqoJwV2w,679
+ibm_fms-0.0.6.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+ibm_fms-0.0.6.dist-info/top_level.txt,sha256=4q4zprUhYB424UwinVFiS1FPsd3KHv1_Y1qvef7MtPw,4
+ibm_fms-0.0.6.dist-info/RECORD,,
```

