# Comparing `tmp/ptdeco-0.4.0.tar.gz` & `tmp/ptdeco-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptdeco-0.4.0.tar", last modified: Sun Jan  7 22:27:58 2024, max compression
+gzip compressed data, was "ptdeco-0.5.0.tar", last modified: Fri May 24 11:14:58 2024, max compression
```

## Comparing `ptdeco-0.4.0.tar` & `ptdeco-0.5.0.tar`

### file list

```diff
@@ -1,36 +1,41 @@
-drwxr-xr-x   0 lopusz   (10000) lopusz   (10000)        0 2024-01-07 22:27:58.261944 ptdeco-0.4.0/
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)    11358 2023-12-01 09:29:42.000000 ptdeco-0.4.0/LICENSE
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)    20668 2024-01-07 22:27:58.261944 ptdeco-0.4.0/PKG-INFO
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)     7338 2024-01-07 18:09:46.000000 ptdeco-0.4.0/README.md
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)      628 2024-01-07 18:06:44.000000 ptdeco-0.4.0/pyproject.toml
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)       12 2023-11-06 09:18:55.000000 ptdeco-0.4.0/requirements.txt
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)       38 2024-01-07 22:27:58.261944 ptdeco-0.4.0/setup.cfg
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)      524 2023-11-16 12:01:31.000000 ptdeco-0.4.0/setup.py
-drwxr-xr-x   0 lopusz   (10000) lopusz   (10000)        0 2024-01-07 22:27:58.257943 ptdeco-0.4.0/src/
-drwxr-xr-x   0 lopusz   (10000) lopusz   (10000)        0 2024-01-07 22:27:58.257943 ptdeco-0.4.0/src/ptdeco/
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)      168 2023-11-15 11:04:35.000000 ptdeco-0.4.0/src/ptdeco/__init__.py
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)      282 2023-11-20 22:47:34.000000 ptdeco-0.4.0/src/ptdeco/_version.py
-drwxr-xr-x   0 lopusz   (10000) lopusz   (10000)        0 2024-01-07 22:27:58.257943 ptdeco-0.4.0/src/ptdeco/falor/
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)      104 2023-11-15 11:04:35.000000 ptdeco-0.4.0/src/ptdeco/falor/__init__.py
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)    15505 2023-12-21 14:06:44.000000 ptdeco-0.4.0/src/ptdeco/falor/decomposition.py
-drwxr-xr-x   0 lopusz   (10000) lopusz   (10000)        0 2024-01-07 22:27:58.257943 ptdeco-0.4.0/src/ptdeco/lockd/
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)      158 2023-11-15 11:04:35.000000 ptdeco-0.4.0/src/ptdeco/lockd/__init__.py
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)    16531 2023-11-15 11:04:35.000000 ptdeco-0.4.0/src/ptdeco/lockd/decomposition.py
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)     2837 2023-11-15 11:04:35.000000 ptdeco-0.4.0/src/ptdeco/lockd/losses.py
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)        0 2023-11-15 11:04:35.000000 ptdeco-0.4.0/src/ptdeco/py.typed
-drwxr-xr-x   0 lopusz   (10000) lopusz   (10000)        0 2024-01-07 22:27:58.261944 ptdeco-0.4.0/src/ptdeco/utils/
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)      299 2023-11-15 11:04:35.000000 ptdeco-0.4.0/src/ptdeco/utils/__init__.py
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)     1060 2023-11-15 11:04:35.000000 ptdeco-0.4.0/src/ptdeco/utils/common.py
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)     1116 2023-11-15 11:04:35.000000 ptdeco-0.4.0/src/ptdeco/utils/losses_primitives.py
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)     4318 2023-11-15 11:04:35.000000 ptdeco-0.4.0/src/ptdeco/utils/modconfig.py
-drwxr-xr-x   0 lopusz   (10000) lopusz   (10000)        0 2024-01-07 22:27:58.261944 ptdeco-0.4.0/src/ptdeco.egg-info/
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)    20668 2024-01-07 22:27:58.000000 ptdeco-0.4.0/src/ptdeco.egg-info/PKG-INFO
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)      723 2024-01-07 22:27:58.000000 ptdeco-0.4.0/src/ptdeco.egg-info/SOURCES.txt
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)        1 2024-01-07 22:27:58.000000 ptdeco-0.4.0/src/ptdeco.egg-info/dependency_links.txt
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)       12 2024-01-07 22:27:58.000000 ptdeco-0.4.0/src/ptdeco.egg-info/requires.txt
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)        7 2024-01-07 22:27:58.000000 ptdeco-0.4.0/src/ptdeco.egg-info/top_level.txt
-drwxr-xr-x   0 lopusz   (10000) lopusz   (10000)        0 2024-01-07 22:27:58.261944 ptdeco-0.4.0/tests/
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)     3164 2023-11-09 09:46:50.000000 ptdeco-0.4.0/tests/test_config_torchvision_timm.py
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)     2686 2023-11-09 09:46:50.000000 ptdeco-0.4.0/tests/test_decompose_torchvision_timm.py
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)     3159 2023-11-15 11:04:35.000000 ptdeco-0.4.0/tests/test_losses_torchvision_timm.py
--rw-r--r--   0 lopusz   (10000) lopusz   (10000)     2485 2023-11-09 09:46:50.000000 ptdeco-0.4.0/tests/test_wrap_torchvision_timm.py
+drwxr-xr-x   0 lopusz   (10000) lopusz   (10000)        0 2024-05-24 11:14:58.522796 ptdeco-0.5.0/
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)    11358 2023-12-01 09:29:42.000000 ptdeco-0.5.0/LICENSE
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)    17309 2024-05-24 11:14:58.522796 ptdeco-0.5.0/PKG-INFO
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)     3979 2024-05-23 12:53:51.000000 ptdeco-0.5.0/README.md
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)      628 2024-02-27 23:14:59.000000 ptdeco-0.5.0/pyproject.toml
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)       12 2023-11-06 09:18:55.000000 ptdeco-0.5.0/requirements.txt
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)       38 2024-05-24 11:14:58.522796 ptdeco-0.5.0/setup.cfg
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)      524 2023-11-16 12:01:31.000000 ptdeco-0.5.0/setup.py
+drwxr-xr-x   0 lopusz   (10000) lopusz   (10000)        0 2024-05-24 11:14:58.518795 ptdeco-0.5.0/src/
+drwxr-xr-x   0 lopusz   (10000) lopusz   (10000)        0 2024-05-24 11:14:58.518795 ptdeco-0.5.0/src/ptdeco/
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)      168 2024-04-09 10:49:25.000000 ptdeco-0.5.0/src/ptdeco/__init__.py
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)      282 2024-05-24 11:13:08.000000 ptdeco-0.5.0/src/ptdeco/_version.py
+drwxr-xr-x   0 lopusz   (10000) lopusz   (10000)        0 2024-05-24 11:14:58.518795 ptdeco-0.5.0/src/ptdeco/dwain/
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)      104 2024-04-09 10:49:25.000000 ptdeco-0.5.0/src/ptdeco/dwain/__init__.py
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)    27130 2024-05-16 20:02:13.000000 ptdeco-0.5.0/src/ptdeco/dwain/decomposition.py
+drwxr-xr-x   0 lopusz   (10000) lopusz   (10000)        0 2024-05-24 11:14:58.522796 ptdeco-0.5.0/src/ptdeco/falor/
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)      104 2024-02-27 23:14:59.000000 ptdeco-0.5.0/src/ptdeco/falor/__init__.py
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)    17316 2024-05-09 21:34:19.000000 ptdeco-0.5.0/src/ptdeco/falor/decomposition.py
+drwxr-xr-x   0 lopusz   (10000) lopusz   (10000)        0 2024-05-24 11:14:58.522796 ptdeco-0.5.0/src/ptdeco/lockd/
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)      158 2024-02-27 23:14:59.000000 ptdeco-0.5.0/src/ptdeco/lockd/__init__.py
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)    16531 2024-02-27 23:14:59.000000 ptdeco-0.5.0/src/ptdeco/lockd/decomposition.py
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)     2837 2024-02-27 23:14:59.000000 ptdeco-0.5.0/src/ptdeco/lockd/losses.py
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)        0 2024-02-27 23:14:59.000000 ptdeco-0.5.0/src/ptdeco/py.typed
+drwxr-xr-x   0 lopusz   (10000) lopusz   (10000)        0 2024-05-24 11:14:58.522796 ptdeco-0.5.0/src/ptdeco/utils/
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)      299 2024-02-27 23:14:59.000000 ptdeco-0.5.0/src/ptdeco/utils/__init__.py
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)     2569 2024-04-22 08:39:34.000000 ptdeco-0.5.0/src/ptdeco/utils/common.py
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)     1914 2024-04-09 10:49:25.000000 ptdeco-0.5.0/src/ptdeco/utils/losses_primitives.py
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)     4318 2024-02-27 23:14:59.000000 ptdeco-0.5.0/src/ptdeco/utils/modconfig.py
+drwxr-xr-x   0 lopusz   (10000) lopusz   (10000)        0 2024-05-24 11:14:58.522796 ptdeco-0.5.0/src/ptdeco.egg-info/
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)    17309 2024-05-24 11:14:58.000000 ptdeco-0.5.0/src/ptdeco.egg-info/PKG-INFO
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)      858 2024-05-24 11:14:58.000000 ptdeco-0.5.0/src/ptdeco.egg-info/SOURCES.txt
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)        1 2024-05-24 11:14:58.000000 ptdeco-0.5.0/src/ptdeco.egg-info/dependency_links.txt
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)       12 2024-05-24 11:14:58.000000 ptdeco-0.5.0/src/ptdeco.egg-info/requires.txt
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)        7 2024-05-24 11:14:58.000000 ptdeco-0.5.0/src/ptdeco.egg-info/top_level.txt
+drwxr-xr-x   0 lopusz   (10000) lopusz   (10000)        0 2024-05-24 11:14:58.522796 ptdeco-0.5.0/tests/
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)     3164 2023-11-09 09:46:50.000000 ptdeco-0.5.0/tests/test_config_torchvision_timm.py
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)     6165 2024-05-09 21:14:08.000000 ptdeco-0.5.0/tests/test_deco_primitives_dwain.py
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)     6144 2024-05-09 21:34:19.000000 ptdeco-0.5.0/tests/test_deco_primitives_falor.py
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)     2686 2023-11-09 09:46:50.000000 ptdeco-0.5.0/tests/test_decompose_torchvision_timm.py
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)     3159 2023-11-15 11:04:35.000000 ptdeco-0.5.0/tests/test_losses_torchvision_timm.py
+-rw-r--r--   0 lopusz   (10000) lopusz   (10000)     2485 2023-11-09 09:46:50.000000 ptdeco-0.5.0/tests/test_wrap_torchvision_timm.py
```

### Comparing `ptdeco-0.4.0/LICENSE` & `ptdeco-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ptdeco-0.4.0/pyproject.toml` & `ptdeco-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ptdeco-0.4.0/setup.py` & `ptdeco-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `ptdeco-0.4.0/src/ptdeco/falor/decomposition.py` & `ptdeco-0.5.0/src/ptdeco/falor/decomposition.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 """Implementation of the FALOR method (FAL = Features Are LOw-Rank)
 
+Inspired by the paper:
+
 Compressing transformers: features are low-rank, but weights are not!,
 Hao Yu, Jianxin Wu, AAAI Conference on Artificial Intelligence (2023)
 
-
 https://doi.org/10.1609/aaai.v37i9.26304
 
 """
 
 import collections
 import collections.abc
 import logging
 import time
 from typing import Any, Optional
 
 import torch
 
 from .. import utils
-from ..utils import modconfig
+
+EIGEN_DAMPEN_FACTOR = 0.01
 
 logger = logging.getLogger(__name__)
 
-__all__ = ["decompose_in_place"]
+__all__ = ["decompose_in_place", "is_decomposeable_module"]
 
 
 class WrappedFALORModule(torch.nn.Module):
     def __init__(self) -> None:
         super().__init__()
 
     def get_weight_copy(self) -> torch.Tensor:
@@ -141,14 +143,17 @@
             in_channels=u.shape[0],
             out_channels=self.conv_orig.out_channels,
             kernel_size=1,
             bias=use_bias,
         )
         conv_1.weight.copy_(u[:, :, None, None])
         conv_2.weight.copy_(v[:, :, None, None])
+        if use_bias:
+            assert conv_2.bias is not None and self.conv_orig.bias is not None
+            conv_2.bias.copy_(self.conv_orig.bias)
         return torch.nn.Sequential(conv_1, conv_2)
 
 
 def _accumulate_Ey_and_Eyyt(
     Ey: torch.Tensor, Eyyt: torch.Tensor, weight: torch.Tensor, x: torch.Tensor
 ) -> tuple[torch.Tensor, torch.Tensor]:
     y = x @ weight.T
@@ -161,30 +166,48 @@
     *,
     root_module: torch.nn.Module,
     decomposed_submodule_name: str,
     data_iterator: collections.abc.Iterator[torch.Tensor],
     weight: torch.Tensor,
     num_data_steps: int,
     device: torch.device,
+    use_float64: bool,
+    use_mean: bool,
+    use_damping: bool,
 ) -> torch.Tensor:
     root_module.eval()
     decomposed_submodule = root_module.get_submodule(decomposed_submodule_name)
     assert isinstance(decomposed_submodule, WrappedFALORModule)
-
-    Ey = torch.zeros(weight.shape[0]).to(device)
-    Eyyt = torch.zeros((weight.shape[0], weight.shape[0])).to(device)
-
+    n_out = weight.shape[0]
+    if use_float64:
+        Ey = torch.zeros(n_out, dtype=torch.float64).to(device)
+        Eyyt = torch.zeros((n_out, n_out), dtype=torch.float64).to(device)
+    else:
+        Ey = torch.zeros(n_out, dtype=torch.float32).to(device)
+        Eyyt = torch.zeros((n_out, n_out), dtype=torch.float32).to(device)
     for i in range(num_data_steps):
         inputs = next(data_iterator).to(device)
         _ = root_module(inputs)
         x = decomposed_submodule.get_last_input()
         Ey, Eyyt = _accumulate_Ey_and_Eyyt(Ey=Ey, Eyyt=Eyyt, weight=weight, x=x)
     Ey /= num_data_steps
     Eyyt /= num_data_steps
-    cov = Eyyt - torch.outer(Ey, Ey)
+    if use_mean:
+        logger.info("Using mean for covariance")
+        cov = Eyyt - torch.outer(Ey, Ey)
+    else:
+        logger.info("Not using mean for covariance")
+        cov = Eyyt
+    if use_damping:
+        # https://stats.stackexchange.com/questions/390532/adding-a-small-constant-to-the-diagonals-of-a-matrix-to-stabilize
+        logger.info("Using damping")
+        damp = EIGEN_DAMPEN_FACTOR * torch.mean(torch.diag(cov))
+        diag = torch.arange(cov.shape[-1], device=cov.device)
+        Eyyt[diag, diag] += damp
+    logger.info(f"{cov.dtype=}")
     _, u = torch.linalg.eigh(cov)
     return u
 
 
 def _compute_metrics(
     *,
     x: torch.Tensor,
@@ -243,24 +266,38 @@
     assert isinstance(decomposed_submodule, WrappedFALORModule)
     orig_module = decomposed_submodule.get_orig_module()
     utils.replace_submodule_in_place(
         root_module, decomposed_submodule_name, orig_module
     )
 
 
+def _is_num_params_reduced(
+    proportion: float,
+    in_features: int,
+    out_features: int,
+) -> bool:
+    baseline_params = in_features * out_features
+    original_rank = min(in_features, out_features)
+    proposed_params = (in_features + out_features) * proportion * original_rank
+    return proposed_params < baseline_params
+
+
 def _process_module(
     *,
     root_module: torch.nn.Module,
     decomposed_submodule_name: str,
     data_iterator: collections.abc.Iterator[torch.Tensor],
     nsr_final_threshold: float,
     kl_final_threshold: float,
     num_data_steps: int,
     num_metric_steps: int,
     device: torch.device,
+    use_float64: bool,
+    use_mean: bool,
+    use_damping: bool,
 ) -> dict[str, Any]:
     decomposed_submodule = root_module.get_submodule(decomposed_submodule_name)
     decomposed_type = utils.get_type_name(decomposed_submodule)
     _wrap_in_place(root_module, decomposed_submodule_name)
     decomposed_submodule = root_module.get_submodule(decomposed_submodule_name)
     assert isinstance(decomposed_submodule, WrappedFALORModule)
     orig_weight = decomposed_submodule.get_weight_copy()
@@ -286,14 +323,17 @@
     u = _compute_decompositon_of_covariance_matrix(
         root_module=root_module,
         decomposed_submodule_name=decomposed_submodule_name,
         data_iterator=data_iterator,
         weight=orig_weight,
         num_data_steps=num_data_steps,
         device=device,
+        use_float64=use_float64,
+        use_mean=use_mean,
+        use_damping=use_damping,
     )
 
     U, V = torch.empty(0), torch.empty(0)
 
     i = 1
 
     # Best rank satisfying conditions kl < kl_threshold and nsr < nsr_threshold
@@ -336,65 +376,69 @@
     assert U.numel() > 0 and V.numel() > 0
     decomposed_submodule.set_weight(orig_weight)
 
     proportion = rank_best / full_rank
     msg_metrics = f"{proportion=:.4f} nsr={nsr_best:.6f} kl={kl_new:.6f}"
     logger.info(f"{msg_prefix} iter=FINAL rank={rank_best} {msg_metrics}")
 
-    if full_rank != rank_best:
+    if full_rank != rank_best and _is_num_params_reduced(proportion, dim_in, dim_out):
         new_decomposed_submodule = decomposed_submodule.get_decomposed_module(
             u=U.T, v=V.T
         )
         new_decomposed_submodule.to(orig_device)
     else:
-        logger.info(f"{msg_prefix} Module decomposed to full rank, not decomposing")
+        msg = f"{proportion=:.4f} leads to num param increase, not decomposing"
+        logger.info(f"{msg_prefix} {msg}")
         new_decomposed_submodule = None
 
     _unwrap_in_place(root_module, decomposed_submodule_name)
     return {
         "proportion": proportion,
         "nsr_final": nsr_new,
         "kl_final": kl_new,
         "decomposed_module": new_decomposed_submodule,
     }
 
 
-def _is_decomposeable_module(module: torch.nn.Module) -> bool:
+def is_decomposeable_module(module: torch.nn.Module) -> bool:
     return isinstance(module, torch.nn.Linear) or (
         isinstance(module, torch.nn.Conv2d)
         and module.kernel_size[0] == 1
         and module.kernel_size[1] == 1
         and module.groups == 1
     )
 
 
 def _get_decomposeable_submodule_names(module: torch.nn.Module) -> list[str]:
     return [
-        name for name, mod in module.named_modules() if _is_decomposeable_module(mod)
+        name for name, mod in module.named_modules() if is_decomposeable_module(mod)
     ]
 
 
-def add_meta_to_module_config(
+def _add_meta_to_module_config(
     module_config: dict[str, Any], module_deco_results: dict[str, Any]
 ) -> None:
     meta = {k: v for k, v in module_deco_results.items() if k != "decomposed_module"}
-    module_config[modconfig.MODCONFIG_META_KEY] = meta
+    module_config[utils.MODCONFIG_META_KEY] = meta
 
 
 def decompose_in_place(
     *,
     module: torch.nn.Module,
     device: torch.device,
     data_iterator: collections.abc.Iterator[torch.Tensor],
     blacklisted_module_names: Optional[list[str]] = None,
     proportion_threshold: float,
     nsr_final_threshold: float,
     kl_final_threshold: float,
     num_data_steps: int,
     num_metric_steps: int,
+    use_float64: bool,
+    use_mean: bool,
+    use_damping: bool,
 ) -> dict[str, Any]:
     start_time = time.perf_counter()
 
     results_all = {}
     decompose_config = {}
 
     if blacklisted_module_names is None:
@@ -416,14 +460,17 @@
                 decomposed_submodule_name=submodule_name,
                 data_iterator=data_iterator,
                 nsr_final_threshold=nsr_final_threshold,
                 kl_final_threshold=kl_final_threshold,
                 num_data_steps=num_data_steps,
                 num_metric_steps=num_metric_steps,
                 device=device,
+                use_float64=use_float64,
+                use_mean=use_mean,
+                use_damping=use_damping,
             )
         results_all[submodule_name] = result
 
     # Decompose
 
     decompose_counter: collections.Counter[str] = collections.Counter()
     for submodule_name in decomposable_submodules:
@@ -431,26 +478,27 @@
         if submodule_name in blacklisted_module_names:
             logger.info(f"{msg_prefix} SKIPPED blacklisted module {submodule_name}")
             continue
 
         assert submodule_name in results_all
         result = results_all[submodule_name]
         new_module = result["decomposed_module"]
+        proportion = result["proportion"]
 
         if new_module is None:
-            logger.info(f"{msg_prefix} SKIPPED module decomposed to full rank")
+            msg = f"SKIPPED {proportion=:.4f} leads to num param increase"
+            logger.info(f"{msg_prefix} {msg}")
             continue
 
-        proportion = result["proportion"]
         if proportion < proportion_threshold:
             old_module = module.get_submodule(submodule_name)
             old_module_type_name = utils.get_type_name(old_module)
             utils.replace_submodule_in_place(module, submodule_name, new_module)
-            module_config = modconfig.get_module_config(new_module)
-            add_meta_to_module_config(module_config, result)
+            module_config = utils.get_module_config(new_module)
+            _add_meta_to_module_config(module_config, result)
             decompose_config[submodule_name] = module_config
             decompose_counter[old_module_type_name] += 1
             logger.info(f"{msg_prefix} finished {proportion=:.3f}")
         else:
             msg_prop = f"{proportion=:.3f} above {proportion_threshold=:.3f}"
             logger.info(f"{msg_prefix} SKIPPED, {msg_prop}")
```

### Comparing `ptdeco-0.4.0/src/ptdeco/lockd/decomposition.py` & `ptdeco-0.5.0/src/ptdeco/lockd/decomposition.py`

 * *Files identical despite different names*

### Comparing `ptdeco-0.4.0/src/ptdeco/lockd/losses.py` & `ptdeco-0.5.0/src/ptdeco/lockd/losses.py`

 * *Files identical despite different names*

### Comparing `ptdeco-0.4.0/src/ptdeco/utils/losses_primitives.py` & `ptdeco-0.5.0/src/ptdeco/utils/losses_primitives.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,23 +8,47 @@
 
 
 def calc_per_channel_noise_to_signal_ratio(
     x: torch.Tensor,
     y: torch.Tensor,
     non_channel_dim: tuple[int, ...] = (0, 2, 3),
     epsilon: float = 1e-3,
+    mode: str = "mean",
 ) -> torch.Tensor:
     y_per_channel_variance = torch.square(torch.std(y, dim=non_channel_dim))
     per_channel_squared_difference = torch.square((x - y)).mean(dim=non_channel_dim)
 
     return torch.divide(
         per_channel_squared_difference, y_per_channel_variance + epsilon
     ).mean()
 
 
+# TODO What to do is this any important?
+
+# def calc_per_channel_noise_to_signal_ratio(
+#     x: torch.Tensor,
+#     y: torch.Tensor,
+#     non_channel_dim: tuple[int, ...] = (0, 2, 3),
+#     epsilon: float = 1e-9,
+#     mode: str = 'mean'
+# ) -> torch.Tensor:
+#     y_per_channel_variance = torch.square(torch.std(y, dim=non_channel_dim))
+#     per_channel_squared_difference = torch.square((x - y)).mean(dim=non_channel_dim)
+#     result = torch.divide(
+#         per_channel_squared_difference, y_per_channel_variance + epsilon
+#     )
+#     result = torch.minimum(result, torch.tensor(1.0, device=x.device))
+#     if mode == 'mean':
+#         return result.mean()
+#     elif mode == 'max':
+#         return result.max()
+#     else:
+#         raise NotImplementedError
+
+
 def calc_kl_divergence(
     q_logits: torch.Tensor,
     p_logits: torch.Tensor,
 ) -> torch.Tensor:
     q_prob = torch.softmax(q_logits, dim=-1)
     p_prob = torch.softmax(p_logits, dim=-1)
     return torch.multiply(p_prob, torch.log(torch.divide(p_prob, q_prob))).sum(dim=1)
```

### Comparing `ptdeco-0.4.0/src/ptdeco/utils/modconfig.py` & `ptdeco-0.5.0/src/ptdeco/utils/modconfig.py`

 * *Files identical despite different names*

### Comparing `ptdeco-0.4.0/src/ptdeco.egg-info/SOURCES.txt` & `ptdeco-0.5.0/src/ptdeco.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -7,20 +7,24 @@
 src/ptdeco/_version.py
 src/ptdeco/py.typed
 src/ptdeco.egg-info/PKG-INFO
 src/ptdeco.egg-info/SOURCES.txt
 src/ptdeco.egg-info/dependency_links.txt
 src/ptdeco.egg-info/requires.txt
 src/ptdeco.egg-info/top_level.txt
+src/ptdeco/dwain/__init__.py
+src/ptdeco/dwain/decomposition.py
 src/ptdeco/falor/__init__.py
 src/ptdeco/falor/decomposition.py
 src/ptdeco/lockd/__init__.py
 src/ptdeco/lockd/decomposition.py
 src/ptdeco/lockd/losses.py
 src/ptdeco/utils/__init__.py
 src/ptdeco/utils/common.py
 src/ptdeco/utils/losses_primitives.py
 src/ptdeco/utils/modconfig.py
 tests/test_config_torchvision_timm.py
+tests/test_deco_primitives_dwain.py
+tests/test_deco_primitives_falor.py
 tests/test_decompose_torchvision_timm.py
 tests/test_losses_torchvision_timm.py
 tests/test_wrap_torchvision_timm.py
```

### Comparing `ptdeco-0.4.0/tests/test_config_torchvision_timm.py` & `ptdeco-0.5.0/tests/test_config_torchvision_timm.py`

 * *Files identical despite different names*

### Comparing `ptdeco-0.4.0/tests/test_decompose_torchvision_timm.py` & `ptdeco-0.5.0/tests/test_decompose_torchvision_timm.py`

 * *Files identical despite different names*

### Comparing `ptdeco-0.4.0/tests/test_losses_torchvision_timm.py` & `ptdeco-0.5.0/tests/test_losses_torchvision_timm.py`

 * *Files identical despite different names*

### Comparing `ptdeco-0.4.0/tests/test_wrap_torchvision_timm.py` & `ptdeco-0.5.0/tests/test_wrap_torchvision_timm.py`

 * *Files identical despite different names*

